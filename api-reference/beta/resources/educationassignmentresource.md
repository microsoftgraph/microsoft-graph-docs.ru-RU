---
title: Тип ресурса educationAssignmentResource
description: Объект оболочки, в которой хранятся ресурсы, связанные с назначением. Добавляет свойство **distributeForStudentWork** и указывает, что ресурс будет программы-оболочки
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: 4d05cf5307e77dc6a7ac438c1bd4f4af4e73784e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529231"
---
# <a name="educationassignmentresource-resource-type"></a><span data-ttu-id="75b81-104">Тип ресурса educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="75b81-104">educationAssignmentResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="75b81-105">Объект оболочки, в которой хранятся ресурсы, связанные с назначением.</span><span class="sxs-lookup"><span data-stu-id="75b81-105">A wrapper object that stores the resources associated with an assignment.</span></span> <span data-ttu-id="75b81-106">Программа-оболочка добавляет свойство **distributeForStudentWork** и указывает, что ресурс будет скопировать для отправки учебы.</span><span class="sxs-lookup"><span data-stu-id="75b81-106">The wrapper adds the **distributeForStudentWork** property and indicates that this resource will be copied to the student submission.</span></span>  <span data-ttu-id="75b81-107">Если объект не копируется, каждого студента появится ссылка на ресурс для назначения.</span><span class="sxs-lookup"><span data-stu-id="75b81-107">If the object is not copied, each student will see a link to the resource on the assignment.</span></span> <span data-ttu-id="75b81-108">Студент не сможет обновлять этот ресурс.</span><span class="sxs-lookup"><span data-stu-id="75b81-108">The student will not be able to update this resource.</span></span> <span data-ttu-id="75b81-109">Это выдаче преподаватель учебы ничего не включены.</span><span class="sxs-lookup"><span data-stu-id="75b81-109">This is a handout from the teacher to the student with nothing to be turned in.</span></span> <span data-ttu-id="75b81-110">Если распространяется ресурса, каждого студента будет получать копию этого ресурса в списке ресурсов их отправки.</span><span class="sxs-lookup"><span data-stu-id="75b81-110">If the resource is distributed, each student will receive a copy of this resource in the resource list of their submission.</span></span> <span data-ttu-id="75b81-111">Каждый студент будет изменять их копию и отправьте его для ранжирования.</span><span class="sxs-lookup"><span data-stu-id="75b81-111">Each student will be able to modify their copy and submit it for grading.</span></span>


## <a name="methods"></a><span data-ttu-id="75b81-112">Методы</span><span class="sxs-lookup"><span data-stu-id="75b81-112">Methods</span></span>

| <span data-ttu-id="75b81-113">Метод</span><span class="sxs-lookup"><span data-stu-id="75b81-113">Method</span></span>           | <span data-ttu-id="75b81-114">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="75b81-114">Return Type</span></span>    |<span data-ttu-id="75b81-115">Описание</span><span class="sxs-lookup"><span data-stu-id="75b81-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="75b81-116">Получение educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="75b81-116">Get educationAssignmentResource</span></span>](../api/educationassignmentresource-get.md) | [<span data-ttu-id="75b81-117">educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="75b81-117">educationAssignmentResource</span></span>](educationassignmentresource.md) |<span data-ttu-id="75b81-118">Чтение свойства и связи объекта **educationAssignmentResource** .</span><span class="sxs-lookup"><span data-stu-id="75b81-118">Read properties and relationships of an **educationAssignmentResource** object.</span></span>|
|[<span data-ttu-id="75b81-119">Update</span><span class="sxs-lookup"><span data-stu-id="75b81-119">Update</span></span>](../api/educationassignmentresource-update.md) | [<span data-ttu-id="75b81-120">educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="75b81-120">educationAssignmentResource</span></span>](educationassignmentresource.md) |<span data-ttu-id="75b81-121">Обновление объекта **educationAssignmentResource** .</span><span class="sxs-lookup"><span data-stu-id="75b81-121">Update an **educationAssignmentResource** object.</span></span> |
|[<span data-ttu-id="75b81-122">Delete</span><span class="sxs-lookup"><span data-stu-id="75b81-122">Delete</span></span>](../api/educationassignmentresource-delete.md) | <span data-ttu-id="75b81-123">Нет</span><span class="sxs-lookup"><span data-stu-id="75b81-123">None</span></span> |<span data-ttu-id="75b81-124">Удаление объекта **educationAssignmentResource** .</span><span class="sxs-lookup"><span data-stu-id="75b81-124">Delete an **educationAssignmentResource** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="75b81-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="75b81-125">Properties</span></span>
| <span data-ttu-id="75b81-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="75b81-126">Property</span></span>     | <span data-ttu-id="75b81-127">Тип</span><span class="sxs-lookup"><span data-stu-id="75b81-127">Type</span></span>   |<span data-ttu-id="75b81-128">Описание</span><span class="sxs-lookup"><span data-stu-id="75b81-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="75b81-129">distributeForStudentWork</span><span class="sxs-lookup"><span data-stu-id="75b81-129">distributeForStudentWork</span></span>|<span data-ttu-id="75b81-130">Логическое</span><span class="sxs-lookup"><span data-stu-id="75b81-130">Boolean</span></span>|<span data-ttu-id="75b81-131">Указывает, будет ли этот ресурс необходимо копировать в каждой учебы отправки для изменения и отправки.</span><span class="sxs-lookup"><span data-stu-id="75b81-131">Indicates whether this resource should be copied to each student submission for modification and submission.</span></span>|
|<span data-ttu-id="75b81-132">id</span><span class="sxs-lookup"><span data-stu-id="75b81-132">id</span></span>|<span data-ttu-id="75b81-133">String</span><span class="sxs-lookup"><span data-stu-id="75b81-133">String</span></span>| <span data-ttu-id="75b81-134">Идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="75b81-134">ID of this resource.</span></span> <span data-ttu-id="75b81-135">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="75b81-135">Read-only.</span></span>|
|<span data-ttu-id="75b81-136">resource</span><span class="sxs-lookup"><span data-stu-id="75b81-136">resource</span></span>|[<span data-ttu-id="75b81-137">educationResource</span><span class="sxs-lookup"><span data-stu-id="75b81-137">educationResource</span></span>](educationresource.md)|<span data-ttu-id="75b81-138">Объект ресурса, связанный с этим назначением.</span><span class="sxs-lookup"><span data-stu-id="75b81-138">Resource object that has been associated with this assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="75b81-139">Отношения</span><span class="sxs-lookup"><span data-stu-id="75b81-139">Relationships</span></span>
<span data-ttu-id="75b81-140">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="75b81-140">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="75b81-141">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="75b81-141">JSON representation</span></span>

<span data-ttu-id="75b81-142">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="75b81-142">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "educationAssignmentResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationassignmentresource.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
