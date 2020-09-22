---
title: Тип ресурса Едукатионассигнментресаурце
description: Объект-оболочка, в котором хранятся ресурсы, связанные с назначением. Упаковщик добавляет свойство **дистрибутефорстудентворк** и указывает на то, что этот ресурс
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 462433a24b8515146303505865b3d356d025d6c4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095550"
---
# <a name="educationassignmentresource-resource-type"></a><span data-ttu-id="28138-104">Тип ресурса Едукатионассигнментресаурце</span><span class="sxs-lookup"><span data-stu-id="28138-104">educationAssignmentResource resource type</span></span>

<span data-ttu-id="28138-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="28138-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="28138-106">Объект-оболочка, в котором хранятся ресурсы, связанные с назначением.</span><span class="sxs-lookup"><span data-stu-id="28138-106">A wrapper object that stores the resources associated with an assignment.</span></span> <span data-ttu-id="28138-107">Оболочка добавляет свойство **дистрибутефорстудентворк** и указывает, что этот ресурс будет скопирован в отправку учащегося.</span><span class="sxs-lookup"><span data-stu-id="28138-107">The wrapper adds the **distributeForStudentWork** property and indicates that this resource will be copied to the student submission.</span></span>  <span data-ttu-id="28138-108">Если объект не копируется, каждый учащийся увидит ссылку на ресурс на назначении.</span><span class="sxs-lookup"><span data-stu-id="28138-108">If the object is not copied, each student will see a link to the resource on the assignment.</span></span> <span data-ttu-id="28138-109">Учащийся не сможет обновить этот ресурс.</span><span class="sxs-lookup"><span data-stu-id="28138-109">The student will not be able to update this resource.</span></span> <span data-ttu-id="28138-110">Это выдача от преподавателя к студенту, которую не следует включать.</span><span class="sxs-lookup"><span data-stu-id="28138-110">This is a handout from the teacher to the student with nothing to be turned in.</span></span> <span data-ttu-id="28138-111">Если ресурс распространяется, каждый учащийся получит копию этого ресурса в списке ресурсов их отправки.</span><span class="sxs-lookup"><span data-stu-id="28138-111">If the resource is distributed, each student will receive a copy of this resource in the resource list of their submission.</span></span> <span data-ttu-id="28138-112">Каждый студент сможет изменить свою копию и отправит их для ступенчатого.</span><span class="sxs-lookup"><span data-stu-id="28138-112">Each student will be able to modify their copy and submit it for grading.</span></span>


## <a name="methods"></a><span data-ttu-id="28138-113">Методы</span><span class="sxs-lookup"><span data-stu-id="28138-113">Methods</span></span>

| <span data-ttu-id="28138-114">Метод</span><span class="sxs-lookup"><span data-stu-id="28138-114">Method</span></span>           | <span data-ttu-id="28138-115">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="28138-115">Return Type</span></span>    |<span data-ttu-id="28138-116">Описание</span><span class="sxs-lookup"><span data-stu-id="28138-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="28138-117">Получение Едукатионассигнментресаурце</span><span class="sxs-lookup"><span data-stu-id="28138-117">Get educationAssignmentResource</span></span>](../api/educationassignmentresource-get.md) | [<span data-ttu-id="28138-118">едукатионассигнментресаурце</span><span class="sxs-lookup"><span data-stu-id="28138-118">educationAssignmentResource</span></span>](educationassignmentresource.md) |<span data-ttu-id="28138-119">Чтение свойств и связей объекта **едукатионассигнментресаурце** .</span><span class="sxs-lookup"><span data-stu-id="28138-119">Read properties and relationships of an **educationAssignmentResource** object.</span></span>|
|[<span data-ttu-id="28138-120">Обновление</span><span class="sxs-lookup"><span data-stu-id="28138-120">Update</span></span>](../api/educationassignmentresource-update.md) | [<span data-ttu-id="28138-121">едукатионассигнментресаурце</span><span class="sxs-lookup"><span data-stu-id="28138-121">educationAssignmentResource</span></span>](educationassignmentresource.md) |<span data-ttu-id="28138-122">Обновление объекта **едукатионассигнментресаурце** .</span><span class="sxs-lookup"><span data-stu-id="28138-122">Update an **educationAssignmentResource** object.</span></span> |
|<span data-ttu-id="28138-123">[удаление](../api/educationassignmentresource-delete.md);</span><span class="sxs-lookup"><span data-stu-id="28138-123">[Delete](../api/educationassignmentresource-delete.md)</span></span> | <span data-ttu-id="28138-124">Нет</span><span class="sxs-lookup"><span data-stu-id="28138-124">None</span></span> |<span data-ttu-id="28138-125">Удаление объекта **едукатионассигнментресаурце** .</span><span class="sxs-lookup"><span data-stu-id="28138-125">Delete an **educationAssignmentResource** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="28138-126">Свойства</span><span class="sxs-lookup"><span data-stu-id="28138-126">Properties</span></span>
| <span data-ttu-id="28138-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="28138-127">Property</span></span>     | <span data-ttu-id="28138-128">Тип</span><span class="sxs-lookup"><span data-stu-id="28138-128">Type</span></span>   |<span data-ttu-id="28138-129">Описание</span><span class="sxs-lookup"><span data-stu-id="28138-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="28138-130">дистрибутефорстудентворк</span><span class="sxs-lookup"><span data-stu-id="28138-130">distributeForStudentWork</span></span>|<span data-ttu-id="28138-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="28138-131">Boolean</span></span>|<span data-ttu-id="28138-132">Указывает, следует ли копировать этот ресурс в каждую отправку учащегося для изменения и отправки.</span><span class="sxs-lookup"><span data-stu-id="28138-132">Indicates whether this resource should be copied to each student submission for modification and submission.</span></span>|
|<span data-ttu-id="28138-133">id</span><span class="sxs-lookup"><span data-stu-id="28138-133">id</span></span>|<span data-ttu-id="28138-134">Строка</span><span class="sxs-lookup"><span data-stu-id="28138-134">String</span></span>| <span data-ttu-id="28138-135">ИДЕНТИФИКАТОР этого ресурса.</span><span class="sxs-lookup"><span data-stu-id="28138-135">ID of this resource.</span></span> <span data-ttu-id="28138-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="28138-136">Read-only.</span></span>|
|<span data-ttu-id="28138-137">resource</span><span class="sxs-lookup"><span data-stu-id="28138-137">resource</span></span>|[<span data-ttu-id="28138-138">едукатионресаурце</span><span class="sxs-lookup"><span data-stu-id="28138-138">educationResource</span></span>](educationresource.md)|<span data-ttu-id="28138-139">Объект ресурса, связанный с этим назначением.</span><span class="sxs-lookup"><span data-stu-id="28138-139">Resource object that has been associated with this assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="28138-140">Связи</span><span class="sxs-lookup"><span data-stu-id="28138-140">Relationships</span></span>
<span data-ttu-id="28138-141">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="28138-141">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="28138-142">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="28138-142">JSON representation</span></span>

<span data-ttu-id="28138-143">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="28138-143">The following is a JSON representation of the resource.</span></span>

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


