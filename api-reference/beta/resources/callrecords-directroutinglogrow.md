---
title: Тип ресурса Директраутинглогров
description: Представляет строку данных в журнале вызовов прямой маршрутизации.
author: williamlooney
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: c5baf5768c7cee9e0525373bb4f7139f6a145acb
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48601204"
---
# <a name="directroutinglogrow-resource-type"></a>Тип ресурса Директраутинглогров

Пространство имен: microsoft.graph.callRecords

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет строку данных в журнале вызовов прямой маршрутизации. Каждая строка соответствует одному вызову.

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор звонка. Кодом.|
|correlationId|String|Идентификатор вызова, который можно использовать при вызове службы поддержки Майкрософт. Кодом.|
|userId|String|Идентификатор вызывающего пользователя в Graph. Эта и другие сведения о пользователе будут иметь значение null или Empty для типов вызовов Bot. Кодом.|
|userPrincipalName|String|UserPrincipalName (имя входа) в Azure Active Directory. Обычно это тот же адрес SIP, что и адрес электронной почты пользователя.|
|userDisplayName|String|Отображаемое имя пользователя.|
|startDateTime|DateTimeOffset|Время начала вызова.<br/>Для неудачных и неотвеченных вызовов это значение может быть равно приглашению или времени сбоя.|
|инвитедатетиме|DateTimeOffset| При отправке первого приглашения.|
|фаилуредатетиме|DateTimeOffset| Существует только для вызовов с ошибками (не полностью установленными).|
|endDateTime|DateTimeOffset| Существует только для успешных (полностью установленных) вызовов. Время окончания звонка.|
|duration|Int32| Продолжительность звонка в секундах.|
|callType|String| Тип и направление звонка.|
|сукцессфулкалл|Boolean| Успех или попытка.|
|каллернумбер|String| Номер пользователя или ленты, выполнившего звонок. Формат [E. 164](https://en.wikipedia.org/wiki/E.164) , но может содержать дополнительные данные.|
|каллинумбер|String| Номер пользователя или робота, который получил звонок. Формат [E. 164](https://en.wikipedia.org/wiki/E.164) , но может содержать дополнительные данные.|
|медиапаслокатион|String| Центр обработки данных, используемый для пути к носителю при вызове без обхода.|
|сигналинглокатион|String| Центр обработки данных, используемый для передачи сигналов как для обхода, так и для вызовов без обхода.|
|финалсипкоде|Int32| Код, с которым закончился вызов, [RFC 3261](https://tools.ietf.org/html/rfc3261).|
|каллендсубреасон|Int32| Помимо SIP кодов, у корпорации Майкрософт есть подкода, указывающие на конкретную ошибку.|
|финалсипкодефрасе|String| Описание кода SIP и подкода корпорации Майкрософт.|
|трункфулликуалифиеддомаиннаме|String| Полное доменное имя пограничного контроллера сеансов.|
|медиабипассенаблед|Boolean| Указывает, включена ли магистраль для обхода сервера мультимедиа.|

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


