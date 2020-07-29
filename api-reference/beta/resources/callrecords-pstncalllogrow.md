---
title: Тип ресурса Пстнкалллогров
description: Представляет строку данных в журнале звонков телефонной сети общего пользования (PSTN).
author: stephenjust
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: fdcaaa311ea3d1f875bd3933420cfed058ef7808
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/29/2020
ms.locfileid: "46510337"
---
# <a name="pstncalllogrow-resource-type"></a>Тип ресурса Пстнкалллогров

Пространство имен: microsoft.graph.callRecords

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет строку данных в журнале звонков телефонной сети общего пользования (PSTN). Каждая строка соответствует одному вызову.

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор звонка. Кодом.|
|callId|Строка|Идентификатор вызова. Не гарантируется уникальным.|
|userId|String|Идентификатор вызывающего пользователя в Graph. Кодом. Эта и другие сведения о пользователе будут иметь значение null или Empty для типов вызовов Bot (ucap_in, ucap_out).|
|userPrincipalName|Строка|UserPrincipalName (имя входа) в Azure Active Directory. Обычно это тот же адрес SIP, что и адрес электронной почты пользователя.|
|userDisplayName|String|Отображаемое имя пользователя.|
|startDateTime|DateTimeOffset|Время начала вызова.|
|endDateTime|DateTimeOffset|Время окончания вызова.|
|duration|Int32|Время подключения вызова в секундах.|
|товар|Двойное с плавающей точкой|Количество денег или затрат на звонок, которые оплачиваются по вашей учетной записи.|
|callType|Строка|Указывает, был ли вызов исходящий или входящий вызов PSTN, и тип вызова, например, поступающий от пользователя или конференции с аудио-и видеосвязи.|
|евро|Строка|Тип валюты, используемой для вычисления стоимости звонка ([ISO 4217](https://en.wikipedia.org/wiki/ISO_4217)).|
|каллинумбер|Строка|Номер, набранный в формате [E. 164](https://en.wikipedia.org/wiki/E.164) .|
|усажекаунтрикоде|Строка|Код страны пользователя, [ISO 3166-1 Alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2).|
|тенанткаунтрикоде|Строка|Код страны клиента, [ISO 3166-1 Alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2).|
|коннектиончарже|Двойное с плавающей точкой|Цена оплаты по подключению.|
|каллернумбер|Строка|Номер, который получил вызов для входящих звонков или номер, набранный для исходящих звонков. Формат E. 164.|
|дестинатионконтекст|Строка|Указывает, является ли вызов внутренним (в стране или регионе) или международным (за пределами страны или региона) на основе расположения пользователя.|
|дестинатионнаме|Строка|Страна или регион набора.|
|конференцеид|Строка|Идентификатор конференции с аудио-и видеосвязи.|
|лиценсекапабилити|Строка|Лицензия, используемая для вызова.|
|инвенторитипе|Строка|Тип номера телефона пользователя, например услуга бесплатных номеров.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "ignored",
  "@odata.type": "microsoft.graph.callRecords.pstnCallLogRow",
  "baseType": "",
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
