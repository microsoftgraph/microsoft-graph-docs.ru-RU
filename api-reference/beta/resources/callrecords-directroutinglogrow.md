---
title: Тип ресурса Директраутинглогров
description: Представляет строку данных в журнале вызовов прямой маршрутизации.
author: stephenjust
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 3a01ed8410532264fceb0164ef4f703b636ccdef
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/29/2020
ms.locfileid: "46510396"
---
# <a name="directroutinglogrow-resource-type"></a>Тип ресурса Директраутинглогров

Пространство имен: microsoft.graph.callRecords

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет строку данных в журнале вызовов прямой маршрутизации. Каждая строка соответствует одному вызову.

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор звонка. Кодом.|
|correlationId|String|Идентификатор вызова, который можно использовать при вызове службы поддержки Майкрософт. Кодом.|
|userId|String|Идентификатор вызывающего пользователя в Graph. Эта и другие сведения о пользователе будут иметь значение null или Empty для типов вызовов Bot. Кодом.|
|userPrincipalName|Строка|UserPrincipalName (имя входа) в Azure Active Directory. Обычно это тот же адрес SIP, что и адрес электронной почты пользователя.|
|userDisplayName|Строка|Отображаемое имя пользователя.|
|startDateTime|DateTimeOffset|Время начала вызова.<br/>Для неудачных и неотвеченных вызовов это значение может быть равно приглашению или времени сбоя.|
|инвитедатетиме|DateTimeOffset| При отправке первого приглашения.|
|фаилуредатетиме|DateTimeOffset| Существует только для вызовов с ошибками (не полностью установленными).|
|endDateTime|DateTimeOffset| Существует только для успешных (полностью установленных) вызовов. Время окончания звонка.|
|duration|Int32| Продолжительность звонка в секундах.|
|callType|Строка| Тип и направление звонка.|
|сукцессфулкалл|Логический| Успех или попытка.|
|каллернумбер|Строка| Номер пользователя или ленты, выполнившего звонок. Формат [E. 164](https://en.wikipedia.org/wiki/E.164) , но может содержать дополнительные данные.|
|каллинумбер|Строка| Номер пользователя или робота, который получил звонок. Формат [E. 164](https://en.wikipedia.org/wiki/E.164) , но может содержать дополнительные данные.|
|медиапаслокатион|Строка| Центр обработки данных, используемый для пути к носителю при вызове без обхода.|
|сигналинглокатион|Строка| Центр обработки данных, используемый для передачи сигналов как для обхода, так и для вызовов без обхода.|
|финалсипкоде|Int32| Код, с которым закончился вызов, [RFC 3261](https://tools.ietf.org/html/rfc3261).|
|каллендсубреасон|Int32| Помимо SIP кодов, у корпорации Майкрософт есть подкода, указывающие на конкретную ошибку.|
|финалсипкодефрасе|Строка| Описание кода SIP и подкода корпорации Майкрософт.|
|трункфулликуалифиеддомаиннаме|Строка| Полное доменное имя пограничного контроллера сеансов.|
|медиабипассенаблед|Логический| Указывает, включена ли магистраль для обхода сервера мультимедиа.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "ignored",
  "@odata.type": "microsoft.graph.callRecords.directRoutingLogRow",
  "baseType": "",
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
