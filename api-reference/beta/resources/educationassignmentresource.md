---
title: Тип ресурса Едукатионассигнментресаурце
description: Объект-оболочка, в котором хранятся ресурсы, связанные с назначением. Упаковщик добавляет свойство **дистрибутефорстудентворк** и указывает на то, что этот ресурс
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: 08a716edabc31c83a7fb3e358fbafd023d5fa784
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334413"
---
# <a name="educationassignmentresource-resource-type"></a><span data-ttu-id="fc47f-104">Тип ресурса Едукатионассигнментресаурце</span><span class="sxs-lookup"><span data-stu-id="fc47f-104">educationAssignmentResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fc47f-105">Объект-оболочка, в котором хранятся ресурсы, связанные с назначением.</span><span class="sxs-lookup"><span data-stu-id="fc47f-105">A wrapper object that stores the resources associated with an assignment.</span></span> <span data-ttu-id="fc47f-106">Оболочка добавляет свойство **дистрибутефорстудентворк** и указывает, что этот ресурс будет скопирован в отправку учащегося.</span><span class="sxs-lookup"><span data-stu-id="fc47f-106">The wrapper adds the **distributeForStudentWork** property and indicates that this resource will be copied to the student submission.</span></span>  <span data-ttu-id="fc47f-107">Если объект не копируется, каждый учащийся увидит ссылку на ресурс на назначении.</span><span class="sxs-lookup"><span data-stu-id="fc47f-107">If the object is not copied, each student will see a link to the resource on the assignment.</span></span> <span data-ttu-id="fc47f-108">Учащийся не сможет обновить этот ресурс.</span><span class="sxs-lookup"><span data-stu-id="fc47f-108">The student will not be able to update this resource.</span></span> <span data-ttu-id="fc47f-109">Это выдача от преподавателя к студенту, которую не следует включать.</span><span class="sxs-lookup"><span data-stu-id="fc47f-109">This is a handout from the teacher to the student with nothing to be turned in.</span></span> <span data-ttu-id="fc47f-110">Если ресурс распространяется, каждый учащийся получит копию этого ресурса в списке ресурсов их отправки.</span><span class="sxs-lookup"><span data-stu-id="fc47f-110">If the resource is distributed, each student will receive a copy of this resource in the resource list of their submission.</span></span> <span data-ttu-id="fc47f-111">Каждый студент сможет изменить свою копию и отправит их для ступенчатого.</span><span class="sxs-lookup"><span data-stu-id="fc47f-111">Each student will be able to modify their copy and submit it for grading.</span></span>


## <a name="methods"></a><span data-ttu-id="fc47f-112">Методы</span><span class="sxs-lookup"><span data-stu-id="fc47f-112">Methods</span></span>

| <span data-ttu-id="fc47f-113">Метод</span><span class="sxs-lookup"><span data-stu-id="fc47f-113">Method</span></span>           | <span data-ttu-id="fc47f-114">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="fc47f-114">Return Type</span></span>    |<span data-ttu-id="fc47f-115">Описание</span><span class="sxs-lookup"><span data-stu-id="fc47f-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fc47f-116">Получение Едукатионассигнментресаурце</span><span class="sxs-lookup"><span data-stu-id="fc47f-116">Get educationAssignmentResource</span></span>](../api/educationassignmentresource-get.md) | [<span data-ttu-id="fc47f-117">Едукатионассигнментресаурце</span><span class="sxs-lookup"><span data-stu-id="fc47f-117">educationAssignmentResource</span></span>](educationassignmentresource.md) |<span data-ttu-id="fc47f-118">Чтение свойств и связей объекта **едукатионассигнментресаурце** .</span><span class="sxs-lookup"><span data-stu-id="fc47f-118">Read properties and relationships of an **educationAssignmentResource** object.</span></span>|
|[<span data-ttu-id="fc47f-119">Update</span><span class="sxs-lookup"><span data-stu-id="fc47f-119">Update</span></span>](../api/educationassignmentresource-update.md) | [<span data-ttu-id="fc47f-120">Едукатионассигнментресаурце</span><span class="sxs-lookup"><span data-stu-id="fc47f-120">educationAssignmentResource</span></span>](educationassignmentresource.md) |<span data-ttu-id="fc47f-121">Обновление объекта **едукатионассигнментресаурце** .</span><span class="sxs-lookup"><span data-stu-id="fc47f-121">Update an **educationAssignmentResource** object.</span></span> |
|[<span data-ttu-id="fc47f-122">Delete</span><span class="sxs-lookup"><span data-stu-id="fc47f-122">Delete</span></span>](../api/educationassignmentresource-delete.md) | <span data-ttu-id="fc47f-123">Нет</span><span class="sxs-lookup"><span data-stu-id="fc47f-123">None</span></span> |<span data-ttu-id="fc47f-124">Удаление объекта **едукатионассигнментресаурце** .</span><span class="sxs-lookup"><span data-stu-id="fc47f-124">Delete an **educationAssignmentResource** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="fc47f-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="fc47f-125">Properties</span></span>
| <span data-ttu-id="fc47f-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="fc47f-126">Property</span></span>     | <span data-ttu-id="fc47f-127">Тип</span><span class="sxs-lookup"><span data-stu-id="fc47f-127">Type</span></span>   |<span data-ttu-id="fc47f-128">Описание</span><span class="sxs-lookup"><span data-stu-id="fc47f-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fc47f-129">Дистрибутефорстудентворк</span><span class="sxs-lookup"><span data-stu-id="fc47f-129">distributeForStudentWork</span></span>|<span data-ttu-id="fc47f-130">Логический</span><span class="sxs-lookup"><span data-stu-id="fc47f-130">Boolean</span></span>|<span data-ttu-id="fc47f-131">Указывает, следует ли копировать этот ресурс в каждую отправку учащегося для изменения и отправки.</span><span class="sxs-lookup"><span data-stu-id="fc47f-131">Indicates whether this resource should be copied to each student submission for modification and submission.</span></span>|
|<span data-ttu-id="fc47f-132">id</span><span class="sxs-lookup"><span data-stu-id="fc47f-132">id</span></span>|<span data-ttu-id="fc47f-133">String</span><span class="sxs-lookup"><span data-stu-id="fc47f-133">String</span></span>| <span data-ttu-id="fc47f-134">ИДЕНТИФИКАТОР этого ресурса.</span><span class="sxs-lookup"><span data-stu-id="fc47f-134">ID of this resource.</span></span> <span data-ttu-id="fc47f-135">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fc47f-135">Read-only.</span></span>|
|<span data-ttu-id="fc47f-136">resource</span><span class="sxs-lookup"><span data-stu-id="fc47f-136">resource</span></span>|[<span data-ttu-id="fc47f-137">Едукатионресаурце</span><span class="sxs-lookup"><span data-stu-id="fc47f-137">educationResource</span></span>](educationresource.md)|<span data-ttu-id="fc47f-138">Объект ресурса, связанный с этим назначением.</span><span class="sxs-lookup"><span data-stu-id="fc47f-138">Resource object that has been associated with this assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fc47f-139">Связи</span><span class="sxs-lookup"><span data-stu-id="fc47f-139">Relationships</span></span>
<span data-ttu-id="fc47f-140">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="fc47f-140">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="fc47f-141">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="fc47f-141">JSON representation</span></span>

<span data-ttu-id="fc47f-142">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fc47f-142">The following is a JSON representation of the resource.</span></span>

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
