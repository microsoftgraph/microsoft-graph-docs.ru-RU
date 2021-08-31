---
title: тип ресурса directRoutingLogRow
description: Представляет строку данных в журнале вызовов прямой маршрутики.
author: williamlooney
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: a1260d3f1406807930e696a1d7adbd6db21392b6
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58788249"
---
# <a name="directroutinglogrow-resource-type"></a>тип ресурса directRoutingLogRow

Пространство имен: microsoft.graph.callRecords

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет строку данных в журнале вызовов прямой маршрутики. Каждая строка сопомна одному вызову.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [getDirectRoutingCalls](../api/callrecords-callrecord-getdirectroutingcalls.md) | [коллекция microsoft.graph.callRecords.directRoutingLogRow](callrecords-directroutinglogrow.md)| Список **объектов directRoutingLogRow** для записи вызовов. |

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|callEndSubReason|Int32| Помимо кодов SIP Корпорация Майкрософт имеет собственные подкоды, которые указывают на конкретную проблему.|
|callType|Строка| Тип и направление вызова.|
|calleeNumber|Строка| Номер пользователя или бота, который получил вызов. [Формат E.164,](https://en.wikipedia.org/wiki/E.164) но может включать дополнительные данные.|
|callerNumber|Строка| Номер пользователя или бота, который сделал вызов. [Формат E.164,](https://en.wikipedia.org/wiki/E.164) но может включать дополнительные данные.|
|correlationId|String|Идентификатор для вызова, который можно использовать при вызове службы поддержки Майкрософт. GUID.|
|duration|Int32| Длительность вызова в секундах.|
|endDateTime|DateTimeOffset| Существует только для успешных (полностью установленных) вызовов. Время окончания вызова.|
|failureDateTime|DateTimeOffset| Существует только для неудавшихся (не полностью установленных) вызовов.|
|finalSipCodePhrase|Строка| Описание кода SIP и подкода Майкрософт.|
|finalSipCode|Int32| Код, с которым завершился вызов, [RFC 3261](https://tools.ietf.org/html/rfc3261).|
|id|Строка|Уникальный идентификатор вызовов. GUID.|
|inviteDateTime|DateTimeOffset| Когда было отправлено начальное приглашение.|
|mediaBypassEnabled|Логический| Указывает, включен ли магистраль для обхода мультимедиа или нет.|
|mediaPathLocation|Строка| Центр обработки данных, используемый для пути мультимедиа при вызове без обхода.|
|signalingLocation|Строка| Центр обработки данных, используемый для сигнализации как для обходных, так и для обходных вызовов.|
|startDateTime|DateTimeOffset|Время начала вызова.<br/>Для неудавшиеся и неотвеченные вызовы это может быть равно времени приглашения или отказа.|
|successfulCall|Логический| Успех или попытка.|
|trunkFullyQualifiedDomainName|Строка| Полное доменное имя пограничного контроллера сеанса.|
|userDisplayName|String|Отображаемое имя пользователя.|
|userId|String|Вызов ID пользователя в Graph. Эта и другая информация пользователя будет null/empty для типов вызовов ботов. GUID.|
|userPrincipalName|String|UserPrincipalName (имя регистрации) в Azure Active Directory. Это обычно то же самое, что и SIP-адрес пользователя, и может быть таким же, как и адрес электронной почты пользователя.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
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
  "endDateTime": "String (timestamp)",
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


