# Майнинг и вознаграждения

Кто является наиболее подходящими майнерами для Meson Network?

- Постоянные пользователи пропускной способности
- Статический IP домашних пользователей
- Владельцы устройств IoT
- Владельцы выделенных серверов
- Владельцы серверов IDC (корпорации/организации/школы).

Все они с радостью становятся нашими самыми стабильными поставщиками. В результате чего, максимально используя эти незадействованные ресурсы, модель становится экономичной и здоровой в соответствии с планом и позиционированием проекта Meson Network.

## Предварительные условия

- Статический (публичный) IP или резервирование DHCP
- Открытие порта брандмауэра (по умолчанию: 443, поддержка пользовательских портов сервера)
- Обеспечение достаточного объема памяти (минимальные требования по умолчанию: 20 Гб)

## Правила майнинга (расчет награды)

Пожалуйста, взгляните для подробностей [miningrules](https://dashboard.meson.network/ming_rules_msntt).

Mining Score = Bandwidth Score * Storage Score * Credit Score

::: tip Ру перевод
Оценка Майнинга = Оценка пропускной способности * Оценка хранилища (гб) * Рейтинг
:::

В основном, пропускная способность является наиболее важным сопутствующим фактом для BandwidthScore.

А место для хранения необходимо для кэширования файлов для StorageScore. 

Кроме того, постоянные и стабильные серверы будут иметь более высокий CreditScore.

Также будут некоторые корректировки вознаграждения для серверов в разных регионах.
Basically, Bandwidth is the most important related fact for BandwidthScore.

<div style="text-align:center">
<table>
    <tr>
        <td>Item</td>
        <td>Value</td>
    </tr>
    <tr>
        <td>Сеть</td>
        <td>TestNet</td>
    </tr>
    <tr>
        <td>Mining Score</td>
        <td>Mining Score = Bandwidth Score * Storage Score * Credit Score</td>
    </tr>
    <tr>
        <td>Процент заработка некоторого узла</td>
        <td><img src="./images/percentage.svg" /></td>
    </tr>
    <tr>
        <td>Оценка пропускной способности</td>
        <td><img src="./images/bandwidth-score.svg" /></td>
    </tr>
    <tr>
        <td>Верхняя граница полосы пропускания</td>
        <td>Показатель пропускной способности не увеличивается после достижения пропускной способности 1500 Мб/с</td>
    </tr>
    <tr>
        <td>Оценка хранения</td>
        <td><img src="./images/storage-score.svg" /></td>
    </tr>
    <tr>
        <td>Минимальная потребность в хранении</td>
        <td>20GB</td>
    </tr>
    <tr>
        <td>Credit Score (Оценка)</td>
        <td><img src="./images/credit-score.svg" /><br>Если ваш узел находится в режиме онлайн и стабилен, кредит будет постепенно увеличиваться до максимального значения 10000000 Когда ваш узел переходит в автономный режим, кредит будет постепенно уменьшаться до 0.</td>
    </tr>
    <tr>
        <td>Пример</td>
        <td align="left">Если ваша пропускная способность составляет 200 Мб/с, "Bandwidth score" будет равен 200<br>Если вы установили объем хранилища 60 Гб, "Storage score" будет равен 0,85 Если ваш кредит составляет 500000, "Credit score" будет равен 0,7<br>Mining score = 200 * 0,85 * 0,7 = 119</td>
    </tr>
</table>
</div>

Все токены Testnet будут сопоставлены с 1% токенов Mainnet. Согласно FAQ-Token, будет выпущено 100 000 000 начальных токенов Meson, из которых 1 000 000 токенов будут использоваться в качестве обмена токенов Testnet.

**Ваши токены Mainnet = (Ваши токены Testnet / Все токены Testnet) * (1% * Все токены Mainnet) = (Ваши токены Testnet / Все токены Testnet) * 1,000,000**

Например, предположим, что всего будет 160 000 000 токенов Testnet, а у вас на тот момент было 2 000 000 токенов Testnet, тогда вы получите (2 000 000 / 160 000 000) * 1 000 000 = 12500 токенов Mainnet.