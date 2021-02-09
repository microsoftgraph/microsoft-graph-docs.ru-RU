---
title: Тип ресурса pstnCallLogRow
description: Представляет строку данных в журнале вызовов телефонной сети общего коммутатора (PSTN).
author: williamlooney
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 5103404bdaa6ac4eafbfcffd45deef41c217600a
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50155582"
---
# <a name="pstncalllogrow-resource-type"></a>Тип ресурса pstnCallLogRow

Пространство имен: microsoft.graph.callRecords

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет строку данных в журнале вызовов телефонной сети общего коммутатора (PSTN). Каждая строка сопозовна одному вызову.

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор вызова. GUID.|
|callId|String|Идентификатор вызова. Не гарантируется уникальность.|
|userId|String|ИД вызываемого пользователя в Graph. GUID. Эти и другие сведения о пользователе будут пустыми или пустыми для типов вызовов ботов (ucap_in, ucap_out).|
|userPrincipalName|String|UserPrincipalName (имя для регистрации) в Azure Active Directory. Обычно он такой же, как SIP-адрес пользователя, и может быть таким же, как и адрес электронной почты пользователя.|
|userDisplayName|String|Отображаемое имя пользователя.|
|startDateTime|DateTimeOffset|Время начала вызова.|
|endDateTime|DateTimeOffset|Время окончания вызова.|
|duration|Int32|Время подключения вызова в секундах.|
|charge|Двойное с плавающей точкой|Сумма денег или стоимость вызова, который взимается с вашей учетной записи.|
|callType|String|Был ли вызов исходящие или входящие вызовы STN, а также тип вызова, например звонок, который был сделан пользователем или аудиоконференции.|
|currency|String|Тип валюты, используемой для расчета стоимости вызова[(ISO 4217).](https://en.wikipedia.org/wiki/ISO_4217)|
|calleeNumber|String|Номер, набираемый [в формате E.164.](https://en.wikipedia.org/wiki/E.164)|
|usageCountryCode|String|Код страны пользователя, [ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2).|
|tenantCountryCode|String|Код страны клиента, [ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2).|
|connectionCharge|Двойное с плавающей точкой|Цена платы за подключение.|
|callerNumber|String|Номер, который принял вызов для входящие вызовы, или номер, набираемый для исходящие вызовы. Формат E.164.|
|destinationContext|String|Был ли звонок внутренним (внутри страны или региона) или международным (за пределами страны или региона) в зависимости от расположения пользователя.|
|destinationName|String|Страна или регион набрана.|
|conferenceId|String|ИД аудиоконференции.|
|licenseCapability|String|Лицензия, используемая для вызова.|
|inventoryType|String|Тип номера телефона пользователя, например служба бесплатных номеров.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "ignored",
  "@odata.type": "microsoft.graph.callRecords.pstnCallLogRow",
  "keyProperty": "id"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.callRecords.pstnCallLogRow",
  "id": "String (identifier)",
  "callId": "String",
  "userId": "String",
  "userPrincipalName": "String",
  "userDisplayName": "String",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "duration": "Integer",
  "charge": "Double",
  "callType": "String",
  "currency": "String",
  "calleeNumber": "String",
  "usageCountryCode": "String",
  "tenantCountryCode": "String",
  "connectionCharge": "Double",
  "callerNumber": "String",
  "destinationContext": "String",
  "destinationName": "String",
  "conferenceId": "String",
  "licenseCapability": "String",
  "inventoryType": "String"
}
```


