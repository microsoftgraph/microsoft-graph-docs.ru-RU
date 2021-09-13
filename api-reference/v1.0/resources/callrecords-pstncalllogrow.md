---
title: тип ресурсов pstnCallLogRow
description: Представляет строку данных в журнале вызовов для общедоступных телефонных сетей коммутатора (PSTN).
author: williamlooney
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 2a4d14df3b46e4a31d74b2f3a0cf2e111e7d1bc0
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59113821"
---
# <a name="pstncalllogrow-resource-type"></a>тип ресурсов pstnCallLogRow

Пространство имен: microsoft.graph.callRecords

Представляет строку данных в журнале вызовов для общедоступных телефонных сетей коммутатора (PSTN). Каждая строка сопомна одному вызову.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [getPstnCalls](../api/callrecords-callrecord-getpstncalls.md) | [коллекция microsoft.graph.callRecords.pstnCallLogRow](callrecords-pstncalllogrow.md) | Список **объектов pstnCallLogRow** в записи вызовов. |

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|callDurationSource|microsoft.graph.callRecords.pstnCallDurationSource|Источник данных о продолжительности вызова. Если при вызове используется сторонний оператор связи через программу операторов Подключение, оператор может предоставить собственные данные о продолжительности вызова. В этом случае значение свойства `operator` . В противном случае значение `microsoft` .|
|calleeNumber|Строка|Номер, набраный [в формате E.164.](https://en.wikipedia.org/wiki/E.164)|
|callerNumber|Строка|Номер, который получил вызов для входящие вызовы или номер, набраный для исходящие вызовы. Формат E.164.|
|callId|String|Идентификатор вызова. Не гарантируется уникальность.|
|callType|String|Был ли вызов исходящие или входящие вызовы PSTN и тип вызова, например вызов, размещенный пользователем или аудиоконференции.|
|заряд|Двойное с плавающей точкой|Сумма денег или стоимость звонка, который взимается с вашей учетной записи.|
|conferenceId|Строка|ID аудиоконференции.|
|connectionCharge|Двойное с плавающей точкой|Цена платы за подключение.|
|валюта|Строка|Тип валюты, используемой для расчета стоимости вызова[(ISO 4217).](https://en.wikipedia.org/wiki/ISO_4217)|
|destinationContext|Строка|Был ли вызов внутренним (в пределах страны или региона) или международным (за пределами страны или региона) в зависимости от расположения пользователя.|
|destinationName|Строка|Страна или регион, набрана.|
|duration|Int32|Сколько времени вызов был подключен, в секундах.|
|endDateTime|DateTimeOffset|Время окончания вызова.|
|id|Строка|Уникальный идентификатор вызовов. GUID.|
|inventoryType|String|Тип номера телефона пользователя, например служба бесплатного номера.|
|licenseCapability|Строка|Лицензия, используемая для вызова.|
|operator|String|Оператор связи, предоставлял службы PSTN для этого вызова. Это может быть Корпорация Майкрософт или сторонний оператор через программу [операторов Подключение.](https://techcommunity.microsoft.com/t5/microsoft-teams-blog/introducing-operator-connect-and-more-teams-calling-updates/ba-p/2176398)|
|startDateTime|DateTimeOffset|Время начала вызова.|
|tenantCountryCode|Строка|Код страны клиента [ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2).|
|useCountryCode|Строка|Код страны пользователя [ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2).|
|userDisplayName|String|Отображаемое имя пользователя.|
|userId|String|Вызов ID пользователя в Graph. GUID. Эта и другие сведения о пользователях будут null/empty для типов вызовов ботов (ucap_in, ucap_out).|
|userPrincipalName|String|UserPrincipalName (имя регистрации) в Azure Active Directory. Это обычно то же самое, что и SIP-адрес пользователя, и может быть таким же, как и адрес электронной почты пользователя.|

## <a name="relationships"></a>Отношения

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
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
  "inventoryType": "String",
  "operator": "String",
  "callDurationSource": "String"
}
```


