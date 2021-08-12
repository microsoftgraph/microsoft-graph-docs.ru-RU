---
title: Тип ресурсов plannerGroup
description: Ресурс **plannerGroup** предоставляет доступ к ресурсам Planner для группы. Он не содержит никаких полезных свойств.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: be82fb6988c88f40bc975af28240e9a99f6f9d5c13ec7069af93c3f34b92e04c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54205229"
---
# <a name="plannergroup-resource-type"></a>Тип ресурсов plannerGroup

Пространство имен: microsoft.graph

Ресурс **plannerGroup** предоставляет доступ к ресурсам Planner для [группы.](group.md) Он не содержит никаких полезных свойств.

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Список планов](../api/plannergroup-list-plans.md) |Коллекция объектов [plannerPlan](plannerplan.md)| Получите **коллекцию объектов plannerPlan.**|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|String| Только для чтения. Идентификатор **планировщикаGroup**|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|планы|Коллекция объектов [plannerPlan](plannerplan.md)| Только для чтения. Допускается значение null. Возвращает [планировщикПланы,](plannerplan.md) которые принадлежат группе.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerGroup"
}-->

```json
{
  "id": "String (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

