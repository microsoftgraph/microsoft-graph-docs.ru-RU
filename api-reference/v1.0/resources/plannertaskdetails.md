---
title: тип ресурса plannerTaskDetails
description: Дополнительные сведения о задаче представляет ресурс **plannerTaskDetails.** Каждый объект задачи имеет объект подробностей.
ms.localizationpriority: medium
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 54d15bdd49d7f8bc61dcc057cf77dd710ca0d8df
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59052869"
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
|description|Строка|Описание задачи.|
|id|String| Только для чтения. ID сведений о задачах. Содержит 28 знаков, учитывается регистр. [Проверка формата](planner-identifiers-disclaimer.md) проводится для службы.|
|previewType|string|Устанавливает тип предварительного просмотра задачи. Допустимые значения: `automatic`, `noPreview`, `checklist`, `description`, `reference`. При `automatic` задав показанный предварительный просмотр, приложение будет просматривать задачу.|
|references|[plannerExternalReferences](plannerexternalreferences.md)|Коллекция ссылок на задачу.|

## <a name="relationships"></a>Отношения
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

