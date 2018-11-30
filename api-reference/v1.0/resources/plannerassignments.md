---
title: Тип ресурса plannerAssignments
description: 'Назначения ресурсов plannerTask представляет **plannerAssignments** ресурс. Этот тип является открытым типом. Имя каждого свойства в этом типе '
ms.openlocfilehash: 1cb080ff8d66c2319b77dd560f10422e1663a46d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27028209"
---
# <a name="plannerassignments-resource-type"></a>Тип ресурса plannerAssignments

Ресурс **plannerAssignments** представляет назначения ресурса [plannerTask](plannertask.md). Это открытый тип. Каждое имя свойства в этом типе представляет собой идентификатор объекта пользователя, которому назначена задача. Чтобы назначить пользователей для задачи, создайте свойства, чьи имена представляют собой идентификаторы соответствующих пользователей, при этом в качестве значения объекта [plannerassignment](plannerassignment.md) необходимо задать свойство orderHint. Чтобы отменить подобное назначение для кого-либо, присвойте свойству, имя которого представляет собой идентификатор соответствующего пользователя, значение null.


## <a name="properties"></a>Свойства
Клиент может определять свойства открытого типа. В этом случае клиент должен предоставить идентификаторы назначенных пользователей в качестве имен свойств. Можно задать свойству объект **plannerAssignment**, чтобы создать или изменить назначенных пользователей, или значение null, чтобы удалить их.

Пример:

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
Этот пример кода удаляет пользователя с идентификатором ca2a1df2-e36b-4987-9f6b-0ea462f4eb47 из списка назначенных для задачи и изменяет порядок в случае пользователя с идентификатором 4e98f8f1-bb03-4015-b8e0-19bb370949d8. Если пользователю с идентификатором 4e98f8f1-bb03-4015-b8e0-19bb370949d8 задача еще не назначена, то это будет сделано при использовании данного значения в случае обновления назначений.

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerAssignments resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->