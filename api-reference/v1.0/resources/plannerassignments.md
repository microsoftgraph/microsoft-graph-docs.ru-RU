---
title: Тип ресурса Планнерассигнментс
description: 'Ресурс **планнерассигнментс** представляет назначения ресурса plannerTask. Этот тип является открытым типом. Имя каждого свойства в этом типе '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 1bcb28800da11255027394ea8de51e9438a5c488
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035338"
---
# <a name="plannerassignments-resource-type"></a>Тип ресурса Планнерассигнментс

Ресурс **планнерассигнментс** представляет назначения ресурса [plannerTask](plannertask.md) . Этот тип является открытым типом. Каждое имя свойства в этом типе — это идентификатор объекта пользователя, которому назначена задача. Пользователи могут быть назначены задачам, создавая новые свойства с именем ID и объект [планнерассигнмент](plannerassignment.md) со свойством ордерхинт, заполненным как значение. Уполномоченные можно отменить от задачи, задав для пропети с именем ID значение null.


## <a name="properties"></a>Свойства
Клиентская возможность может определять свойства открытого типа. В этом случае клиент должен предоставить идентификаторы назначенных пользователей в качестве имен свойств. Свойству необходимо присвоить значение объекта **планнерассигнмент** , чтобы создать или изменить уполномоченные, и значение null, чтобы удалить их.

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
В этом примере показано, как удалить пользователя с ИДЕНТИФИКАТОРом ca2a1df2-e36b-4987-9f6b-0ea462f4eb47 из списка уполномоченные задачи, изменив порядок поручения ИДЕНТИФИКАТОРом пользователя 4e98f8f1-bb03-4015-b8e0-19bb370949d8. Если задача еще не назначена пользователю с ИДЕНТИФИКАТОРом 4e98f8f1-bb03-4015-b8e0-19bb370949d8, то при обновлении назначений с этим значением задача будет назначена этому пользователю.

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerAssignments resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
