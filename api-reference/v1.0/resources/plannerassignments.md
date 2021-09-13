---
title: Тип ресурса plannerAssignments
description: 'Ресурс **plannerAssignments** представляет назначения ресурса plannerTask. Этот тип — открытый тип. Каждое имя свойства в этом типе '
ms.localizationpriority: medium
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: c6c90a607622dc47f7fd3a3d77b7b42b2c39b6e5
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59044344"
---
# <a name="plannerassignments-resource-type"></a>Тип ресурса plannerAssignments

Пространство имен: microsoft.graph

Ресурс **plannerAssignments** представляет назначения ресурса [plannerTask.](plannertask.md) Этот тип — открытый тип. Каждое имя свойства в этом типе — это ID объекта пользователя, на который назначена задача. Пользователям могут быть назначены задачи с созданием новых свойств с именем их ID с объектом [plannerassignment](plannerassignment.md) с свойством orderHint, населенным в качестве значения. Назначение может быть не назначено из задачи, установив пропеть с именем их ID в null.


## <a name="properties"></a>Свойства
Свойства открытого типа могут быть определены клиентом. Однако в этом случае клиент должен предоставить задамые им имена пользователей в качестве имен свойств. Свойство должно быть задавано **объекту plannerAssignment** для создания или изменения назначений, а также для удаления их.

Пример.

<!-- {
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [ "ca2a1df2-e36b-4987-9f6b-0ea462f4eb47", "4e98f8f1-bb03-4015-b8e0-19bb370949d8" ],
  "@odata.type": "microsoft.graph.plannerAssignments"
}-->
```json
{
  "ca2a1df2-e36b-4987-9f6b-0ea462f4eb47": null,
  "4e98f8f1-bb03-4015-b8e0-19bb370949d8": { 
      "@odata.type": "microsoft.graph.plannerAssignment",
      "orderHint": "String"
    }
}
```
В этом примере пользователь с ID ca2a1df2-e36b-4987-9f6b-0ea462f4eb47 удаляется из списка назначающих задач, меняя порядок назначения на пользовательский ID 4e98f8f1-bb03-4015-b8e0-19bb370949d8. Если задача еще не назначена пользователю с ID 4e98f8f1-bb03-4015-b8e0-19bb370949d8, обновление назначений с этим значением назначит задачу этому пользователю.

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerAssignments resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

