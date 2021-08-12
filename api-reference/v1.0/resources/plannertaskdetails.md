---
title: тип ресурса plannerTaskDetails
description: Дополнительные сведения о задаче представляет ресурс **plannerTaskDetails.** Каждый объект задачи имеет объект подробностей.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 852deda3e48c78b2e70968cb7e8b7ec9a11956bbf2fcab66ecc127ea653abce9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54189396"
---
# <a name="plannertaskdetails-resource-type"></a>тип ресурса plannerTaskDetails

Пространство имен: microsoft.graph

Дополнительные сведения о задаче представляет ресурс **plannerTaskDetails.** Каждый [объект](plannertask.md) задачи имеет объект подробностей.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта plannerTaskDetails](../api/plannertaskdetails-get.md) | [plannerTaskDetails](plannertaskdetails.md); |Чтение свойств и связей **объекта plannerTaskDetails.**|
|[Обновление](../api/plannertaskdetails-update.md) | [plannerTaskDetails](plannertaskdetails.md);    |Объект **Update plannerTaskDetails.** |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|checklist|[plannerChecklistItems](plannerchecklistitems.md)|Коллекция элементов контрольного списка задачи.|
|description|String|Описание задачи.|
|id|String| Только для чтения. ID сведений о задачах. Содержит 28 знаков, учитывается регистр. [Проверка формата](planner-identifiers-disclaimer.md) проводится для службы.|
|previewType|string|Устанавливает тип предварительного просмотра задачи. Допустимые значения: `automatic`, `noPreview`, `checklist`, `description`, `reference`. При `automatic` задав показанный предварительный просмотр, приложение будет просматривать задачу.|
|references|[plannerExternalReferences](plannerexternalreferences.md)|Коллекция ссылок на задачу.|

## <a name="relationships"></a>Связи
Нет


## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.plannerTaskDetails"
}-->

```json
{
  "checklist": {"@odata.type": "microsoft.graph.plannerChecklistItems"},
  "description": "String",
  "id": "String (identifier)",
  "previewType": "string",
  "references": {"@odata.type": "microsoft.graph.plannerExternalReferences"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerTaskDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

