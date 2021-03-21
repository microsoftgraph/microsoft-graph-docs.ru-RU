---
title: Тип ресурса inferenceClassificationOverride
description: Представляет переопределения пользователя в том, как всегда следует классифицировать входящие сообщения от конкретного отправи-
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: abheek-das
ms.openlocfilehash: 537032c220ed98fc9052afe6a31376359836fa94
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50954999"
---
# <a name="inferenceclassificationoverride-resource-type"></a>Тип ресурса inferenceClassificationOverride

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет переопределения пользователя в том, как всегда следует классифицировать входящие сообщения от конкретного отправитель, как в [сфокусированных почтовых ящиках.](manage-focused-inbox.md)


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Обновление](../api/inferenceclassificationoverride-update.md) | [inferenceClassificationOverride](inferenceclassificationoverride.md) |Изменение поля **ClassifyAs** переопределения указанным образом. |
|[удаление](../api/inferenceclassificationoverride-delete.md); | Нет |Удаление переопределения по идентификатору. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|classifyAs|inferenceClassificationType| Указывает, как должны классифицироваться все входящие сообщения от определенного отправителя. Возможные значения: `focused`, `other`.|
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


