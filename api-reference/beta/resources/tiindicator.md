---
title: тип ресурса tiIndicator
description: Индикаторы сведении об угрозах представляют данные, используемые для выявления вредоносных действий.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 2f657a68626b7b56a9c91a287e24abb888d90a51
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720209"
---
# <a name="tiindicator-resource-type"></a>тип ресурса tiIndicator

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Индикаторы сведении об угрозах представляют данные, используемые для выявления вредоносных действий. Если ваша организация работает с индикаторами угроз, либо создавая собственные, получать их из каналов с открытым исходным кодом, совместное использование с партнерскими организациями или сообществами, либо приобретая каналы данных, вы можете использовать эти показатели в различных средствах безопасности для совпадения с данными журнала. TiIndicators API Microsoft Graph security **tiIndicators** позволяет загружать индикаторы угроз в средства безопасности Майкрософт для действий разрешить, заблокировать или предупредить.

Индикаторы угроз, загруженные через **tiIndicators,** будут использоваться совместно с microsoft threat intelligence для предоставления настраиваемой системы безопасности для вашей организации. При использовании **сущности tiIndicators** вы указываете решение безопасности Microsoft, для которого необходимо использовать индикаторы с помощью свойства **targetProduct,** и укажите действие (разрешить, заблокировать или предупредить), к которому решение безопасности должно применять индикаторы с помощью свойства **действия.**

Текущая **поддержка targetProduct** включает в себя следующие:

- **Azure Sentinel** — поддерживает все задокументированные методы **tiIndicators,** перечисленные в следующем разделе.
- **Microsoft Defender ATP (Microsoft Defender Advanced Threat Protection)** — поддерживает следующие методы **tiIndicators:**
     - [Получение объекта tiIndicator](../api/tiindicator-get.md)
     - [Создание объекта tiIndicator](../api/tiindicators-post.md)
     - [Перечисление объектов tiIndicator](../api/tiindicators-list.md)
     - [Обновление](../api/tiindicator-update.md)
     - [Удаление](../api/tiindicator-delete.md)

     Поддержка массовых методов скоро появится.

  > [!NOTE]
  >Следующие типы индикаторов поддерживаются целевым продуктом ATP Microsoft Defender:
  > - Файлы
  > - IP-адреса: Microsoft Defender ATP поддерживает только IPv4/IPv6 — задает свойство в свойствах networkDestinationIPv4 или networkDestinationIPv6 в **tiIndicator** API безопасности Microsoft Graph.
  > - URL-адреса/домены

   Существует ограничение в 15000 индикаторов на одного клиента для ATP Защитника Майкрософт.

Подробнее о поддерживаемых типах индикаторов и ограничениях относительно количества индикаторов для каждого клиента см. в статье [Управление индикаторами](/windows/security/threat-protection/microsoft-defender-atp/manage-indicators).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Получение объекта tiIndicator](../api/tiindicator-get.md) | [tiIndicator](tiindicator.md) | Чтение свойств и связей объекта tiIndicator. |
| [Создание объекта tiIndicator](../api/tiindicators-post.md) | [tiIndicator](tiindicator.md) | Создайте новый tiIndicator, разместив в коллекции tiIndicators. |
| [Перечисление объектов tiIndicator](../api/tiindicators-list.md) | [коллекция tiIndicator](tiindicator.md) | Получите коллекцию объектов tiIndicator. |
| [Обновление](../api/tiindicator-update.md) | [tiIndicator](tiindicator.md) | Обновление объекта tiIndicator. |
| [Удаление](../api/tiindicator-delete.md) | Нет | Удаление объекта tiIndicator. |
|[deleteTiIndicators](../api/tiindicator-deletetiindicators.md)|Нет| Удаление нескольких объектов tiIndicator.|
|[deleteTiIndicatorsByExternalId](../api/tiindicator-deletetiindicatorsbyexternalid.md)|Нет| Удаление свойством нескольких объектов tiIndicator. `externalId`|
|[submitTiIndicators](../api/tiindicator-submittiindicators.md)|[коллекция tiIndicator](tiindicator.md)|Создайте новые tiIndicators, разместив коллекцию tiIndicators.|
|[updateTiIndicators](../api/tiindicator-updatetiindicators.md)|[коллекция tiIndicator](tiindicator.md)| Обновление нескольких объектов tiIndicator.|

### <a name="methods-supported-by-each-target-product"></a>Методы, поддерживаемые каждым целевым продуктом

| Method                                                          | Azure Sentinel                                                                                                                                                                                                                                                                                                                                                                      | ATP в Microsoft Defender — это                                                                                                                                                                                               |
|:----------------------------------------------------------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [Создание объекта tiIndicator](../api/tiindicators-post.md)               | Необходимые поля: , , , , , , , и по крайней мере одна `action` `azureTenantId` электронная `description` почта, сеть или файл `expirationDateTime` `targetProduct` `threatType` `tlpLevel` наблюдаемых.                                                                                                                                                                                                | Обязательными полями являются: и одно из следующих `action` значений: , , , , ( должны `domainName` `url` `networkDestinationIPv4` `networkDestinationIPv6` `fileHashValue` поставлять в случае `fileHashType` `fileHashValue` ). |
| [Отправка tiIndicators](../api/tiindicator-submittiindicators.md) | Обратитесь к [методу Create tiIndicator](../api/tiindicators-post.md) для необходимых полей для каждого tiIndicator. Существует ограничение в 100 tiIndicators на запрос.                                                                                                                                                                                                                    | Обратитесь к [методу Create tiIndicator](../api/tiindicators-post.md) для необходимых полей для каждого tiIndicator. Существует ограничение в 100 tiIndicators на запрос.                                                     |
| [Обновление объекта tiIndicator](../api/tiindicator-update.md)              | Необходимые поля: `id` , `expirationDateTime` `targetProduct` . <br> Редактируемые поля:  `action` , , , , , `activityGroupNames` , `additionalInformation` `confidence` `description` `diamondModel` `expirationDateTime` `externalId` , `isActive` `killChain` `knownFalsePositives` `lastReportedDateTime` `malwareFamilyNames` `passiveOnly` `severity` `tags` `tlpLevel` . | Необходимые поля: `id` , `expirationDateTime` `targetProduct` . <br> Редактируемые поля: `expirationDateTime` `severity` , `description` .                                                                         |
| [Обновление tiIndicators](../api/tiindicator-updatetiindicators.md) | Обратитесь к [методу Update tiIndicator](../api/tiindicator-update.md) для необходимых и редактируемых полей для каждого tiIndicator.                                                                                                                                                                                                                                                       | <p align="center">[Уведомление о проблеме](https://github.com/microsoftgraph/security-api-solutions/issues/new) </p>                                                                                                             |
| [Удаление объекта tiIndicator](../api/tiindicator-delete.md)              | Необходимое поле: `id` .                                                                                                                                                                                                                                                                                                                                                            | Необходимое поле: `id` .                                                                                                                                                                                             |
| [Удаление tiIndicators](../api/tiindicator-deletetiindicators.md) | Обратитесь к [методу Delete tiIndicator](../api/tiindicator-delete.md) выше для требуемого поля для каждого tiIndicator.                                                                                                                                                                                                                                                               | <p align="center">[Уведомление о проблеме](https://github.com/microsoftgraph/security-api-solutions/issues/new) </p>                                                                                                             |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|action|Строка| Действие, применяемая, если индикатор соответствует из средства безопасности targetProduct. Возможные значения: `unknown`, `allow`, `block`, `alert`. **Обязательное поле.**|
|activityGroupNames|Коллекция объектов string|Имя разведки киберугроз для сторон, ответственных за вредоносную деятельность, подпадаемую под индикатор угрозы.|
|additionalInformation|String|Область catchall, в которую могут быть помещены дополнительные данные из индикатора, не охваченного другими свойствами tiIndicator. Данные, помещенные в дополнительнуюinformation, как правило, не будут использоваться средством безопасности targetProduct.|
|azureTenantId|String| Штампуется системой при прохохо-стике индикатора. ID клиента Azure Active Directory для отправки клиента. **Обязательное поле.**|
|confidence|Int32|Integer, представляющий доверие к данным в индикаторе, точно определяет вредоносное поведение. Допустимые значения : 0 — 100, а 100 — самые высокие.|
|description|String| Краткое описание (100 символов или менее) угрозы, представленной индикатором. **Обязательное поле.**|
|diamondModel|[diamondModel](#diamondmodel-values)|Область бриллиантовой модели, в которой существует этот индикатор. Возможные значения: `unknown`, `adversary`, `capability`, `infrastructure`, `victim`.|
|expirationDateTime|DateTimeOffset| Строка DateTime, указывающая, когда истекает срок действия индикатора. Чтобы избежать сохраняющихся в системе устаревших индикаторов, все индикаторы должны иметь дату истечения срока действия. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. **Обязательное поле.**|
|externalId|String| Идентификационный номер, который связывает индикатор с системой поставщика индикаторов (например, с иностранным ключом). |
|id|String|Создается системой при прохо-мыве индикатора. Созданный GUID/уникальный идентификатор. Только для чтения.|
|ingestedDateTime|DateTimeOffset| Штампуется системой при прохохо-стике индикатора. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|isActive|Boolean| Используется для отключения индикаторов внутри системы. По умолчанию любой представленный индикатор задан как активный. Однако для отключения индикаторов в системе поставщики могут отправлять существующие индикаторы с этим набором в "False".|
|killChain|[коллекция killChain](#killchain-values)|Массив строк JSON, который описывает, какие точки или точки на цепочке убийств этот индикатор цели. Для точных значений см. ниже значения killChain. |
|knownFalsePositives|String|Сценарии, в которых индикатор может вызывать ложные срабатыва- Это должен быть текст, читаемый для человека.|
|lastReportedDateTime|DateTimeOffset|Последний раз индикатор был замечен. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|malwareFamilyNames|Коллекция объектов string|Семейство вредоносных программ, связанное с индикатором, если оно существует. Корпорация Майкрософт предпочитает имя семейства вредоносных программ Майкрософт, если это возможно, которое можно найти в энциклопедии Защитник Windows security [Intelligence.](https://www.microsoft.com/wdsi/threats)|
|passiveOnly|Boolean |Определяет, должен ли индикатор вызвать событие, которое видно конечному пользователю. При наборе "true" средства безопасности не будут уведомлять конечного пользователя о том, что произошло "попадание". Это чаще всего рассматривается как режим аудита или бесшумного режима с помощью продуктов безопасности, в которых они просто регистрировали совпадение, но не выполняли действие. Значение по умолчанию − ложь. |
|severity|Int32| Набор, представляющий серьезность вредоносного поведения, определяемого данными в индикаторе. Допустимые значения : 0 — 5, где 5 является самым строгим, а нуль — не очень серьезным. Значение по умолчанию: 3. |
|tags|Коллекция объектов string|Массив строк JSON, который хранит произвольные теги и ключевые слова. |
|targetProduct|String|Строковая величина, представляющая один продукт безопасности, к которому должен применяться индикатор. Допустимые значения: `Azure Sentinel` , `Microsoft Defender ATP` . **Required**|
|threatType|[threatType](#threattype-values)| Каждый индикатор должен иметь допустимый тип угрозы индикатора. Возможные значения: `Botnet`, `C2`, `CryptoMining`, `Darknet`, `DDoS`, `MaliciousUrl`, `Malware`, `Phishing`, `Proxy`, `PUA`, `WatchList`. **Обязательное поле.** |
|tlpLevel|[tlpLevel](#tlplevel-values)| Значение Протокола светофора для индикатора. Возможные значения: `unknown`, `white`, `green`, `amber`, `red`. **Обязательное поле.**|

### <a name="indicator-observables---email"></a>Наблюдаемые индикаторы — электронная почта

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|emailEncoding|String|Тип коди-кодии текста, используемый в электронной почте.|
|emailLanguage|String|Язык электронной почты.|
|emailRecipient|String|Адрес электронной почты получателя.|
|emailSenderAddress|String|Адрес электронной почты злоумышленника&#124;жертвы.|
|emailSenderName|String|Отображается имя злоумышленника&#124;жертвы.|
|emailSourceDomain|String|Домен, используемый в электронной почте.|
|emailSourceIpAddress|String|Исходный IP-адрес электронной почты.|
|emailSubject|String|Тема строки электронной почты.|
|emailXMailer|String|Значение X-Mailer, используемого в электронной почте.|

### <a name="indicator-observables---file"></a>Наблюдаемые индикаторы — файл

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|fileCompileDateTime|DateTimeOffset|DateTime, когда файл был скомпилирован. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|fileCreatedDateTime|DateTimeOffset| DateTime, когда файл был создан. Тип Timestamp представляет сведения о дате и времени в формате ISO 8601 и всегда находится во времени UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|fileHashType|Строка| Тип hash, хранимый в fileHashValue. Возможные значения: `unknown`, `sha1`, `sha256`, `md5`, `authenticodeHash256`, `lsHash`, `ctph`.|
|fileHashValue|String| Значение hash файла.|
|fileMutexName|String| Имя Mutex, используемого в обнаружениях на основе файлов.|
|fileName|String|Имя файла, если индикатор основан на файле. Несколько имен файлов могут быть делимитированы запятой. |
|filePacker|String|Упаковщик, используемый для создания файла, о чем идет речь.|
|filePath|String|Путь файла, указывающий компромисс. Может быть путь в стиле Windows или *nix.|
|fileSize|Int64|Размер файла в bytes.|
|fileType|String| Текстовое описание типа файла. Например, "Word Document" или "Binary".|

### <a name="indicator-observables---network"></a>Наблюдаемые индикаторы — сеть

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|domainName|String|Доменное имя, связанное с этим индикатором. Должен быть формат subdomain.domain.toplev rarelyain (Например, baddomain.domain.net)|
|networkCidrBlock|String| Представление нотации ciDR Block для сети, ссылаясь на этот индикатор. Используйте только в том случае, если источник и пункт назначения не могут быть определены. |
|networkDestinationAsn|Int32|Идентификатор автономной системы назначения сети, на который ссылается индикатор.|
|networkDestinationCidrBlock|String|Представление нотации ciDR Block в сети назначения в этом индикаторе.|
|networkDestinationIPv4|String|Назначение IP-адресов IPv4.|
|networkDestinationIPv6|String|Назначение IP-адресов IPv6.|
|networkDestinationPort|Int32|Пункт назначения порта TCP.|
|networkIPv4|String| IP-адрес IPv4. Используйте только в том случае, если источник и пункт назначения не могут быть определены. |
|networkIPv6|String| IP-адрес IPv6. Используйте только в том случае, если источник и пункт назначения не могут быть определены. |
|networkPort|Int32| Порт TCP. Используйте только в том случае, если источник и пункт назначения не могут быть определены. |
|networkProtocol|Int32|Десятичной представление поля протокола в заголовке IPv4.|
|networkSourceAsn|Int32|Исходный автономный системный идентификатор сети, на который ссылается индикатор.|
|networkSourceCidrBlock|String|Представление нотации блока CIDR для исходных сетей в этом индикаторе|
|networkSourceIPv4|String|Источник IP-адресов IPv4.|
|networkSourceIPv6|String|Источник IP-адресов IPv6.|
|networkSourcePort|Int32|Источник порта TCP.|
|url|String|Единый локатор ресурсов. Этот URL-адрес должен соответствовать RFC 1738.|
|userAgent|String|User-Agent строка из веб-запроса, которая может указывать на компромисс.|

### <a name="diamondmodel-values"></a>значения diamondModel

Сведения об этой модели см. в [примере The Diamond Model.](http://diamondmodel.org)

| Элемент | Значение | Описание |
|:-------|:----- |:------------|
| unknown |  0    | |
| adversary |  1    |Индикатор описывает противника.|
| возможности |  2    |Индикатор — это возможность противника.|
| инфраструктура | 3  |Индикатор описывает инфраструктуру противника.|
| жертва | 4  |Индикатор описывает жертву противника.|
| unknownFutureValue | 127 | |

### <a name="killchain-values"></a>значения killChain

| Member | Описание |
|:-------|:------------|
|Actions|Сообщается, что злоумышленник использует скомпрометированную систему для действий, таких как распределенная атака отказа в обслуживании.|
|C2|Представляет канал управления, с помощью которого управляется скомпрометированная система.|
|Delivery|Процесс распространения кода эксплойтов среди жертв (например, USB, электронная почта, веб-сайты).|
|Эксплуатация|Код эксплойтов, используя уязвимости (например, выполнение кода).|
|Установка|Установка вредоносных программ после использования уязвимости.|
|Рекогносцировка|Индикатор является свидетельством сведений о сборе данных группы действий, которые будут использоваться в будущей атаке.|
|Везамизация|Превращение уязвимости в код эксплойтов (например, вредоносные программы).|

### <a name="threattype-values"></a>значения threatType

| Member | Описание |
|:-------|:------------|
|Botnet| Индикатор подробно содержит узел или член ботсети.|
|C2|Индикатор подробно содержит командный узел & управления ботсети.|
|CryptoMining|Трафик, связанный с этим сетевым адресом или URL-адресом, указывает на злоупотребление ресурсами и cyrptoMining.|
|Darknet|Индикатор — это узел/сеть Darknet.
|DDoS|Индикаторы, относящиеся к активной или предстоящей DDoS-кампании.|
|MaliciousUrl|URL-адрес, обслуживающий вредоносные программы.|
|Вредоносные программы|Индикатор, описывающий вредоносный файл или файлы.|
|Фишинговое|Индикаторы, относящиеся к фишинговой кампании.|
|Прокси-сервер|Индикатор — это прокси-служба.|
|PUA|Потенциально нежелательное приложение.|
|WatchList|Это общее ведро, в которое помещаются индикаторы, когда невозможно точно определить, что представляет собой угроза или потребуется ручная интерпретация. Обычно это не следует использовать партнерам, относя к системе данные.|

### <a name="tlplevel-values"></a>значения tlpLevel

Каждый индикатор также должен иметь значение Протокола светофора при его отправке. Это значение представляет область чувствительности и общего доступа к данному индикатору.

| Member | Описание |
|:-------|:------------|
|Белый| Область общего доступа: Unlimited. Индикаторы можно использовать свободно, без ограничений.|
|Зеленый| Область общего доступа. Сообщество. Индикаторы могут быть общими для сообщества безопасности.|
|Amber| Область общего доступа: Ограниченная. Это параметр по умолчанию для индикаторов и ограничивает общий доступ только к тем, у которых "необходимо знать" является 1) Службы и операторы служб, реализуют сведения об угрозах 2) Клиенты, чьи системы (ы) демонстрируют поведение, соответствующее индикатору.|
|Красный| Область общего доступа: Personal. Эти показатели должны быть общими только непосредственно и, желательно, лично. Как правило, красные индикаторы TLP не используются из-за заранее определенных ограничений. Если представлены красные индикаторы TLP, следует также установить свойство `True` PassiveOnly. |

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.tiIndicator",
  "keyProperty": "id"
}-->

```json
{
  "action": "string",
  "activityGroupNames": ["String"],
  "additionalInformation": "String",
  "azureTenantId": "String",
  "confidence": 1024,
  "description": "String",
  "diamondModel": "string",
  "domainName": "String",
  "emailEncoding": "String",
  "emailLanguage": "String",
  "emailRecipient": "String",
  "emailSenderAddress": "String",
  "emailSenderName": "String",
  "emailSourceDomain": "String",
  "emailSourceIpAddress": "String",
  "emailSubject": "String",
  "emailXMailer": "String",
  "expirationDateTime": "String (timestamp)",
  "externalId": "String",
  "fileCompileDateTime": "String (timestamp)",
  "fileCreatedDateTime": "String (timestamp)",
  "fileHashType": "string",
  "fileHashValue": "String",
  "fileMutexName": "String",
  "fileName": "String",
  "filePacker": "String",
  "filePath": "String",
  "fileSize": 1024,
  "fileType": "String",
  "id": "String (identifier)",
  "ingestedDateTime": "String (timestamp)",
  "isActive": true,
  "killChain": ["String"],
  "knownFalsePositives": "String",
  "lastReportedDateTime": "String (timestamp)",
  "malwareFamilyNames": ["String"],
  "networkCidrBlock": "String",
  "networkDestinationAsn": 1024,
  "networkDestinationCidrBlock": "String",
  "networkDestinationIPv4": "String",
  "networkDestinationIPv6": "String",
  "networkDestinationPort": 1024,
  "networkIPv4": "String",
  "networkIPv6": "String",
  "networkPort": 1024,
  "networkProtocol": 1024,
  "networkSourceAsn": 1024,
  "networkSourceCidrBlock": "String",
  "networkSourceIPv4": "String",
  "networkSourceIPv6": "String",
  "networkSourcePort": 1024,
  "passiveOnly": true,
  "severity": 1024,
  "tags": ["String"],
  "targetProduct": "String",
  "threatType": "String",
  "tlpLevel": "string",
  "url": "String",
  "userAgent": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "tiIndicator resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->