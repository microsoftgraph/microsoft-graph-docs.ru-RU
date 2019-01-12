---
title: Тип ресурса plannerAssignments
description: 'Назначения ресурсов plannerTask представляет **plannerAssignments** ресурс. Этот тип является открытым типом. Имя каждого свойства в этом типе '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: bf079cbf91e0c9b8b1a8c92403324b301bbde923
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27966820"
---
# <a name="plannerassignments-resource-type"></a><span data-ttu-id="ec0b9-105">Тип ресурса plannerAssignments</span><span class="sxs-lookup"><span data-stu-id="ec0b9-105">plannerAssignments resource type</span></span>

<span data-ttu-id="ec0b9-p102">Ресурс **plannerAssignments** представляет назначения ресурса [plannerTask](plannertask.md). Это открытый тип. Каждое имя свойства в этом типе представляет собой идентификатор объекта пользователя, которому назначена задача. Чтобы назначить пользователей для задачи, создайте свойства, чьи имена представляют собой идентификаторы соответствующих пользователей, при этом в качестве значения объекта [plannerassignment](plannerassignment.md) необходимо задать свойство orderHint. Чтобы отменить подобное назначение для кого-либо, присвойте свойству, имя которого представляет собой идентификатор соответствующего пользователя, значение null.</span><span class="sxs-lookup"><span data-stu-id="ec0b9-p102">The **plannerAssignments** resource represents assignments of a [plannerTask](plannertask.md) resource. This type is an open type. Each property name in this type is the ID of a user object a task is assigned to. The users can be assigned to tasks with creating new properties named with their ID, with a [plannerassignment](plannerassignment.md) object with orderHint property populated as the value. The assignees can be unassigned from the task by setting the propety named with their ID to null.</span></span>


## <a name="properties"></a><span data-ttu-id="ec0b9-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="ec0b9-111">Properties</span></span>
<span data-ttu-id="ec0b9-p103">Клиент может определять свойства открытого типа. В этом случае клиент должен предоставить идентификаторы назначенных пользователей в качестве имен свойств. Можно задать свойству объект **plannerAssignment**, чтобы создать или изменить назначенных пользователей, или значение null, чтобы удалить их.</span><span class="sxs-lookup"><span data-stu-id="ec0b9-p103">Properties of an Open Type can be defined by the client. In this case though, the client must provide assigned user's IDs as property names. The property must be set to a **plannerAssignment** object to create or modify assignees, and to null to remove them.</span></span>

<span data-ttu-id="ec0b9-115">Пример:</span><span class="sxs-lookup"><span data-stu-id="ec0b9-115">Example:</span></span>

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
<span data-ttu-id="ec0b9-p104">Этот пример кода удаляет пользователя с идентификатором ca2a1df2-e36b-4987-9f6b-0ea462f4eb47 из списка назначенных для задачи и изменяет порядок в случае пользователя с идентификатором 4e98f8f1-bb03-4015-b8e0-19bb370949d8. Если пользователю с идентификатором 4e98f8f1-bb03-4015-b8e0-19bb370949d8 задача еще не назначена, то это будет сделано при использовании данного значения в случае обновления назначений.</span><span class="sxs-lookup"><span data-stu-id="ec0b9-p104">This example removes user with ID ca2a1df2-e36b-4987-9f6b-0ea462f4eb47 from the assignees list of the task, while changing the order of the assignee with user ID 4e98f8f1-bb03-4015-b8e0-19bb370949d8. If the task isn't already assigned to user with ID 4e98f8f1-bb03-4015-b8e0-19bb370949d8, updating the assignments with this value will assign the task to this user.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerAssignments resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
