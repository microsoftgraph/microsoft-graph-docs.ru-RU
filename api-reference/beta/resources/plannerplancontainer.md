---
title: Тип ресурса plannerPlanContainer
description: Представляет контейнер для plannerPlan. Контейнер — это ресурс, который определяет правила авторизации и срок действия плана.
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 8b3abb10892077159e6f02c33a31d501a75dba2a
ms.sourcegitcommit: 1d2adc4062c8e83d23768682cf66a731bccd313c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/16/2021
ms.locfileid: "49883255"
---
# <a name="plannerplancontainer-resource-type"></a>Тип ресурса plannerPlanContainer

Пространство имен: microsoft.graph

Представляет контейнер для [plannerPlan.](plannerPlan.md) Контейнер — это ресурс, который определяет правила авторизации и срок действия плана. Это означает, что только люди, которым разрешено работать с ресурсом, содержащим план, смогут работать с планом и задачами в нем. При удалении содержащегося ресурса также удаляются содержащиеся планы. Свойства **объекта plannerPlanContainer** нельзя изменить после создания плана.

Планировщик в настоящее время поддерживает типы контейнеров, перечисленные в следующей таблице. При создании плана свойство **containerUrl** должно быть указано с помощью пути к ресурсу, указанному в таблице.

|Тип|Описание|Путь к ресурсу|
|----|-----------|--------------------|
|group| План содержится в группе.| https://graph.microsoft.com/v1.0/groups/&lt;id&gt;|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|containerId|Строка|Идентификатор ресурса, который содержит план.|
|type|plannerContainerType| Тип ресурса, который содержит план. Поддерживаемые типы см. в предыдущей таблице. Возможные значения: `group`, `unknownFutureValue`.|
|url|String|Полный канонический URL-адрес контейнера.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.plannerPlanContainer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.plannerPlanContainer",
  "url": "String",
  "containerId": "String",
  "type": "String"
}
```

