---
title: Тип ресурса Планнерассигнментс
description: 'Ресурс **планнерассигнментс** представляет назначения ресурса plannerTask. Этот тип является открытым типом. Имя каждого свойства в этом типе '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 915064d1c697f05c66dfefbbda39a6d31d7d8b47
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42534024"
---
# <a name="plannerassignments-resource-type"></a><span data-ttu-id="ef3d7-105">Тип ресурса Планнерассигнментс</span><span class="sxs-lookup"><span data-stu-id="ef3d7-105">plannerAssignments resource type</span></span>

<span data-ttu-id="ef3d7-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ef3d7-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ef3d7-107">Ресурс **планнерассигнментс** представляет назначения ресурса [plannerTask](plannertask.md) .</span><span class="sxs-lookup"><span data-stu-id="ef3d7-107">The **plannerAssignments** resource represents assignments of a [plannerTask](plannertask.md) resource.</span></span> <span data-ttu-id="ef3d7-108">Этот тип является открытым типом.</span><span class="sxs-lookup"><span data-stu-id="ef3d7-108">This type is an open type.</span></span> <span data-ttu-id="ef3d7-109">Каждое имя свойства в этом типе — это идентификатор объекта пользователя, которому назначена задача.</span><span class="sxs-lookup"><span data-stu-id="ef3d7-109">Each property name in this type is the ID of a user object a task is assigned to.</span></span> <span data-ttu-id="ef3d7-110">Пользователи могут быть назначены задачам, создавая новые свойства с именем ID и объект [планнерассигнмент](plannerassignment.md) со свойством ордерхинт, заполненным как значение.</span><span class="sxs-lookup"><span data-stu-id="ef3d7-110">The users can be assigned to tasks with creating new properties named with their ID, with a [plannerassignment](plannerassignment.md) object with orderHint property populated as the value.</span></span> <span data-ttu-id="ef3d7-111">Уполномоченные можно отменить от задачи, задав для пропети с именем ID значение null.</span><span class="sxs-lookup"><span data-stu-id="ef3d7-111">The assignees can be unassigned from the task by setting the propety named with their ID to null.</span></span>


## <a name="properties"></a><span data-ttu-id="ef3d7-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="ef3d7-112">Properties</span></span>
<span data-ttu-id="ef3d7-113">Клиентская возможность может определять свойства открытого типа.</span><span class="sxs-lookup"><span data-stu-id="ef3d7-113">Properties of an Open Type can be defined by the client.</span></span> <span data-ttu-id="ef3d7-114">В этом случае клиент должен предоставить идентификаторы назначенных пользователей в качестве имен свойств.</span><span class="sxs-lookup"><span data-stu-id="ef3d7-114">In this case though, the client must provide assigned user's IDs as property names.</span></span> <span data-ttu-id="ef3d7-115">Свойству необходимо присвоить значение объекта **планнерассигнмент** , чтобы создать или изменить уполномоченные, и значение null, чтобы удалить их.</span><span class="sxs-lookup"><span data-stu-id="ef3d7-115">The property must be set to a **plannerAssignment** object to create or modify assignees, and to null to remove them.</span></span>

<span data-ttu-id="ef3d7-116">Пример:</span><span class="sxs-lookup"><span data-stu-id="ef3d7-116">Example:</span></span>

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
<span data-ttu-id="ef3d7-117">В этом примере показано, как удалить пользователя с ИДЕНТИФИКАТОРом ca2a1df2-e36b-4987-9f6b-0ea462f4eb47 из списка уполномоченные задачи, изменив порядок поручения ИДЕНТИФИКАТОРом пользователя 4e98f8f1-bb03-4015-b8e0-19bb370949d8.</span><span class="sxs-lookup"><span data-stu-id="ef3d7-117">This example removes user with ID ca2a1df2-e36b-4987-9f6b-0ea462f4eb47 from the assignees list of the task, while changing the order of the assignee with user ID 4e98f8f1-bb03-4015-b8e0-19bb370949d8.</span></span> <span data-ttu-id="ef3d7-118">Если задача еще не назначена пользователю с ИДЕНТИФИКАТОРом 4e98f8f1-bb03-4015-b8e0-19bb370949d8, то при обновлении назначений с этим значением задача будет назначена этому пользователю.</span><span class="sxs-lookup"><span data-stu-id="ef3d7-118">If the task isn't already assigned to user with ID 4e98f8f1-bb03-4015-b8e0-19bb370949d8, updating the assignments with this value will assign the task to this user.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerAssignments resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
