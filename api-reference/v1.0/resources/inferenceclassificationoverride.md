---
title: Тип ресурса inferenceClassificationOverride
description: Представляет пользовательское переопределение для классификации входящих сообщений от определенного отправителя.
localization_priority: Normal
author: abheek-das
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: f9a02528f9bb781e8dd1a6f842f8d5a429160706f8fb3a3da3073358653b38cb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54160067"
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
|id|строка| Уникальный идентификатор переопределения. Только для чтения.|
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

