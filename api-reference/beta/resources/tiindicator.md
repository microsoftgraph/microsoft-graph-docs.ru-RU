---
title: Тип ресурса tiIndicator
description: Индикаторы аналитики угроз представляют данные, используемые для идентификации вредоносных действий.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 33c14b4bc60fe492c961445cb294200555e2cc9a
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158746"
---
# <a name="tiindicator-resource-type"></a>Тип ресурса tiIndicator

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Индикаторы аналитики угроз представляют данные, используемые для идентификации вредоносных действий. Если ваша организация работает с индикаторами угроз либо путем создания собственных, получения их из веб-каналов с открытым исходным кодом, обмена данными с партнерскими организациями или сообществами, либо путем приобретения веб-каналов данных, вы можете использовать эти индикаторы в различных средствах безопасности для совпадения с данными журнала. Объект **tiIndicators** API безопасности Microsoft Graph позволяет отправить индикаторы угроз в средства безопасности Майкрософт для действий с разрешением, блокировкой или оповещением.

Индикаторы угроз, загруженные **через tiIndicators,** будут использоваться вместе с аналитикой угроз Майкрософт для предоставления настраиваемой системы безопасности для вашей организации. При использовании объекта **tiIndicators** вы указываете решение безопасности Майкрософт, для которого требуется использовать индикаторы, с помощью свойства **targetProduct** и указываете действие (разрешение, блокировку или оповещение), к которому решение безопасности должно применять индикаторы через свойство **действия.**

Текущая **поддержка targetProduct** включает следующее:

- **Azure Sentinel** — поддерживает все задокументированные методы **tiIndicators,** перечисленные в следующем разделе.
- ATP в Microsoft **Defender (Advanced Threat Protection в Microsoft Defender)** поддерживает следующие методы **tiIndicators:**
     - [Получение объекта tiIndicator](../api/tiindicator-get.md)
     - [Создание объекта tiIndicator](../api/tiindicators-post.md)
     - [Перечисление объектов tiIndicator](../api/tiindicators-list.md)
     - [Обновление](../api/tiindicator-update.md)
     - [удаление](../api/tiindicator-delete.md);

     Поддержка массовых методов появится в ближайшее время.

  > [!NOTE]
  >AtP в Microsoft Defender targetProduct поддерживает следующие типы индикаторов:
  > - Файлы
  > - IP-адреса: ATP в Microsoft Defender поддерживает только IPv4/IPv6 назначения — задав свойство в свойствах networkDestinationIPv4 или networkDestinationIPv6 в API безопасности Microsoft Graph **tiIndicator.**
  > - URL-адреса и домены

   Существует ограничение в 15 000 индикаторов на клиент для ATP в Microsoft Defender.

Подробнее о поддерживаемых типах индикаторов и ограничениях относительно количества индикаторов для каждого клиента см. в статье [Управление индикаторами](/windows/security/threat-protection/microsoft-defender-atp/manage-indicators).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Получение объекта tiIndicator](../api/tiindicator-get.md) | [tiIndicator](tiindicator.md) | Чтение свойств и связей объекта tiIndicator. |
| [Создание объекта tiIndicator](../api/tiindicators-post.md) | [tiIndicator](tiindicator.md) | Создание нового tiIndicator путем публикации в коллекции tiIndicators. |
| [Перечисление объектов tiIndicator](../api/tiindicators-list.md) | [Коллекция tiIndicator](tiindicator.md) | Получите коллекцию объектов tiIndicator. |
| [Обновление](../api/tiindicator-update.md) | [tiIndicator](tiindicator.md) | Обновление объекта tiIndicator. |
| [удаление](../api/tiindicator-delete.md); | Нет | Удаление объекта tiIndicator. |
|[deleteTiIndicators](../api/tiindicator-deletetiindicators.md)|Нет| Удаление нескольких объектов tiIndicator.|
|[deleteTiIndicatorsByExternalId](../api/tiindicator-deletetiindicatorsbyexternalid.md)|Нет| Удаление нескольких объектов tiIndicator по `externalId` свойству.|
|[submitTiIndicators](../api/tiindicator-submittiindicators.md)|[Коллекция tiIndicator](tiindicator.md)|Создание новых tiIndicators путем публикации коллекции tiIndicators.|
|[updateTiIndicators](../api/tiindicator-updatetiindicators.md)|[Коллекция tiIndicator](tiindicator.md)| Обновление нескольких объектов tiIndicator.|

### <a name="methods-supported-by-each-target-product"></a>Методы, поддерживаемые каждым целевым продуктом

| Метод                                                          | Azure Sentinel                                                                                                                                                                                                                                                                                                                                                                      | ATP в Microsoft Defender — это                                                                                                                                                                                               |
|:----------------------------------------------------------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [Создание объекта tiIndicator](../api/tiindicators-post.md)               | Необходимые поля: , , , , , , и по крайней мере `action` `azureTenantId` одна электронная `description` `expirationDateTime` почта, сеть или `targetProduct` `threatType` `tlpLevel` файл.                                                                                                                                                                                                | Обязательными являются следующие поля: и одно из следующих `action` значений: , , , , ( должен предоставить `domainName` в случае `url` `networkDestinationIPv4` `networkDestinationIPv6` `fileHashValue` `fileHashType` `fileHashValue` ). |
| [Отправка tiIndicators](../api/tiindicator-submittiindicators.md) | Необходимые поля [для каждого tiIndicator](../api/tiindicators-post.md) можно найти в методе Create tiIndicator. Ограничение составляет 100 tiIndicators для каждого запроса.                                                                                                                                                                                                                    | Необходимые поля [для каждого tiIndicator](../api/tiindicators-post.md) можно найти в методе Create tiIndicator. Ограничение составляет 100 tiIndicators для каждого запроса.                                                     |
| [Обновление объекта tiIndicator](../api/tiindicator-update.md)              | Необходимые поля: `id` , `expirationDateTime` , `targetProduct` . <br> Редактируемые поля:  `action` , , , , , , `activityGroupNames` , `additionalInformation` , , , , `confidence` , `description` `diamondModel` , `expirationDateTime` `externalId` `isActive` `killChain` `knownFalsePositives` `lastReportedDateTime` `malwareFamilyNames` `passiveOnly` `severity` `tags` `tlpLevel` . | Необходимые поля: `id` , `expirationDateTime` , `targetProduct` . <br> Редактируемые поля: `expirationDateTime` , `severity` , `description` .                                                                         |
| [Обновление tiIndicators](../api/tiindicator-updatetiindicators.md) | Необходимые и редактируемые поля для каждого [tiIndicator](../api/tiindicator-update.md) можно найти в методе Update tiIndicator.                                                                                                                                                                                                                                                       | <p align="center">[Уведомление о проблеме](https://github.com/microsoftgraph/security-api-solutions/issues/new) </p>                                                                                                             |
| [Удаление объекта tiIndicator](../api/tiindicator-delete.md)              | Обязательное поле: `id` .                                                                                                                                                                                                                                                                                                                                                            | Обязательное поле: `id` .                                                                                                                                                                                             |
| [Удаление tiIndicators](../api/tiindicator-deletetiindicators.md) | Обязательное поле [для каждого tiIndicator](../api/tiindicator-delete.md) можно найти в методе Delete tiIndicator выше.                                                                                                                                                                                                                                                               | <p align="center">[Уведомление о проблеме](https://github.com/microsoftgraph/security-api-solutions/issues/new) </p>                                                                                                             |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|action|string| Действие, применяемая при совпадении индикатора из средства безопасности targetProduct. Возможные значения: `unknown`, `allow`, `block`, `alert`. **Обязательно.**|
|activityGroupNames|Коллекция String|Имена аналитики киберугроз для сторон, ответственных за вредоносные действия, на которые распространяется индикатор угроз.|
|additionalInformation|String|Область catchall, в которую могут быть помещены дополнительные данные индикатора, не охваченные другими свойствами tiIndicator. Данные, помещенные в additionalInformation, как правило, не используются средством безопасности targetProduct.|
|azureTenantId|String| Помежается системой, когда индикатор вошел в систему. ИД клиента Azure Active Directory для отправки клиента. **Обязательно.**|
|confidence|Int32|Integer representing the confidence the data within the indicator accurately identifies malicious behavior. Допустимые значения: 0–100, 100 — наивысшее.|
|description|String| Краткое описание (не более 100 символов) угрозы, представляемой индикатором. **Обязательно.**|
|diamondModel|[diamondModel](#diamondmodel-values)|Область диамантской модели, в которой существует этот индикатор. Возможные значения: `unknown`, `adversary`, `capability`, `infrastructure`, `victim`.|
|expirationDateTime|DateTimeOffset| Строка DateTime, указывающая, когда истекает срок действия индикатора. Все индикаторы должны иметь дату окончания срока действия, чтобы избежать сохраняющихся устаревших индикаторов в системе. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. **Обязательно.**|
|externalId|String| Идентификационный номер, который связывает индикатор с системой поставщика индикаторов (например, с внешней клавишей). |
|id|String|Создается системой, когда индикатор засмеяется. Созданный ИДЕНТИФИКАТОР GUID/уникальный идентификатор. Только для чтения.|
|ingestedDateTime|DateTimeOffset| Помежается системой, когда индикатор вошел в систему. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|isActive|Boolean| Используется для отключения индикаторов в системе. По умолчанию все отправленные индикаторы заданы как активные. Однако поставщики могут отправлять существующие индикаторы, для отключения индикаторов в системе для этого установлено "False".|
|killChain|[Коллекция killChain](#killchain-values)|Массив строк JSON, который описывает точку или точку в цепочке событий, на которую направлен этот индикатор. Точные значения см. в приведенном ниже значении "killChain values". |
|knownFalsePositives|String|Сценарии, в которых индикатор может вызывать ложные срабатываия. Это должен быть текст, читаемый человеком.|
|lastReportedDateTime|DateTimeOffset|Время последнего увидеть индикатор. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|malwareFamilyNames|Коллекция String|Имя семейства вредоносных программ, связанное с индикатором, если оно существует. Корпорация Майкрософт по возможности предпочитает имя семейства вредоносных программ Майкрософт, которое можно найти с помощью Защитник Windows аналитики [безопасности.](https://www.microsoft.com/wdsi/threats)|
|passiveOnly|Boolean |Определяет, должен ли индикатор запускать событие, которое видно конечному пользователю. Если установлено "true", средства безопасности не будут уведомлять конечного пользователя о том, что произошло "попадание". Это чаще всего рассматривается как аудит или режим в тихом режиме продуктами безопасности, в которых они просто регистрировали совпадение, но не выполняли это действие. Значение по умолчанию − ложь. |
|severity|Int32| Integer representing the severity of the malicious behavior identified by the data within the indicator. Допустимые значения: от 0 до 5, где 5 — самый серьезный, а ноль — нет. Значение по умолчанию: 3. |
|tags|Коллекция String|Массив строк JSON, который хранит произвольные теги и ключевые слова. |
|targetProduct|String|Строка, представляющая один продукт безопасности, к которому должен применяться индикатор. Допустимые значения: `Azure Sentinel` , `Microsoft Defender ATP` . **Required**|
|threatType|[threatType](#threattype-values)| Каждый индикатор должен иметь допустимый тип угрозы индикатора. Возможные значения: `Botnet`, `C2`, `CryptoMining`, `Darknet`, `DDoS`, `MaliciousUrl`, `Malware`, `Phishing`, `Proxy`, `PUA`, `WatchList`. **Обязательно.** |
|tlpLevel|[tlpLevel](#tlplevel-values)| Значение протокола light traffic light для индикатора. Возможные значения: `unknown`, `white`, `green`, `amber`, `red`. **Обязательно.**|

### <a name="indicator-observables---email"></a>Наблюдаемые индикаторы — электронная почта

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|emailEncoding|String|Тип текстовой кодии, используемой в сообщении электронной почты.|
|emailLanguage|String|Язык сообщения электронной почты.|
|emailRecipient|String|Адрес электронной почты получателя.|
|emailSenderAddress|String|Адрес электронной почты злоумышленника,&#124;злоумышленника.|
|emailSenderName|String|Отображаемого имени злоумышленника,&#124;злоумышленника.|
|emailSourceDomain|String|Домен, используемый в сообщении электронной почты.|
|emailSourceIpAddress|String|Исходный IP-адрес электронной почты.|
|emailSubject|String|Строка темы электронной почты.|
|emailXMailer|String|Значение X-Mailer, используемого в сообщении электронной почты.|

### <a name="indicator-observables---file"></a>Наблюдаемые индикаторы — файл

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|fileCompileDateTime|DateTimeOffset|Дата и время компиляции файла. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|fileCreatedDateTime|DateTimeOffset| Дата и время создания файла. Тип Timestamp представляет сведения о дате и времени в формате ISO 8601 и всегда используется в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|fileHashType|string| Тип hash, хранимый в fileHashValue. Возможные значения: `unknown`, `sha1`, `sha256`, `md5`, `authenticodeHash256`, `lsHash`, `ctph`.|
|fileHashValue|String| Значение hash файла.|
|fileMutexName|String| Имя мьютека, используемого при обнаружении файлов.|
|fileName|String|Имя файла, если индикатор основан на файле. Несколько имен файлов могут быть делегированы запятой. |
|filePacker|String|Упаковщик, используемый для создания нужного файла.|
|filePath|String|Путь к файлу, указывающий на компрометации. Может быть путем к стилю Windows или *nix.|
|fileSize|Int64|Размер файла в ветвях.|
|fileType|String| Текстовое описание типа файла. Например, "Документ Word" или "Двоичный".|

### <a name="indicator-observables---network"></a>Наблюдаемые индикаторы — сеть

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|domainName|String|Доменное имя, связанное с этим индикатором. Должен иметь формат subdomain.domain.toplev rarelyain (например, baddomain.domain.net)|
|networkCidrBlock|String| Представление нотации блокировки CIDR для сети, на который ссылается этот индикатор. Используйте только в том случае, если не удается определить источник и назначение. |
|networkDestinationAsn|Int32|Идентификатор конечной автономной системы сети, на который ссылается индикатор.|
|networkDestinationCidrBlock|String|Представление нотации блокировки CIDR для конечной сети в этом индикаторе.|
|networkDestinationIPv4|String|Назначение IP-адреса IPv4.|
|networkDestinationIPv6|String|Ip-адрес IPv6.|
|networkDestinationPort|Int32|Назначение порта TCP.|
|networkIPv4|String| IP-адрес IPv4. Используйте только в том случае, если источник и назначение не удается определить. |
|networkIPv6|String| IP-адрес IPv6. Используйте только в том случае, если источник и назначение не удается определить. |
|networkPort|Int32| TCP-порт. Используйте только в том случае, если источник и назначение не удается определить. |
|networkProtocol|Int32|Десятиическое представление поля протокола в заголовке IPv4.|
|networkSourceAsn|Int32|Исходный автономный системный идентификатор сети, на который ссылается индикатор.|
|networkSourceCidrBlock|String|Представление нотации блокировки CIDR для сети источника в этом индикаторе|
|networkSourceIPv4|String|Источник IP-адресов IPv4.|
|networkSourceIPv6|String|Источник IP-адресов IPv6.|
|networkSourcePort|Int32|Источник порта TCP.|
|url|String|Унифицированный поиск ресурсов. Этот URL-адрес должен соответствовать RFC 1738.|
|userAgent|String|User-Agent строка из веб-запроса, которая может указывать на компрометации.|

### <a name="diamondmodel-values"></a>значения diamondModel

Сведения об этой модели см. в [примере "Модель диаманта".](http://diamondmodel.org)

| Элемент | Значение | Описание |
|:-------|:----- |:------------|
| unknown |  0    | |
| вися |  1     |Индикатор описывает злоумышленника.|
| capability |  2    |Индикатор — это возможность злоумышленника.|
| инфраструктура | 3  |Индикатор описывает инфраструктуру злоумышленника.|
| victim | 4  |Индикатор описывает жертву злоумышленника.|
| unknownFutureValue | 127 | |

### <a name="killchain-values"></a>значения killChain

| Member | Описание |
|:-------|:------------|
|Действия|Сообщает, что злоумышленник использует скомпрометированную систему для действий, таких как распределенная атака типа "отказ в обслуживании".|
|C2|Представляет канал управления, с помощью которого управляет скомпрометированная система.|
|Delivery|Процесс распространения кода эксплойтов среди злоумышленников (например, USB, электронная почта, веб-сайты).|
|Эксплуатация|Код эксплойтов, который использует уязвимости (например, выполнение кода).|
|Установка|Установка вредоносных программ после уязвимости.|
|Рекогносцировка|Индикатор является свидетельством того, что группа действий собирала информацию, которая будет использоваться в будущих атаках.|
|Виртуализация|Включение уязвимости в код эксплойтов (например, вредоносные программы).|

### <a name="threattype-values"></a>значения threatType

| Member | Описание |
|:-------|:------------|
|Ботнет| Индикатор подробно содержит данные о узле или члене ботсети.|
|C2|Индикатор подробно содержит подробные & управления командой ботсети.|
|CryptoMining|Трафик, включающий этот сетевой адрес или URL-адрес, указывает на то, что cyrptoMining / Resource abuse.|
|Darknet|Индикатор — узел/сеть Темной сети.
|DDoS|Индикаторы, связанные с активной или предстоящей DDoS-кампанией.|
|MaliciousUrl|URL-адрес, обслуживающий вредоносные программы.|
|Вредоносные программы|Индикатор, описывающий вредоносный файл или файлы.|
|Фишинговое|Индикаторы, связанные с фишинговой кампанией.|
|Прокси-сервер|Индикатором является прокси-служба.|
|PuA|Потенциально нежелательные приложения.|
|WatchList|Это универсальный сегмент, в который помещаются индикаторы, когда невозможно точно определить угрозу или потребуется ручная интерпретация. Как правило, партнеры не должны использовать эти данные в системе.|

### <a name="tlplevel-values"></a>Значения tlpLevel

Каждый индикатор также должен иметь значение протокола traffic light при его отправке. Это значение представляет область конфиденциальности и общего доступа для данного индикатора.

| Member | Описание |
|:-------|:------------|
|Белый| Область общего доступа: неограниченный. К индикаторам можно свободно использовать общий доступ без ограничений.|
|Зеленый| Область общего доступа: сообщество. Индикаторы могут быть общими для сообщества безопасности.|
|Amber| Область общего доступа: ограниченная. Это параметр по умолчанию для индикаторов и ограничивает общий доступ только теми службами и операторами служб, которые реализуют аналитику угроз 2) Клиенты, поведение системы которых соответствует индикатору.|
|Красный| Область общего доступа: личная. Эти индикаторы должны быть общими только напрямую и, желательно, лично. Как правило, красные индикаторы TLP не используются из-за заранее определенных ограничений. Если отправлены красные индикаторы TLP, следует также установить свойство `True` PassiveOnly. |

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