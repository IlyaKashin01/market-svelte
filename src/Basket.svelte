<script>
    import Sidebar from "./Sidebar.svelte";
</script>

<main>
    <Sidebar />
    <div class="cart">
        <div class="product-card-basket">
            <img
                src="https://c.dns-shop.ru/thumb/st4/fit/320/250/56d2836ffa0105ca29b69fb304e15f10/f471f73186df557b2322a352d3147c14ea1d65fcbfdfe1129756366247cdf78e.jpg"
                alt="Товар 1"
                class="img-card"
            />
            <div class="description">
                <h3>Компьютер</h3>
                <p>
                    ПК ARDOR GAMING RAGE H322 [Intel Core i5-13400F, 6 x 2.5
                    ГГц, 32 ГБ DDR4, GeForce RTX 4070, SSD 1000 ГБ, без ОС]
                </p>
            </div>
            <input type="number" id="quantity1" value="1" />
            <h4>146 999 ₽</h4>
            <input type="checkbox" id="checkbox1" class="checkbox" />
        </div>
        <div class="product-card-basket">
            <img
                src="https://c.dns-shop.ru/thumb/st4/fit/320/250/aaa5c9e0ff2fb2d11cf07a0b2267c579/1db1b2f57db5a86a13f75eb235c2178cc6ec0d08808a58952056d376d2fc12d2.jpg"
                alt="Товар 2"
                class="img-card"
            />
            <div class="description">
                <h3>Компьютер</h3>
                <p>
                    ПК ARDOR GAMING RAGE H322 [Intel Core i5-13400F, 6 x 2.5
                    ГГц, 32 ГБ DDR4, GeForce RTX 4070, SSD 1000 ГБ, без ОС]
                </p>
            </div>
            <input type="number" id="quantity2" value="1" />
            <h4>87 499 ₽</h4>
            <input type="checkbox" id="checkbox2" class="checkbox" />
        </div>

        <div class="product-card-basket">
            <img
                src="https://c.dns-shop.ru/thumb/st4/fit/320/250/7ff63a73950df6a4c565435618bcca4f/323f353cc37b864b469f5f5d2fdddd0d27fd06b62ce6947975a764f587de5a49.jpg"
                alt="Товар 3"
                class="img-card"
            />
            <div class="description">
                <h3>Компьютер</h3>
                <p>
                    ПК MSI MAG Infinite S3 13TC-853XRU [9S6-B93821-853] [Intel
                    Core i5-13400F, 6 x 2.5 ГГц, 16 ГБ DDR4, GeForce RTX 3060,
                    SSD 512 ГБ, без ОС]
                </p>
            </div>
            <input type="number" id="quantity3" value="1" />
            <h4>146 999 ₽</h4>
            <input type="checkbox" id="checkbox3" class="checkbox" />
        </div>
    </div>
    <div class="cart-total">
        <p>Доставка в пункт выдачи</p>
        <p>г.Владимир</p>
        <p>30 октября</p>
        <p>Оплата картой</p>
        <p>Спишем оплату при получении ?</p>

        <div class="checkbox-pay">
            <input type="checkbox" id="checkbox3" class="checkbox" />
            <p>Оплатить сразу</p>
        </div>
        <p>Товары, 3 шт. 381 497₽</p>
        <p>ИТОГО: 381 497₽</p>
        <button class="order-button">Заказать</button>
    </div>
</main>

<style>
    .cart {
        display: flex;
        flex-direction: column;
        flex-wrap: wrap;
        justify-content: space-between;
        max-width: 70%;
        float: left;
        margin-top: 1%;
        margin-left: 1%;
    }

    .product-card-basket {
        height: 10%;
        display: flex;
        flex-direction: row;
        border: 1px solid #ccc;
        border-radius: 5px;
        padding: 10px;
        margin-bottom: 10px;
        background-color: #f9f9f9;
        justify-content: center;
        align-items: center;
    }

    .img-card {
        width: 10% !important;
        height: 10% !important;
        height: auto;
        border-radius: 5px;
        margin-bottom: 5px;
        margin-right: 1%;
    }

    .description {
        margin-right: 15%;
    }

    .description p {
        width: 500px;
    }

    .product-card-basket h4 {
        float: right;
        width: 20%;
    }

    .product-card-basket input {
        height: 10%;
        width: 10%;
        margin-right: 5%;
    }

    .cart-total {
        float: right;
        margin-top: 1%;
        margin-right: 1%;
        border: 1px solid #ccc;
        border-radius: 5px;
        padding: 10px;
        background-color: #f9f9f9;
        justify-content: center;
        align-items: center;
        text-align: center;
        width: 25%;
    }

    .checkbox {
        width: 20%;
        height: 20%;
    }

    .checkbox-pay {
        display: flex;
        flex-direction: row;
        text-align: center;
        justify-content: center;
    }

    .checkbox-pay p {
        margin: 0;
    }

    .order-button {
        background-color: #ff0000;
        color: #fff;
        border: none;
        padding: 8px 16px;
        border-radius: 5px;
        cursor: pointer;
        width: 40%;
        height: 30%;
    }
</style>
