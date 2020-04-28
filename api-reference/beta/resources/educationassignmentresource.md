---
title: Тип ресурса Едукатионассигнментресаурце
description: Объект-оболочка, в котором хранятся ресурсы, связанные с назначением. Упаковщик добавляет свойство **дистрибутефорстудентворк** и указывает на то, что этот ресурс
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 0012344d2a641b892ae5e3fa905ce1e0c6282a5a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42502426"
---
# <a name="educationassignmentresource-resource-type"></a><span data-ttu-id="4eccd-104">Тип ресурса Едукатионассигнментресаурце</span><span class="sxs-lookup"><span data-stu-id="4eccd-104">educationAssignmentResource resource type</span></span>

<span data-ttu-id="4eccd-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4eccd-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4eccd-106">Объект-оболочка, в котором хранятся ресурсы, связанные с назначением.</span><span class="sxs-lookup"><span data-stu-id="4eccd-106">A wrapper object that stores the resources associated with an assignment.</span></span> <span data-ttu-id="4eccd-107">Оболочка добавляет свойство **дистрибутефорстудентворк** и указывает, что этот ресурс будет скопирован в отправку учащегося.</span><span class="sxs-lookup"><span data-stu-id="4eccd-107">The wrapper adds the **distributeForStudentWork** property and indicates that this resource will be copied to the student submission.</span></span>  <span data-ttu-id="4eccd-108">Если объект не копируется, каждый учащийся увидит ссылку на ресурс на назначении.</span><span class="sxs-lookup"><span data-stu-id="4eccd-108">If the object is not copied, each student will see a link to the resource on the assignment.</span></span> <span data-ttu-id="4eccd-109">Учащийся не сможет обновить этот ресурс.</span><span class="sxs-lookup"><span data-stu-id="4eccd-109">The student will not be able to update this resource.</span></span> <span data-ttu-id="4eccd-110">Это выдача от преподавателя к студенту, которую не следует включать.</span><span class="sxs-lookup"><span data-stu-id="4eccd-110">This is a handout from the teacher to the student with nothing to be turned in.</span></span> <span data-ttu-id="4eccd-111">Если ресурс распространяется, каждый учащийся получит копию этого ресурса в списке ресурсов их отправки.</span><span class="sxs-lookup"><span data-stu-id="4eccd-111">If the resource is distributed, each student will receive a copy of this resource in the resource list of their submission.</span></span> <span data-ttu-id="4eccd-112">Каждый студент сможет изменить свою копию и отправит их для ступенчатого.</span><span class="sxs-lookup"><span data-stu-id="4eccd-112">Each student will be able to modify their copy and submit it for grading.</span></span>


## <a name="methods"></a><span data-ttu-id="4eccd-113">Методы</span><span class="sxs-lookup"><span data-stu-id="4eccd-113">Methods</span></span>

| <span data-ttu-id="4eccd-114">Метод</span><span class="sxs-lookup"><span data-stu-id="4eccd-114">Method</span></span>           | <span data-ttu-id="4eccd-115">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4eccd-115">Return Type</span></span>    |<span data-ttu-id="4eccd-116">Описание</span><span class="sxs-lookup"><span data-stu-id="4eccd-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4eccd-117">Получение Едукатионассигнментресаурце</span><span class="sxs-lookup"><span data-stu-id="4eccd-117">Get educationAssignmentResource</span></span>](../api/educationassignmentresource-get.md) | [<span data-ttu-id="4eccd-118">едукатионассигнментресаурце</span><span class="sxs-lookup"><span data-stu-id="4eccd-118">educationAssignmentResource</span></span>](educationassignmentresource.md) |<span data-ttu-id="4eccd-119">Чтение свойств и связей объекта **едукатионассигнментресаурце** .</span><span class="sxs-lookup"><span data-stu-id="4eccd-119">Read properties and relationships of an **educationAssignmentResource** object.</span></span>|
|<span data-ttu-id="4eccd-120">[обновление](../api/educationassignmentresource-update.md).</span><span class="sxs-lookup"><span data-stu-id="4eccd-120">[Update](../api/educationassignmentresource-update.md)</span></span> | [<span data-ttu-id="4eccd-121">едукатионассигнментресаурце</span><span class="sxs-lookup"><span data-stu-id="4eccd-121">educationAssignmentResource</span></span>](educationassignmentresource.md) |<span data-ttu-id="4eccd-122">Обновление объекта **едукатионассигнментресаурце** .</span><span class="sxs-lookup"><span data-stu-id="4eccd-122">Update an **educationAssignmentResource** object.</span></span> |
|<span data-ttu-id="4eccd-123">[удаление](../api/educationassignmentresource-delete.md);</span><span class="sxs-lookup"><span data-stu-id="4eccd-123">[Delete](../api/educationassignmentresource-delete.md)</span></span> | <span data-ttu-id="4eccd-124">Нет</span><span class="sxs-lookup"><span data-stu-id="4eccd-124">None</span></span> |<span data-ttu-id="4eccd-125">Удаление объекта **едукатионассигнментресаурце** .</span><span class="sxs-lookup"><span data-stu-id="4eccd-125">Delete an **educationAssignmentResource** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="4eccd-126">Свойства</span><span class="sxs-lookup"><span data-stu-id="4eccd-126">Properties</span></span>
| <span data-ttu-id="4eccd-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="4eccd-127">Property</span></span>     | <span data-ttu-id="4eccd-128">Тип</span><span class="sxs-lookup"><span data-stu-id="4eccd-128">Type</span></span>   |<span data-ttu-id="4eccd-129">Описание</span><span class="sxs-lookup"><span data-stu-id="4eccd-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4eccd-130">дистрибутефорстудентворк</span><span class="sxs-lookup"><span data-stu-id="4eccd-130">distributeForStudentWork</span></span>|<span data-ttu-id="4eccd-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="4eccd-131">Boolean</span></span>|<span data-ttu-id="4eccd-132">Указывает, следует ли копировать этот ресурс в каждую отправку учащегося для изменения и отправки.</span><span class="sxs-lookup"><span data-stu-id="4eccd-132">Indicates whether this resource should be copied to each student submission for modification and submission.</span></span>|
|<span data-ttu-id="4eccd-133">id</span><span class="sxs-lookup"><span data-stu-id="4eccd-133">id</span></span>|<span data-ttu-id="4eccd-134">String</span><span class="sxs-lookup"><span data-stu-id="4eccd-134">String</span></span>| <span data-ttu-id="4eccd-135">ИДЕНТИФИКАТОР этого ресурса.</span><span class="sxs-lookup"><span data-stu-id="4eccd-135">ID of this resource.</span></span> <span data-ttu-id="4eccd-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4eccd-136">Read-only.</span></span>|
|<span data-ttu-id="4eccd-137">resource</span><span class="sxs-lookup"><span data-stu-id="4eccd-137">resource</span></span>|[<span data-ttu-id="4eccd-138">едукатионресаурце</span><span class="sxs-lookup"><span data-stu-id="4eccd-138">educationResource</span></span>](educationresource.md)|<span data-ttu-id="4eccd-139">Объект ресурса, связанный с этим назначением.</span><span class="sxs-lookup"><span data-stu-id="4eccd-139">Resource object that has been associated with this assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4eccd-140">Связи</span><span class="sxs-lookup"><span data-stu-id="4eccd-140">Relationships</span></span>
<span data-ttu-id="4eccd-141">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="4eccd-141">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="4eccd-142">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="4eccd-142">JSON representation</span></span>

<span data-ttu-id="4eccd-143">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4eccd-143">The following is a JSON representation of the resource.</span></span>

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
