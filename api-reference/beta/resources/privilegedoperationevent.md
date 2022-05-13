---
title: Тип ресурса privilegedOperationEvent
description: Представляет событие аудита, созданное управление привилегированными пользователями для операций роли, например администратор управляет привилегированными ролями, пользователь активирует свою роль, а пользователь деактивирует свою роль.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: rkarim-ms
ms.openlocfilehash: 0002e10cff2324d60f9000b1cdf961b865409056
ms.sourcegitcommit: d7efd03a6782da5e44b422c9016869c779d64add
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2022
ms.locfileid: "65397546"
---
# <a name="privilegedoperationevent-resource-type-deprecated"></a>Тип ресурса privilegedOperationEvent (не рекомендуется)

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [pim-v2AADRoles-deprecation](../../includes/pim-v2AADRoles-deprecation.md)]

Представляет событие аудита, созданное управление привилегированными пользователями для операций роли, например администратор управляет привилегированными ролями, пользователь активирует свою роль, а пользователь деактивирует свою роль.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Перечисление privilegedOperationEvent](../api/privilegedoperationevent-list.md) | [коллекция privilegedOperationEvent](privilegedoperationevent.md) . |Получение коллекции объектов privilegedOperationEvent.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|additionalInformation|string|Подробные удобочитаемые сведения о событии.|
|creationDateTime|DateTimeOffset|Указывает время создания события.|
|expirationDateTime|DateTimeOffset|Он используется только в том случае, если **параметр requestType** `Activate`имеет значение и указывает время окончания срока действия активации роли.|
|id|string|Уникальный идентификатор для privilegedOperationEvent. Только для чтения.|
|referenceKey|string|Номер билета инцидента или запроса во время активации роли. Значение предоставляется только в том случае, если номер билета указан во время активации роли.|
|referenceSystem|string|Система запросов и инцидентов, предоставляемая во время активации tole. Значение предоставляется только в том случае, если система запросов предоставляется во время активации роли.|
|requestType|String|Тип операции запроса. Значение requestType может быть следующим: `Assign` (назначение роли), `Activate` (активация роли), `Unassign` (удаление назначения роли), `ScanAlertsNow` `Deactivate` (проверка оповещений системы безопасности), `DismissAlert` (отклонение оповещения системы безопасности), `FixAlertItem` (исправление проблемы с оповещением системы безопасности), `AccessReview_Review` (просмотрите проверку доступа), `AccessReview_Create` (создайте проверку доступа) и `AccessReview_Update` (обновите проверку доступа) `AccessReview_Delete` (удалите проверку доступа).|
|requestorId|string|Идентификатор пользователя инициатора запроса, который инициирует операцию.|
|requestorName|string|Имя пользователя инициатора запроса, который инициирует операцию.|
|roleId|string|Идентификатор роли, связанной с операцией.|
|roleName|string|Имя роли.|
|tenantId|string|Идентификатор клиента (организации).|
|userId|строка|Идентификатор пользователя, связанного с операцией.|
|userMail|string|Сообщение электронной почты пользователя.|
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


