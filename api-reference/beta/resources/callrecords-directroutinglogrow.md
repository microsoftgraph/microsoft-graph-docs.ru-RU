---
title: Тип ресурса directRoutingLogRow
description: Представляет строку данных в журнале вызовов прямой маршрутки.
author: williamlooney
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 21104f3d0812edd2af7918d6b55ff9a2f9013037
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159656"
---
# <a name="directroutinglogrow-resource-type"></a>Тип ресурса directRoutingLogRow

Пространство имен: microsoft.graph.callRecords

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет строку данных в журнале вызовов прямой маршрутки. Каждая строка сопозовна одному вызову.

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор вызова. GUID.|
|correlationId|String|Идентификатор вызова, который можно использовать при вызове службы поддержки Майкрософт. GUID.|
|userId|String|ИД вызываемого пользователя в Graph. Эти и другие сведения о пользователе будут пустыми или пустыми для типов вызовов ботов. GUID.|
|userPrincipalName|String|UserPrincipalName (имя для регистрации) в Azure Active Directory. Обычно он такой же, как SIP-адрес пользователя, и может быть таким же, как и адрес электронной почты пользователя.|
|userDisplayName|String|Отображаемое имя пользователя.|
|startDateTime|DateTimeOffset|Время начала вызова.<br/>Для неудачных и неотвеченных вызовов это может быть равно приглашению или времени сбоя.|
|inviteDateTime|DateTimeOffset| Когда было отправлено начальное приглашение.|
|failureDateTime|DateTimeOffset| Существует только для неудачных (не полностью установленных) вызовов.|
|endDateTime|DateTimeOffset| Существует только для успешных (полностью установленных) вызовов. Время окончания вызова.|
|duration|Int32| Продолжительность вызова в секундах.|
|callType|String| Тип и направление вызова.|
|successfulCall|Boolean| Успех или попытка.|
|callerNumber|String| Номер пользователя или бота, который сделал вызов. [Формат E.164,](https://en.wikipedia.org/wiki/E.164) но может включать дополнительные данные.|
|calleeNumber|String| Номер пользователя или бота, который принял вызов. [Формат E.164,](https://en.wikipedia.org/wiki/E.164) но может включать дополнительные данные.|
|mediaPathLocation|String| Центр обработки данных, используемый для пути мультимедиа при вызове без обхода.|
|signalingLocation|String| Центр обработки данных, используемый для передачи сигналов как для вызовов обхода, так и для вызовов без обхода.|
|finalSipCode|Int32| Код, с помощью которого вызов был завершен, [RFC 3261](https://tools.ietf.org/html/rfc3261).|
|callEndSubReason|Int32| Помимо кодов SIP, корпорация Майкрософт имеет собственные подкоды, которые указывают на конкретную проблему.|
|finalSipCodePhrase|String| Описание кода SIP и подкода Майкрософт.|
|trunkFullyQualifiedDomainName|String| Полное доменное имя пограничного контроллера сеанса.|
|mediaBypassEnabled|Boolean| Указывает, включена ли для магистрали обход мультимедиа.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "ignored",
  "@odata.type": "microsoft.graph.callRecords.directRoutingLogRow",
  "keyProperty": "id"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.callRecords.directRoutingLogRow",
  "id": "String (identifier)",
  "correlationId": "String",
  "userId": "String",
  "userPrincipalName": "String",
  "userDisplayName": "String",
  "startDateTime": "String (timestamp)",
  "inviteDateTime": "String (timestamp)",
  "failureDateTime": "String (timestamp)",
  "duration": "Integer",
  "callType": "String",
  "successfulCall": "Boolean",
  "callerNumber": "String",
  "calleeNumber": "String",
  "mediaPathLocation": "String",
  "signalingLocation": "String",
  "finalSipCode": "Integer",
  "callEndSubReason": "Integer",
  "finalSipCodePhrase": "String",
  "trunkFullyQualifiedDomainName": "String",
  "mediaBypassEnabled": "Boolean"
}
```


