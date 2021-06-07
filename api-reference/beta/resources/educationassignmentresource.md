---
title: тип ресурса educationAssignmentResource
description: Объект оболочки, который хранит ресурсы, связанные с назначением. Оболочка добавляет свойство **distributeForStudentWork** и указывает, что этот ресурс будет
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: a4f4e96c4b08eed4584d6357a8c903c080b2d16d
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52750373"
---
# <a name="educationassignmentresource-resource-type"></a><span data-ttu-id="01a14-104">тип ресурса educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="01a14-104">educationAssignmentResource resource type</span></span>

<span data-ttu-id="01a14-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="01a14-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="01a14-106">Объект оболочки, который хранит ресурсы, связанные с назначением.</span><span class="sxs-lookup"><span data-stu-id="01a14-106">A wrapper object that stores the resources associated with an assignment.</span></span> <span data-ttu-id="01a14-107">Оболочка добавляет свойство **distributeForStudentWork** и указывает, что этот ресурс будет скопирован в студенческую отправку.</span><span class="sxs-lookup"><span data-stu-id="01a14-107">The wrapper adds the **distributeForStudentWork** property and indicates that this resource will be copied to the student submission.</span></span>  <span data-ttu-id="01a14-108">Если объект не копируется, каждый учащийся увидит ссылку на ресурс в задании.</span><span class="sxs-lookup"><span data-stu-id="01a14-108">If the object is not copied, each student will see a link to the resource on the assignment.</span></span> <span data-ttu-id="01a14-109">Студент не сможет обновить этот ресурс.</span><span class="sxs-lookup"><span data-stu-id="01a14-109">The student will not be able to update this resource.</span></span> <span data-ttu-id="01a14-110">Это раздатка от преподавателя ученику без включаемой информации.</span><span class="sxs-lookup"><span data-stu-id="01a14-110">This is a handout from the teacher to the student with nothing to be turned in.</span></span> <span data-ttu-id="01a14-111">Если ресурс распространяется, каждый учащийся получит копию этого ресурса в списке ресурсов их отправки.</span><span class="sxs-lookup"><span data-stu-id="01a14-111">If the resource is distributed, each student will receive a copy of this resource in the resource list of their submission.</span></span> <span data-ttu-id="01a14-112">Каждый студент сможет изменить свою копию и отправить ее для классификации.</span><span class="sxs-lookup"><span data-stu-id="01a14-112">Each student will be able to modify their copy and submit it for grading.</span></span>


## <a name="methods"></a><span data-ttu-id="01a14-113">Методы</span><span class="sxs-lookup"><span data-stu-id="01a14-113">Methods</span></span>

| <span data-ttu-id="01a14-114">Метод</span><span class="sxs-lookup"><span data-stu-id="01a14-114">Method</span></span>           | <span data-ttu-id="01a14-115">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="01a14-115">Return Type</span></span>    |<span data-ttu-id="01a14-116">Описание</span><span class="sxs-lookup"><span data-stu-id="01a14-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="01a14-117">Get educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="01a14-117">Get educationAssignmentResource</span></span>](../api/educationassignmentresource-get.md) | [<span data-ttu-id="01a14-118">educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="01a14-118">educationAssignmentResource</span></span>](educationassignmentresource.md) |<span data-ttu-id="01a14-119">Чтение свойств и связей объекта **educationAssignmentResource.**</span><span class="sxs-lookup"><span data-stu-id="01a14-119">Read properties and relationships of an **educationAssignmentResource** object.</span></span>|
|[<span data-ttu-id="01a14-120">Delete</span><span class="sxs-lookup"><span data-stu-id="01a14-120">Delete</span></span>](../api/educationassignmentresource-delete.md) | <span data-ttu-id="01a14-121">Нет.</span><span class="sxs-lookup"><span data-stu-id="01a14-121">None</span></span> |<span data-ttu-id="01a14-122">Удаление **объекта educationAssignmentResource.**</span><span class="sxs-lookup"><span data-stu-id="01a14-122">Delete an **educationAssignmentResource** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="01a14-123">Свойства</span><span class="sxs-lookup"><span data-stu-id="01a14-123">Properties</span></span>
| <span data-ttu-id="01a14-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="01a14-124">Property</span></span>     | <span data-ttu-id="01a14-125">Тип</span><span class="sxs-lookup"><span data-stu-id="01a14-125">Type</span></span>   |<span data-ttu-id="01a14-126">Описание</span><span class="sxs-lookup"><span data-stu-id="01a14-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="01a14-127">distributeForStudentWork</span><span class="sxs-lookup"><span data-stu-id="01a14-127">distributeForStudentWork</span></span>|<span data-ttu-id="01a14-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="01a14-128">Boolean</span></span>|<span data-ttu-id="01a14-129">Указывает, следует ли скопировать этот ресурс для каждого студента для изменения и отправки.</span><span class="sxs-lookup"><span data-stu-id="01a14-129">Indicates whether this resource should be copied to each student submission for modification and submission.</span></span>|
|<span data-ttu-id="01a14-130">id</span><span class="sxs-lookup"><span data-stu-id="01a14-130">id</span></span>|<span data-ttu-id="01a14-131">String</span><span class="sxs-lookup"><span data-stu-id="01a14-131">String</span></span>| <span data-ttu-id="01a14-132">ID этого ресурса.</span><span class="sxs-lookup"><span data-stu-id="01a14-132">ID of this resource.</span></span> <span data-ttu-id="01a14-133">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="01a14-133">Read-only.</span></span>|
|<span data-ttu-id="01a14-134">resource</span><span class="sxs-lookup"><span data-stu-id="01a14-134">resource</span></span>|[<span data-ttu-id="01a14-135">educationResource</span><span class="sxs-lookup"><span data-stu-id="01a14-135">educationResource</span></span>](educationresource.md)|<span data-ttu-id="01a14-136">Объект resource, связанный с этим назначением.</span><span class="sxs-lookup"><span data-stu-id="01a14-136">Resource object that has been associated with this assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="01a14-137">Отношения</span><span class="sxs-lookup"><span data-stu-id="01a14-137">Relationships</span></span>
<span data-ttu-id="01a14-138">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="01a14-138">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="01a14-139">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="01a14-139">JSON representation</span></span>

<span data-ttu-id="01a14-140">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="01a14-140">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->


