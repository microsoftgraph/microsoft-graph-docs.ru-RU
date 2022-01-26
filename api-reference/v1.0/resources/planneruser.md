---
title: Тип ресурса plannerUser
description: Ресурс **plannerUser предоставляет** пользователю доступ к ресурсам Planner. Он не содержит никаких полезных свойств.
ms.localizationpriority: medium
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 1c921b11c54075a8ff844f7ef932cc9c34172b44
ms.sourcegitcommit: 871db8b3f68489d24e2aeafe694725579ee44c47
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2022
ms.locfileid: "62225212"
---
# <a name="planneruser-resource-type"></a>Тип ресурса plannerUser

Пространство имен: microsoft.graph

Ресурс **plannerUser предоставляет** доступ к ресурсам Planner для [пользователя.](user.md) Он не содержит никаких полезных свойств.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Список планов](../api/planneruser-list-plans.md) |Коллекция объектов [plannerPlan](plannerplan.md)| Получите **коллекцию объектов plannerPlan.**|
|[Перечисление задач](../api/planneruser-list-tasks.md) |Коллекция объектов [plannerTask](plannertask.md)| Получение коллекции объектов **plannerTask**.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|String| Только для чтения. Идентификатор plannerUser|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|планы|Коллекция объектов [plannerPlan](plannerplan.md)| Только для чтения. Допускается значение null. Возвращает [планировщикTasks,](plannertask.md) назначенного пользователю.|
|tasks|Коллекция объектов [plannerTask](plannertask.md)| Только для чтения. Допускается значение null. Возвращает [планировщикПланы, общие](plannerplan.md) пользователю.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerUser"
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
  "description": "plannerUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

