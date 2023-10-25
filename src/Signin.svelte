<script>
    import { Link } from "svelte-routing";
</script>

<main>
    <div class="Container">
        <div class="FormWrap">
            <button class="market">Market</button>
            <div class="FormContent">
                <form class="Form" action="#">
                    <h1 class="FormH1">Вход в учетную запись</h1>
                    <p class="FormLabel">Логин</p>
                    <input
                        class="FormInput"
                        required
                        type="text"
                        name="login"
                    />
                    <p class="FormLabel">Пароль</p>
                    <input
                        class="FormInput"
                        required
                        type="text"
                        name="password"
                    />
                    <Link to="/catalog">
                        <button class="FormButton" type="submit">Войти</button>
                    </Link>
                    <span class="Text">Забыли пароль?</span>
                </form>
            </div>
        </div>
    </div>
</main>

<style>
    .Container {
        min-height: 50%;
        position: fixed;
        bottom: 0;
        left: 0;
        right: 0;
        top: 0;
        z-index: 0;
        overflow: hidden;
        background: linear-gradient(
            108deg,
            rgba(1, 147, 86, 1) 0%,
            rgba(10, 201, 122, 1) 100%
        );
    }

    .FormWrap {
        height: 100%;
        display: flex;
        flex-direction: column;
        justify-content: center;

        @media screen and (max-width: 480px) {
            height: 80%;
        }
    }

    .market {
        margin-left: 32px;
        margin-top: 32px;
        text-decoration: none;
        color: #fff;
        font-weight: bold;
        font-size: 32px;

        @media screen and (max-width: 480px) {
            margin-left: 16px;
            margin-top: 8px;
        }
    }

    .FormContent {
        height: 100%;
        display: flex;
        flex-direction: column;
        justify-content: center;

        @media screen and (max-width: 480px) {
            padding: 10px;
        }
    }

    .Form {
        background-color: #010101;
        min-width: 25%;
        height: auto;
        width: auto;
        z-index: 1;
        display: grid;
        margin: 0 auto;
        padding: 80px 32px;
        border-radius: 20px;
        box-shadow: 10px 10px 15px rgb(0 0 0 / 90%);

        @media screen and (max-width: 480px) {
            padding: 32px 32px;
        }
    }

    .FormH1 {
        margin-bottom: 5%;
        color: #fff;
        font-size: 20px;
        font-weight: 400;
        text-align: center;
    }

    .FormLabel {
        margin-bottom: 2%;
        font-size: 14px;
        color: #fff;
    }

    .FormInput {
        padding: 16px 16px;
        margin-bottom: 10%;
        border-radius: 4px;
    }

    .FormInput:focus {
        border: 2px solid #01bf71;
    }

    .FormButton {
        background: #01bf71;
        padding: 16px 0;
        border: none;
        border-radius: 4px;
        color: #fff;
        font-size: 20px;
        cursor: pointer;
    }

    .Text {
        text-align: center;
        margin-top: 24px;
        color: #fff;
        font-size: 14px;
    }
</style>
