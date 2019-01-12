---
title: Тип ресурса educationAssignmentResource
description: Объект оболочки, в которой хранятся ресурсы, связанные с назначением. Добавляет свойство **distributeForStudentWork** и указывает, что ресурс будет программы-оболочки
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: eb0879737d0375bf2463268fe29f2c98f2b6ed51
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991351"
---
# <a name="educationassignmentresource-resource-type"></a><span data-ttu-id="e6630-104">Тип ресурса educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="e6630-104">educationAssignmentResource resource type</span></span>

> <span data-ttu-id="e6630-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e6630-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e6630-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e6630-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e6630-107">Объект оболочки, в которой хранятся ресурсы, связанные с назначением.</span><span class="sxs-lookup"><span data-stu-id="e6630-107">A wrapper object that stores the resources associated with an assignment.</span></span> <span data-ttu-id="e6630-108">Программа-оболочка добавляет свойство **distributeForStudentWork** и указывает, что ресурс будет скопировать для отправки учебы.</span><span class="sxs-lookup"><span data-stu-id="e6630-108">The wrapper adds the **distributeForStudentWork** property and indicates that this resource will be copied to the student submission.</span></span>  <span data-ttu-id="e6630-109">Если объект не копируется, каждого студента появится ссылка на ресурс для назначения.</span><span class="sxs-lookup"><span data-stu-id="e6630-109">If the object is not copied, each student will see a link to the resource on the assignment.</span></span> <span data-ttu-id="e6630-110">Студент не сможет обновлять этот ресурс.</span><span class="sxs-lookup"><span data-stu-id="e6630-110">The student will not be able to update this resource.</span></span> <span data-ttu-id="e6630-111">Это выдаче преподаватель учебы ничего не включены.</span><span class="sxs-lookup"><span data-stu-id="e6630-111">This is a handout from the teacher to the student with nothing to be turned in.</span></span> <span data-ttu-id="e6630-112">Если распространяется ресурса, каждого студента будет получать копию этого ресурса в списке ресурсов их отправки.</span><span class="sxs-lookup"><span data-stu-id="e6630-112">If the resource is distributed, each student will receive a copy of this resource in the resource list of their submission.</span></span> <span data-ttu-id="e6630-113">Каждый студент будет изменять их копию и отправьте его для ранжирования.</span><span class="sxs-lookup"><span data-stu-id="e6630-113">Each student will be able to modify their copy and submit it for grading.</span></span>


## <a name="methods"></a><span data-ttu-id="e6630-114">Методы</span><span class="sxs-lookup"><span data-stu-id="e6630-114">Methods</span></span>

| <span data-ttu-id="e6630-115">Метод</span><span class="sxs-lookup"><span data-stu-id="e6630-115">Method</span></span>           | <span data-ttu-id="e6630-116">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e6630-116">Return Type</span></span>    |<span data-ttu-id="e6630-117">Описание</span><span class="sxs-lookup"><span data-stu-id="e6630-117">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e6630-118">Получение educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="e6630-118">Get educationAssignmentResource</span></span>](../api/educationassignmentresource-get.md) | [<span data-ttu-id="e6630-119">educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="e6630-119">educationAssignmentResource</span></span>](educationassignmentresource.md) |<span data-ttu-id="e6630-120">Чтение свойства и связи объекта **educationAssignmentResource** .</span><span class="sxs-lookup"><span data-stu-id="e6630-120">Read properties and relationships of an **educationAssignmentResource** object.</span></span>|
|<span data-ttu-id="e6630-121">[обновление](../api/educationassignmentresource-update.md);</span><span class="sxs-lookup"><span data-stu-id="e6630-121">[Update](../api/educationassignmentresource-update.md)</span></span> | [<span data-ttu-id="e6630-122">educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="e6630-122">educationAssignmentResource</span></span>](educationassignmentresource.md) |<span data-ttu-id="e6630-123">Обновление объекта **educationAssignmentResource** .</span><span class="sxs-lookup"><span data-stu-id="e6630-123">Update an **educationAssignmentResource** object.</span></span> |
|[<span data-ttu-id="e6630-124">Delete</span><span class="sxs-lookup"><span data-stu-id="e6630-124">Delete</span></span>](../api/educationassignmentresource-delete.md) | <span data-ttu-id="e6630-125">Нет</span><span class="sxs-lookup"><span data-stu-id="e6630-125">None</span></span> |<span data-ttu-id="e6630-126">Удаление объекта **educationAssignmentResource** .</span><span class="sxs-lookup"><span data-stu-id="e6630-126">Delete an **educationAssignmentResource** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="e6630-127">Свойства</span><span class="sxs-lookup"><span data-stu-id="e6630-127">Properties</span></span>
| <span data-ttu-id="e6630-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="e6630-128">Property</span></span>     | <span data-ttu-id="e6630-129">Тип</span><span class="sxs-lookup"><span data-stu-id="e6630-129">Type</span></span>   |<span data-ttu-id="e6630-130">Описание</span><span class="sxs-lookup"><span data-stu-id="e6630-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e6630-131">distributeForStudentWork</span><span class="sxs-lookup"><span data-stu-id="e6630-131">distributeForStudentWork</span></span>|<span data-ttu-id="e6630-132">Boolean</span><span class="sxs-lookup"><span data-stu-id="e6630-132">Boolean</span></span>|<span data-ttu-id="e6630-133">Указывает, будет ли этот ресурс необходимо копировать в каждой учебы отправки для изменения и отправки.</span><span class="sxs-lookup"><span data-stu-id="e6630-133">Indicates whether this resource should be copied to each student submission for modification and submission.</span></span>|
|<span data-ttu-id="e6630-134">id</span><span class="sxs-lookup"><span data-stu-id="e6630-134">id</span></span>|<span data-ttu-id="e6630-135">String</span><span class="sxs-lookup"><span data-stu-id="e6630-135">String</span></span>| <span data-ttu-id="e6630-136">Идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="e6630-136">ID of this resource.</span></span> <span data-ttu-id="e6630-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e6630-137">Read-only.</span></span>|
|<span data-ttu-id="e6630-138">resource</span><span class="sxs-lookup"><span data-stu-id="e6630-138">resource</span></span>|[<span data-ttu-id="e6630-139">educationResource</span><span class="sxs-lookup"><span data-stu-id="e6630-139">educationResource</span></span>](educationresource.md)|<span data-ttu-id="e6630-140">Объект ресурса, связанный с этим назначением.</span><span class="sxs-lookup"><span data-stu-id="e6630-140">Resource object that has been associated with this assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e6630-141">Связи</span><span class="sxs-lookup"><span data-stu-id="e6630-141">Relationships</span></span>
<span data-ttu-id="e6630-142">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e6630-142">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="e6630-143">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e6630-143">JSON representation</span></span>

<span data-ttu-id="e6630-144">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e6630-144">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationAssignmentResource"
}-->

```json
{
  "distributeForStudentWork": true,
  "id": "String (identifier)",
  "resource": {"@odata.type": "microsoft.graph.educationResource"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationAssignmentResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
