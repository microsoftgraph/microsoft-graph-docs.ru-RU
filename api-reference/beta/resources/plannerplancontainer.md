---
title: тип ресурса plannerPlanContainer
description: Представляет контейнер для планировщикаPlan. Контейнер — это ресурс, который указывает правила авторизации и срок службы плана.
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: ea0af35bf9f82928e9da3abc90670566f3cc0869
ms.sourcegitcommit: 596b3d5636f3f3e042d180ea8f039f00ebd6b38a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/30/2021
ms.locfileid: "53665771"
---
# <a name="plannerplancontainer-resource-type"></a>тип ресурса plannerPlanContainer

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет контейнер для [планировщикаPlan](plannerPlan.md). Контейнер — это ресурс, который указывает правила авторизации и срок службы плана. Это означает, что только те, кто уполномочен работать с ресурсом, содержащим план, смогут работать с планом и задачами в нем. При удалении содержащего ресурса также удаляются содержащиеся планы. Свойства **планировщикаPlanContainer** не могут быть изменены после создания плана.

Планировщик в настоящее время поддерживает типы контейнеров, перечисленные в следующей таблице. При создании плана свойство **containerUrl** должно быть указано с помощью пути ресурса, указанного в таблице.

|Тип|Описание|Путь к ресурсу|
|----|-----------|--------------------|
|group| План содержится [группой](group.md).| https://graph.microsoft.com/beta/groups/&lt;id&gt;|
|реестр| План содержится [планировщикомRoster](plannerroster.md) | https://graph.microsoft.com/beta/planner/rosters/&lt;id&gt;|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|containerId|String|Идентификатор ресурса, который содержит план.|
|type|plannerContainerType| Тип ресурса, который содержит план. См. предыдущую таблицу поддерживаемых типов. Возможные значения: `group`, `unknownFutureValue`, `roster`. Обратите внимание, что вы должны использовать загон запроса, чтобы получить следующее значение в `Prefer: include-unknown-enum-members` этом [развиваемом переуме.](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations) `roster`|
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

