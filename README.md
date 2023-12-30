![Tux, the Linux mascot](/assets/logo.png)

## 🔗 Official telegram channel
[![Telegram channel](https://img.shields.io/endpoint?url=https://runkit.io/damiankrawczyk/telegram-badge/branches/master?url=https://t.me/codespec)](https://t.me/codespec)


# Отчет аудита

### Оригинальный репозиторий (private): https://github.com/munris-vlad/layerzero

### Audit Commit hash:                  `33cb4a5cb1dd3f10a113302106cbdf1afa8794b5`

---



## Анализ кода

### Список проверенных файлов:
    
        ------------------------------------------------------------------------------------
        File                                             blank        comment           code
        ------------------------------------------------------------------------------------
        .\package-lock.json                                  0              0           2596
        .\data\abi\zerius.ts                                 1              0            765
        .\modules\fee_checker.ts                            53              2            350
        .\modules\l2pass.ts                                 29              1            228
        .\data\abi\l2telegraph_message.ts                    0              1            225
        .\data\l2telegraphContracts.ts                       3             35            210
        .\config.ts                                          7              5            125
        .\start.ts                                          19              1            125
        .\config_example.ts                                  7              4            123
        .\modules\l2telegraph.ts                            19              1            119
        .\modules\polyhedra.ts                              13              1            119
        .\modules\zerius.ts                                 19              1            119
        .\modules\okx.ts                                    15              1            107
        .\utils\networks.ts                                  7              1            107
        .\modules\merkly.ts                                 17              1            105
        .\utils\routes.ts                                    7              8             77
        .\modules\binance.ts                                10              1             74
        .\utils\clients\bnb.ts                               6              1             58
        .\utils\clients\ethereum.ts                          4              1             57
        .\utils\clients\polygon.ts                           4              1             57
        .\utils\clients\moonbeam.ts                          4              1             56
        .\utils\clients\moonriver.ts                         4              1             56
        .\utils\clients\arbitrum.ts                          4              1             53
        .\utils\clients\zksync.ts                            4              1             50
        .\utils\clients\base.ts                              4              1             48
        .\utils\refill.ts                                   10              1             48
        .\utils\clients\fantom.ts                            4              1             43
        .\utils\clients\optimism.ts                          4              1             43
        .\utils\clients\harmony.ts                           4              1             42
        .\utils\walletStats.ts                               4              1             38
        .\utils\clients\klaytn.ts                            4              1             37
        .\utils\gas.ts                                       6              1             35
        .\data\zeriusContracts.ts                            3              1             31
        .\package.json                                       0              0             29
        .\tsconfig.json                                      0              0             21
        .\data\l2passContracts.ts                            1              1             20
        .\utils\clients\celo.ts                              3              1             19
        .\utils\wallet.ts                                    2              1             19
        .\README.md                                          9              0             18
        .\utils\common.ts                                    4              1             18
        .\rpc_config.ts                                      0              1             14
        .\utils\logger.ts                                    3              1             13
        .\data\merklyContracts.ts                            0              1             12
        .\harmony-converter.ts                               3              1             12
        .\utils\types.ts                                     2              1             12
        .\audit\report.md                                    0              0              7
        .\utils\currentPrice.ts                              1              1              6
        .\logError.js                                        0              1              2
        .\data\abi\l2pass.ts                                 0              1              1
        .\data\abi\l2pass_nft.ts                             0              1              1
        .\data\abi\layerzero.ts                              0              1              1
        .\data\abi\merkly.ts                                 0              1              1
        .\data\abi\polyhedra.ts                              0              1              1
        .\data\polyhedraContracts.ts                         0              1              1
        ------------------------------------------------------------------------------------
        SUM:                                               327             97           6554
        ------------------------------------------------------------------------------------
    

В ходе аудита, уязвимостей в програмном коде длинной `6554` строк найдено не было.


## Адреса контрактов:

### Адреса контрактов, используемые в коде, которые были подтвержденные официальными источниками:


* ### Модуль L2Pass:

    | Protocol           | Chain | Address                                   |
    |--------------------|-------|-------------------------------------------|
    | gas refuel         |  ALL  | 0x222228060e7efbb1d78bb5d454581910e3922222|
    | onft mint + bridge |  ALL  | 0x0000049f63ef0d60abe49fdd8bebfa5a68822222|


* ### Модуль L2Telegraph:

    | Chain      | Address                                   |
    |------------|-------------------------------------------|
    | nova       | 0x5F26EA1E4D47071a4d9A2c2611C2ae0665d64b6d|
    | bsc        | 0x2f4572C09D6bE78F9adc18FE26fB298546eEf58e|
    | zkevm      | 0x1e3F506a665995727456f24e8CcbC4Cab0077Bad|
    | optimism   | 0xa5B72e35E35d219c3274Cee227FbE4D317915E0C|
    | avalanche  | 0x811bcF49225ffE8039989a30cf5C03f60660753d|
    | arbitrum   | 0x479e97FdE57A70bcC85e861EDB71bB613600d55a|
    | polygon    | 0x523d5581A0bb8BB2Bc9f23B5202894E31124eA3e|
    | fantom     | 0xf268D9232Ef928FD2b861a4eC8A7b4195B9e47a7|
    | harmony    | 0x0c49827666ED50407284073c6beA24DA635F78D0|
    | celo       | 0x83017335bAE4837016311bDb75dF5a320b54D636|
    | meter      | 0x46A9f7E1DB25A3c9CFEF6F2635033a9b6E9548dF|
    | zksync     | 0x0D4a6D5964F3b618d8e46BCfBF2792b0D769fBDa|
    | base       | 0x64e0F6164ac110b67Df9A4848707fFbcB86C87a9|
    | linea      | 0x7599d1275831c9fc63f9a27a3c67fe0c8fc19a47|
    | mantle     | 0xDC60fd9d2A4ccF97f292969580874De69E6c326E|
    | tenet      | 0x36a358b3Ba1FB368E35b71ea40c7f4Ab89bFd8e1|
    | canto      | 0x5B10aE182C297ec76fE6fe0E3Da7c4797ceDE02D|
    | zora       | 0x241704d8f874b1f0D7a7dE577BA10fAF004dc0ba|
    | opbnb      | 0xDC60fd9d2A4ccF97f292969580874De69E6c326E|
    | scroll     | 0x9F63DBdF90837384872828d1Ed6Eb424A7F7f939|
    | conflux    | 0xDC60fd9d2A4ccF97f292969580874De69E6c326E|
    | moonbeam   | 0x36a358b3Ba1FB368E35b71ea40c7f4Ab89bFd8e1|
    | shimmer    | 0x811bcF49225ffE8039989a30cf5C03f60660753d|
    | kava       | 0x3Aef52924De5638652c525569373A3D94E0b202f|
    | astar      | 0xDC60fd9d2A4ccF97f292969580874De69E6c326E|
    | telos      | 0xDC60fd9d2A4ccF97f292969580874De69E6c326E|
    | klaytn     | 0xDC60fd9d2A4ccF97f292969580874De69E6c326E|
    | pgn        | 0xDC60fd9d2A4ccF97f292969580874De69E6c326E|
    | gnosis     | 0xE266EedB13A69AF15c1756a241021905B1827F6A|
    | fuse       | 0x811bcF49225ffE8039989a30cf5C03f60660753d|
    | moonriver  | 0x5B10aE182C297ec76fE6fe0E3Da7c4797ceDE02D|
    | orderly    | 0x64e0F6164ac110b67Df9A4848707fFbcB86C87a9|

* ### Модуль Merkly:
    | Chain     | Address                                    |
    |-----------|--------------------------------------------|
    | base      | 0x6bf98654205B1AC38645880Ae20fc00B0bB9FFCA |
    | polygon   | 0x0E1f20075C90Ab31FC2Dd91E536e6990262CF76d |
    | bsc       | 0xeF1eAE0457e8D56A003d781569489Bc5466E574b |
    | optimism  | 0xD7bA4057f43a7C4d4A34634b2A3151a60BF78f0d |
    | celo      | 0xC20A842e1Fc2681920C1A190552A2f13C46e7fCF |
    | klaytn    | 0x79DB0f1A83f8e743550EeB5DD5B0B83334F2F083 |
    | moonriver | 0xd379c3D0930d70022B3C6EBA8217e4B990705540 |
    | fantom    | 0xF56605276cefffe32DFD8B6bF80B93c2A6840136 |
    | moonbeam  | 0x671861008497782F7108D908D4dF18eBf9598b82 |
    | harmony   | 0x671861008497782F7108D908D4dF18eBf9598b82 |
    | zksync    | 0x5673B6e6e51dE3479B8deB22dF46B12308db5E1e |
    | arbitrum  | 0x4Ae8CEBcCD7027820ba83188DFD73CCAD0A92806 |



* ### Модуль Polyhedra:
    | Chain     | Address                                    |
    |-----------|--------------------------------------------|
    | polygon   | 0x4Ab75E9cdF450C4204828c05F01491A356880A16 |


* ### Другие найденные адреса контактов, которые были подтвержденные официальными источниками:
    | Protocol           | Chain | Address                                   |
    |--------------------|-------|-------------------------------------------|
    | Multicall3         |  arbitrum  | 0xca11bde05977b3631167028862be2a173976ca11|
    | Multicall3 |  base  | 0xca11bde05977b3631167028862be2a173976ca11|
    | Multicall3 |  bsc  | 0xca11bde05977b3631167028862be2a173976ca11|
    | Multicall3 |  eth  | 0xca11bde05977b3631167028862be2a173976ca11|
    | Multicall3 |  fantom  | 0xca11bde05977b3631167028862be2a173976ca11|
    | Multicall3 |  moonbeam  | 0xca11bde05977b3631167028862be2a173976ca11|
    | Multicall3 |  moonriver  | 0xca11bde05977b3631167028862be2a173976ca11|
    | Multicall3 |  polygon  | 0xca11bde05977b3631167028862be2a173976ca11|
    | Multicall3 |  zksync  | 0xF9cda624FBC7e059355ce98a31693d299FACd963|



### Адреса контрактов, которые не были подтвержденные официальными источниками:

* ### Zerius:

    Файл `data/zeriusContracts.ts`:

    ```javascript
        export const zeriusBaseContract = '0x9415AD63EdF2e0de7D8B9D8FeE4b939dd1e52F2C'
        export const zeriusBnbContract = '0x5B209E7c81DEaad0ffb8b76b696dBb4633A318CD'
        export const zeriusPolygonContract = '0x2ef766b59e4603250265EcC468cF38a6a00b84b3'
        export const zeriusOptimismContract = '0x2076BDd52Af431ba0E5411b3dd9B5eeDa31BB9Eb'
        export const zeriusCeloContract = '0xFF21d5a3a8e3E8BA2576e967888Deea583ff02f8'
        export const zeriusFantomContract = '0xBFd3539e4e0b1B29e8b08d17f30F1291C837a18E'
        export const zeriusHarmonyContract = '0x5B209E7c81DEaad0ffb8b76b696dBb4633A318CD'
        export const zeriusZksyncContract = '0xeC8Afef7aFe586EB523c228B6BAf3171b1f6dD95'
        export const zeriusArbitrumContract = '0x412aea168aDd34361aFEf6a2e3FC01928Fba1248'

        export const zeriusRefuelContracts: ZeriusRefuelContract = {
            111: '0x2076BDd52Af431ba0E5411b3dd9B5eeDa31BB9Eb',
            102: '0x5B209E7c81DEaad0ffb8b76b696dBb4633A318CD',
            110: '0x412aea168aDd34361aFEf6a2e3FC01928Fba1248',
            109: '0x2ef766b59e4603250265EcC468cF38a6a00b84b3',
            158: '0xBAf5C493a4c364cBD2CA83C355E75F0ff7042945',
            145: '0x1fe2c567169d39CCc5299727FfAC96362b2Ab90E',
            112: '0xBFd3539e4e0b1B29e8b08d17f30F1291C837a18E',
            175: '0x3Fc5913D35105f338cEfcB3a7a0768c48E2Ade8E',
            116: '0x5B209E7c81DEaad0ffb8b76b696dBb4633A318CD',
            125: '0xFF21d5a3a8e3E8BA2576e967888Deea583ff02f8',
            126: '0xb0bea3bB2d6EDDD2014952ABd744660bAeF9747d',
            184: '0x9415AD63EdF2e0de7D8B9D8FeE4b939dd1e52F2C',
            214: '0xB074f8D92b930D3415DA6bA80F6D38f69ee4B9cf',
            195: '0x1fe2c567169d39CCc5299727FfAC96362b2Ab90E',
            151: '0x1b07F1f4F860e72c9367e718a30e38130114AD22',
            181: '0x4F1C698e5cA32b28030E9d9F17C164F27aB5D866',
        }
    ```



## Использованные библиотеки

### Таблица результатов сканирования файла `package.json` на известные уязвимости:

    | Name                | Version          | Issue     |
    |---------------------|------------------|-----------|
    | @harmony-js/crypto  | ^0.1.58          | Not found |
    | axios               | ^1.4.0           | Not found |
    | ccxt                | ^4.1.89          | Not found |
    | https-proxy-agent   | ^7.0.2           | Not found |
    | inquirer            | ^9.2.11          | Not found |
    | op-viem             | ^0.0.1-alpha.7   | Not found |
    | random-words        | ^2.0.0           | Not found |
    | tslog               | ^4.9.2           | Not found |
    | typescript          | ^5.2.2           | Not found |
    | viem                | ^1.15.1          | Not found |

    Источник: snyk.io

Уязвимостей в использованных библиотеках найдено не было.

---

### Рекомендации:

1. **Безопасность кода:**  
   Аудит подтвердил **отсутствие уязвимостей в программном коде**. Это указывает на высокий уровень безопасности и надежности рассматриваемого программного обеспечения.

2. **Адреса контрактов:**  
   Было установлено, что **большинство используемых модулей опираются на адреса контрактов, подтвержденные официальными источниками**. Это обеспечивает дополнительный уровень доверия.

3. **Использование протокола Zerius:**  
   Рекомендуется **проявлять осторожность при использовании модуля Zerius**. 
   Адреса контрактов, указанные автором, не были найдены в официальных источниках в ходе проверки, что может свидетельствовать о потенциальных рисках.

4. **Библиотеки:**  
   В ходе анализа использованных библиотек **уязвимостей не обнаружено**. Это говорит о том, что выбранные для проекта библиотеки являются безопасными и надежными для применения в текущей реализации.

### Общие Выводы:

Отчет показывает, что проверенный код соответствует высоким стандартам безопасности и надежности. Рекомендуется следовать вышеуказанным советам для обеспечения эффективного и безопасного использования программного обеспечения.
