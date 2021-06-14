---
title: тип ресурса educationAssignmentResource
description: Объект оболочки, который хранит ресурсы, связанные с назначением.
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: d301eb8f0d9b9f13197be01b2bcf3ccf4297fa24
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912859"
---
# <a name="educationassignmentresource-resource-type"></a><span data-ttu-id="b759e-103">тип ресурса educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="b759e-103">educationAssignmentResource resource type</span></span>

<span data-ttu-id="b759e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b759e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b759e-105">Объект оболочки, который хранит ресурсы, связанные с назначением.</span><span class="sxs-lookup"><span data-stu-id="b759e-105">A wrapper object that stores the resources associated with an assignment.</span></span> 

<span data-ttu-id="b759e-106">Оболочка добавляет свойство **distributeForStudentWork** и указывает, что этот ресурс будет скопирован в студенческую отправку.</span><span class="sxs-lookup"><span data-stu-id="b759e-106">The wrapper adds the **distributeForStudentWork** property and indicates that this resource will be copied to the student submission.</span></span>  <span data-ttu-id="b759e-107">Если объект не копируется, каждый учащийся увидит ссылку на ресурс в задании.</span><span class="sxs-lookup"><span data-stu-id="b759e-107">If the object isn't copied, each student will see a link to the resource on the assignment.</span></span> <span data-ttu-id="b759e-108">Студент не сможет обновить этот ресурс.</span><span class="sxs-lookup"><span data-stu-id="b759e-108">The student will not be able to update this resource.</span></span> <span data-ttu-id="b759e-109">Это раздатка от преподавателя ученику без включаемой информации.</span><span class="sxs-lookup"><span data-stu-id="b759e-109">This is a handout from the teacher to the student with nothing to be turned in.</span></span> <span data-ttu-id="b759e-110">Если ресурс распространяется, каждый учащийся получит копию этого ресурса в списке ресурсов их отправки.</span><span class="sxs-lookup"><span data-stu-id="b759e-110">If the resource is distributed, each student will receive a copy of this resource in the resource list of their submission.</span></span> <span data-ttu-id="b759e-111">Каждый студент сможет изменить свою копию и отправить ее для классификации.</span><span class="sxs-lookup"><span data-stu-id="b759e-111">Each student will be able to modify their copy and submit it for grading.</span></span>


## <a name="methods"></a><span data-ttu-id="b759e-112">Методы</span><span class="sxs-lookup"><span data-stu-id="b759e-112">Methods</span></span>

| <span data-ttu-id="b759e-113">Метод</span><span class="sxs-lookup"><span data-stu-id="b759e-113">Method</span></span>           | <span data-ttu-id="b759e-114">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b759e-114">Return Type</span></span>    |<span data-ttu-id="b759e-115">Описание</span><span class="sxs-lookup"><span data-stu-id="b759e-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b759e-116">Get educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="b759e-116">Get educationAssignmentResource</span></span>](../api/educationassignmentresource-get.md) | [<span data-ttu-id="b759e-117">educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="b759e-117">educationAssignmentResource</span></span>](educationassignmentresource.md) |<span data-ttu-id="b759e-118">Чтение свойств и связей объекта **educationAssignmentResource.**</span><span class="sxs-lookup"><span data-stu-id="b759e-118">Read properties and relationships of an **educationAssignmentResource** object.</span></span>|
|[<span data-ttu-id="b759e-119">Удаление</span><span class="sxs-lookup"><span data-stu-id="b759e-119">Delete</span></span>](../api/educationassignmentresource-delete.md) | <span data-ttu-id="b759e-120">Нет</span><span class="sxs-lookup"><span data-stu-id="b759e-120">None</span></span> |<span data-ttu-id="b759e-121">Удаление **объекта educationAssignmentResource.**</span><span class="sxs-lookup"><span data-stu-id="b759e-121">Delete an **educationAssignmentResource** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="b759e-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="b759e-122">Properties</span></span>
| <span data-ttu-id="b759e-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="b759e-123">Property</span></span>     | <span data-ttu-id="b759e-124">Тип</span><span class="sxs-lookup"><span data-stu-id="b759e-124">Type</span></span>   |<span data-ttu-id="b759e-125">Описание</span><span class="sxs-lookup"><span data-stu-id="b759e-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b759e-126">distributeForStudentWork</span><span class="sxs-lookup"><span data-stu-id="b759e-126">distributeForStudentWork</span></span>|<span data-ttu-id="b759e-127">Логический</span><span class="sxs-lookup"><span data-stu-id="b759e-127">Boolean</span></span>|<span data-ttu-id="b759e-128">Указывает, следует ли скопировать этот ресурс для каждого студента для изменения и отправки.</span><span class="sxs-lookup"><span data-stu-id="b759e-128">Indicates whether this resource should be copied to each student submission for modification and submission.</span></span>|
|<span data-ttu-id="b759e-129">id</span><span class="sxs-lookup"><span data-stu-id="b759e-129">id</span></span>|<span data-ttu-id="b759e-130">String</span><span class="sxs-lookup"><span data-stu-id="b759e-130">String</span></span>| <span data-ttu-id="b759e-131">ID этого ресурса.</span><span class="sxs-lookup"><span data-stu-id="b759e-131">ID of this resource.</span></span> <span data-ttu-id="b759e-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b759e-132">Read-only.</span></span>|
|<span data-ttu-id="b759e-133">resource</span><span class="sxs-lookup"><span data-stu-id="b759e-133">resource</span></span>|[<span data-ttu-id="b759e-134">educationResource</span><span class="sxs-lookup"><span data-stu-id="b759e-134">educationResource</span></span>](educationresource.md)|<span data-ttu-id="b759e-135">Объект resource, связанный с этим назначением.</span><span class="sxs-lookup"><span data-stu-id="b759e-135">Resource object that has been associated with this assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b759e-136">Связи</span><span class="sxs-lookup"><span data-stu-id="b759e-136">Relationships</span></span>
<span data-ttu-id="b759e-137">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="b759e-137">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="b759e-138">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="b759e-138">JSON representation</span></span>

<span data-ttu-id="b759e-139">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b759e-139">The following is a JSON representation of the resource.</span></span>

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


