---
title: Тип ресурса inferenceClassificationOverride
description: Представляет пользовательское переопределение для классификации входящих сообщений от определенного отправителя.
localization_priority: Normal
author: abheek-das
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 07bd56a197daa97f2c45baf62531ff53dee0bb1a
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137538"
---
# <a name="inferenceclassificationoverride-resource-type"></a>Тип ресурса inferenceClassificationOverride

Пространство имен: microsoft.graph

Представляет пользовательское переопределение для классификации входящих сообщений от определенного отправителя.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Обновление](../api/inferenceclassificationoverride-update.md) | [inferenceClassificationOverride](inferenceclassificationoverride.md) |Изменение поля **ClassifyAs** переопределения указанным образом. |
|[Удаление](../api/inferenceclassificationoverride-delete.md) | Нет |Удаление переопределения по идентификатору. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|classifyAs|inferenceClassificationType| Указывает, как должны классифицироваться все входящие сообщения от определенного отправителя. Возможные значения: `focused` , `other` .|
|id|string| Уникальный идентификатор переопределения. Только для чтения.|
|senderEmailAddress|[emailAddress](emailaddress.md)|Сведения об электронном адресе отправителя, для которого создано переопределение.|

## <a name="relationships"></a>Связи
Нет


## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
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
<!-- {
  "type": "#page.annotation",
  "description": "inferenceClassificationOverride resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

