<script>
    import Sidebar from "./Sidebar.svelte";
</script>

<main>
    <Sidebar />
    <div class="content">
        <h2>Личная информация</h2>
        <div class="profile">
            <img
                src="https://e7.pngegg.com/pngimages/375/358/png-clipart-song-learning-high-hopes-google-play-user-game-monochrome.png"
                alt="Аватар"
            />
            <div class="details">
                <h3>Кашин Илья Сергеевич</h3>
                <p>user@example.com</p>
            </div>
        </div>

        <h2>История заказов</h2>
        <table>
            <thead>
                <tr>
                    <th>Заказ</th>
                    <th>Дата</th>
                    <th>Статус</th>
                </tr>
            </thead>
            <tbody>
                <tr>
                    <td>#1234</td>
                    <td>01.01.2022</td>
                    <td>В процессе</td>
                </tr>
                <tr>
                    <td>#5678</td>
                    <td>05.02.2022</td>
                    <td>Доставлен</td>
                </tr>
            </tbody>
        </table>
    </div>
</main>

<style>
    h2,
    h3,
    p,
    table,
    tr,
    td {
        margin: 0;
        padding: 0;
    }
    .content {
        margin-top: 20px;
        background-color: #fff;
        padding: 20px;
    }

    h2 {
        font-size: 20px;
        color: #333;
        margin-bottom: 10px;
    }

    .profile {
        display: flex;
        align-items: center;
        margin-bottom: 20px;
    }

    .profile img {
        width: 100px;
        height: 100px;
        border-radius: 50%;
        margin-right: 20px;
    }

    .profile h3 {
        font-size: 18px;
        color: #333;
        margin-bottom: 5px;
    }

    .profile p {
        color: #666;
    }

    table {
        width: 100%;
        border-collapse: collapse;
    }

    table th,
    table td {
        padding: 10px;
        text-align: left;
        border-bottom: 1px solid #ccc;
    }

    table th {
        font-weight: bold;
        background-color: #f5f5f5;
    }
</style>
