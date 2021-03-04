---
title: тип ресурса privilegedOperationEvent
description: Представляет событие аудита, которое создается привилегированным управлением удостоверениями для операций ролей, таких как администратор управляет привилегированными ролями, пользователь активирует свою роль, а пользователь отключает свою роль.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 408eb2ca06168b4e22b945aa9d3d6faa2b1a561a
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440164"
---
# <a name="privilegedoperationevent-resource-type"></a>тип ресурса privilegedOperationEvent

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет событие аудита, которое создается привилегированным управлением удостоверениями для операций ролей, таких как администратор управляет привилегированными ролями, пользователь активирует свою роль, а пользователь отключает свою роль.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Перечисление privilegedOperationEvent](../api/privilegedoperationevent-list.md) | [коллекция privilegedOperationEvent.](privilegedoperationevent.md) |Получите коллекцию объектов privilegedOperationEvent.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|additionalInformation|string|Подробные сведения о читаемом человеке для события.|
|creationDateTime|dateTimeOffset|Указывает время создания события.|
|expirationDateTime|dateTimeOffset|Это используется только тогда, когда requestType является "Активировать", и указывает время истечения срока действия активации роли.|
|id|string|Уникальный идентификатор для privilegedOperationEvent. Только для чтения.|
|referenceKey|string|Номер билета incident/Request во время активации роли. Значение представлено только в том случае, если номер билета предоставляется во время активации роли.|
|referenceSystem|string|Система билетов incident/Request, предоставляемая во время активации tole. Значение представлено только в том случае, если система билетов предоставляется во время активации роли.|
|requestType|string|Тип операции запроса. Значение requestType может быть: ```Assign``` (назначение ```Activate``` ролей), (активация роли), (удаление назначения ролей), (отключение роли), (сканирование оповещений о безопасности), (устранение проблемы оповещения о безопасности), (просмотрите обзор доступа), (создайте обзор ```Unassign``` ```Deactivate``` ```ScanAlersNow``` ```DismissAlert``` ```FixAlertItem``` ```AccessReview_Review``` ```AccessReview_Create``` доступа), ```AccessReview_Update``` (обновите ```AccessReview_Delete``` обзор доступа) и (удалите обзор доступа).|
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


