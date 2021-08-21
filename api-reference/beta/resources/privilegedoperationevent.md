---
title: тип ресурса privilegedOperationEvent
description: Представляет событие аудита, которое создается управление привилегированными пользователями для операций ролей, например администратор управляет привилегированными ролями, пользователь активирует свою роль, а пользователь отключает свою роль.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu1
ms.openlocfilehash: af317a8fa1257b9ba9e6bb4c80dc4291337b4d8c
ms.sourcegitcommit: 01755ac7c0ab7becf28052e05e58567caa8364cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/21/2021
ms.locfileid: "58454096"
---
# <a name="privilegedoperationevent-resource-type"></a>тип ресурса privilegedOperationEvent

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет событие аудита, которое создается управление привилегированными пользователями для операций ролей, например администратор управляет привилегированными ролями, пользователь активирует свою роль, а пользователь отключает свою роль.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Перечисление privilegedOperationEvent](../api/privilegedoperationevent-list.md) | [коллекция privilegedOperationEvent.](privilegedoperationevent.md) |Получите коллекцию объектов privilegedOperationEvent.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|additionalInformation|string|Подробные сведения о читаемом человеке для события.|
|creationDateTime|DateTimeOffset|Указывает время создания события.|
|expirationDateTime|DateTimeOffset|Это используется только тогда, когда **requestType** — и указывает время истечения срока действия `Activate` активации роли.|
|id|string|Уникальный идентификатор для privilegedOperationEvent. Только для чтения.|
|referenceKey|string|Номер билета incident/Request во время активации роли. Значение представлено только в том случае, если номер билета предоставляется во время активации роли.|
|referenceSystem|string|Система билетов incident/Request, предоставляемая во время активации tole. Значение представлено только в том случае, если система билетов предоставляется во время активации роли.|
|requestType|String|Тип операции запроса. Значение requestType может быть: `Assign` (назначение ролей), (активация роли), (удаление назначения ролей), (отключение роли), (сканирование оповещений о безопасности), (устранение проблемы оповещения о безопасности), (просмотрите обзор доступа), (создайте обзор доступа) (обновите обзор `Activate` `Unassign` `Deactivate` `ScanAlertsNow` `DismissAlert` `FixAlertItem`  `AccessReview_Review` `AccessReview_Create` `AccessReview_Update` доступа), `AccessReview_Delete` (удалите обзор доступа).|
|requestorId|string|Пользовательский id запросителя, который инициирует операцию.|
|requestorName|string|Имя пользователя запросителя, который инициирует операцию.|
|roleId|string|ID роли, связанной с операцией.|
|имя roleName|string|Имя роли.|
|tenantId|string|ID клиента (организации).|
|userId|строка|ID пользователя, связанного с операцией.|
|userMail|string|Электронная почта пользователя.|
|userName|string|Отображаемое имя пользователя.|

## <a name="relationships"></a>Связи
Нет


## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.privilegedOperationEvent"
}-->

```json
{
  "additionalInformation": "string",
  "creationDateTime": "String (timestamp)",
  "expirationDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "requestType": "string",
  "requestorId": "string",
  "requestorName": "string",
  "roleId": "string",
  "roleName": "string",
  "tenantId": "string",
  "userId": "string",
  "userMail": "string",
  "userName": "string",
  "referenceKey": "string",
  "referenceSystem": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedOperationEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


