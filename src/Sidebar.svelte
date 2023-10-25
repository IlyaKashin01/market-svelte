<script>
    import { Link, Router } from "svelte-routing";
</script>

<main>
    <div class="header">
        <div class="logo">
            <button>
                <Link to="/catalog"><h1>Market</h1></Link>
            </button>
        </div>
        <div class="search">
            <input type="text" placeholder="Поиск" />
        </div>
        <div class="icons">
            <Router>
                <Link to="/basket">
                    <button>
                        <img
                            src="https://pngteam.com/images/cart-png-980x804_cf7c7237_transparent_202743.png.png"
                            alt="Корзина"
                        />
                        <h3>Корзина</h3>
                    </button>
                </Link>
                <Link to="/profile">
                    <button>
                        <img
                            src="https://uploads-ssl.webflow.com/612e1151f336d5488bcf09cf/612e3216fc10566ce6bcfdb7_kirjaudu%20sisään%20(1).png"
                            alt="Профиль"
                        />
                        <h3>Профиль</h3>
                    </button>
                </Link>
            </Router>
        </div>
    </div>
</main>

<style>
    .header {
        background-color: #2b2d33;
        display: flex;
        padding: 10px;
        align-items: center;
        justify-content: space-between;
    }

    .logo h1 {
        display: inline;
        margin-left: 10px;
        font-size: 40px;
        color: #ffffff;
    }

    .logo button {
        overflow: hidden;
        background-color: #2b2d33;
        border: none;
    }

    .search input {
        padding: 5px;
        border: 1px solid #ccc;
        border-radius: 25px;
        width: 500px;
        height: 40px;
    }

    .icons {
        display: flex;
        align-items: center;
    }

    .icons button {
        background-color: transparent;
        border: none;
        cursor: pointer;
        color: #ffffff;
    }

    .icons button img {
        width: 30px;
        height: 30px;
        filter: invert(100%);
    }

    @media screen and (max-width: 768px) {
        .logo h1 {
            display: inline;
            font-size: 20px;
            color: #ffffff;
        }

        .logo button {
            overflow: hidden;
            background-color: #2b2d33;
            border: none;
        }

        .search input {
            padding: 5px;
            border: 1px solid #ccc;
            border-radius: 20px;
            width: 80%;
            margin-left: 5%;
            height: 40px;
        }

        .icons {
            display: flex;
            align-items: center;
        }

        .icons button {
            background-color: transparent;
            border: none;
            margin-right: 10px;
            cursor: pointer;
            color: #ffffff;
        }

        .icons button img {
            width: 20px;
            height: 20px;
            filter: invert(100%);
        }

        .icons h3 {
            font-size: small;
        }
    }
</style>
