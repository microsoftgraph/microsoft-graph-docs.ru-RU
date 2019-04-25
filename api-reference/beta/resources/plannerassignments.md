---
title: Тип ресурса Планнерассигнментс
description: 'Ресурс **планнерассигнментс** представляет назначения ресурса plannerTask. Этот тип является открытым типом. Имя каждого свойства в этом типе '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 2c379c786e3b94395aa3de7bc382e184db0fcc24
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32541369"
---
# <a name="plannerassignments-resource-type"></a><span data-ttu-id="c4b70-105">Тип ресурса Планнерассигнментс</span><span class="sxs-lookup"><span data-stu-id="c4b70-105">plannerAssignments resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c4b70-106">Ресурс **планнерассигнментс** представляет назначения ресурса [plannerTask](plannertask.md) .</span><span class="sxs-lookup"><span data-stu-id="c4b70-106">The **plannerAssignments** resource represents assignments of a [plannerTask](plannertask.md) resource.</span></span> <span data-ttu-id="c4b70-107">Этот тип является открытым типом.</span><span class="sxs-lookup"><span data-stu-id="c4b70-107">This type is an open type.</span></span> <span data-ttu-id="c4b70-108">Каждое имя свойства в этом типе — это идентификатор объекта пользователя, которому назначена задача.</span><span class="sxs-lookup"><span data-stu-id="c4b70-108">Each property name in this type is the ID of a user object a task is assigned to.</span></span> <span data-ttu-id="c4b70-109">Пользователи могут быть назначены задачам, создавая новые свойства с именем ID и объект [планнерассигнмент](plannerassignment.md) со свойством ордерхинт, заполненным как значение.</span><span class="sxs-lookup"><span data-stu-id="c4b70-109">The users can be assigned to tasks with creating new properties named with their ID, with a [plannerassignment](plannerassignment.md) object with orderHint property populated as the value.</span></span> <span data-ttu-id="c4b70-110">Уполномоченные можно отменить от задачи, задав для пропети с именем ID значение null.</span><span class="sxs-lookup"><span data-stu-id="c4b70-110">The assignees can be unassigned from the task by setting the propety named with their ID to null.</span></span>


## <a name="properties"></a><span data-ttu-id="c4b70-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="c4b70-111">Properties</span></span>
<span data-ttu-id="c4b70-112">Клиентская возможность может определять свойства открытого типа.</span><span class="sxs-lookup"><span data-stu-id="c4b70-112">Properties of an Open Type can be defined by the client.</span></span> <span data-ttu-id="c4b70-113">В этом случае клиент должен предоставить идентификаторы назначенных пользователей в качестве имен свойств.</span><span class="sxs-lookup"><span data-stu-id="c4b70-113">In this case though, the client must provide assigned user's IDs as property names.</span></span> <span data-ttu-id="c4b70-114">Свойству необходимо присвоить значение объекта **планнерассигнмент** , чтобы создать или изменить уполномоченные, и значение null, чтобы удалить их.</span><span class="sxs-lookup"><span data-stu-id="c4b70-114">The property must be set to a **plannerAssignment** object to create or modify assignees, and to null to remove them.</span></span>

<span data-ttu-id="c4b70-115">Пример.</span><span class="sxs-lookup"><span data-stu-id="c4b70-115">Example:</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
<span data-ttu-id="c4b70-116">В этом примере показано, как удалить пользователя с ИДЕНТИФИКАТОРом ca2a1df2-e36b-4987-9f6b-0ea462f4eb47 из списка уполномоченные задачи, изменив порядок поручения ИДЕНТИФИКАТОРом пользователя 4e98f8f1-bb03-4015-b8e0-19bb370949d8.</span><span class="sxs-lookup"><span data-stu-id="c4b70-116">This example removes user with ID ca2a1df2-e36b-4987-9f6b-0ea462f4eb47 from the assignees list of the task, while changing the order of the assignee with user ID 4e98f8f1-bb03-4015-b8e0-19bb370949d8.</span></span> <span data-ttu-id="c4b70-117">Если задача еще не назначена пользователю с ИДЕНТИФИКАТОРом 4e98f8f1-bb03-4015-b8e0-19bb370949d8, то при обновлении назначений с этим значением задача будет назначена этому пользователю.</span><span class="sxs-lookup"><span data-stu-id="c4b70-117">If the task isn't already assigned to user with ID 4e98f8f1-bb03-4015-b8e0-19bb370949d8, updating the assignments with this value will assign the task to this user.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerAssignments resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerassignments.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
