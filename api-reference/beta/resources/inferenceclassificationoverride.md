---
title: Тип ресурса inferenceClassificationOverride
description: Представляет переопределение пользователя, определяющее, как должны классифицироваться входящие сообщения от определенного отправителя
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 944d9784e43ff5c1277c526a6b9fe3115487ac8d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42496210"
---
# <a name="inferenceclassificationoverride-resource-type"></a>Тип ресурса inferenceClassificationOverride

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет переопределение пользователя, которое всегда должно классифицироваться как входящие сообщения от определенного отправителя, как в [папке "отсортированные"](manage-focused-inbox.md).


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Обновление](../api/inferenceclassificationoverride-update.md) | [inferenceClassificationOverride](inferenceclassificationoverride.md) |Изменение поля **ClassifyAs** переопределения указанным образом. |
|[удаление](../api/inferenceclassificationoverride-delete.md); | Нет |Удаление переопределения по идентификатору. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|classifyAs|string| Указывает, как должны классифицироваться все входящие сообщения от определенного отправителя. Возможные значения: `focused`, `other`.|
|id|string| Уникальный идентификатор переопределения. Только для чтения.|
|senderEmailAddress|[emailAddress](emailaddress.md)|Сведения об электронном адресе отправителя, для которого создано переопределение.|

## <a name="relationships"></a>Связи
Нет


## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.inferenceClassificationOverride"
}-->

```json
{
  "classifyAs": "string",
  "id": "string (identifier)",
  "senderEmailAddress": {"@odata.type": "microsoft.graph.emailAddress"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "inferenceClassificationOverride resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
