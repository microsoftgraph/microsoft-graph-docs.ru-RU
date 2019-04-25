---
title: Тип ресурса Едукатионассигнментресаурце
description: Объект-оболочка, в котором хранятся ресурсы, связанные с назначением. Упаковщик добавляет свойство **дистрибутефорстудентворк** и указывает на то, что этот ресурс
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: 4d05cf5307e77dc6a7ac438c1bd4f4af4e73784e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32542987"
---
# <a name="educationassignmentresource-resource-type"></a><span data-ttu-id="2b249-104">Тип ресурса Едукатионассигнментресаурце</span><span class="sxs-lookup"><span data-stu-id="2b249-104">educationAssignmentResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2b249-105">Объект-оболочка, в котором хранятся ресурсы, связанные с назначением.</span><span class="sxs-lookup"><span data-stu-id="2b249-105">A wrapper object that stores the resources associated with an assignment.</span></span> <span data-ttu-id="2b249-106">Оболочка добавляет свойство **дистрибутефорстудентворк** и указывает, что этот ресурс будет скопирован в отправку учащегося.</span><span class="sxs-lookup"><span data-stu-id="2b249-106">The wrapper adds the **distributeForStudentWork** property and indicates that this resource will be copied to the student submission.</span></span>  <span data-ttu-id="2b249-107">Если объект не копируется, каждый учащийся увидит ссылку на ресурс на назначении.</span><span class="sxs-lookup"><span data-stu-id="2b249-107">If the object is not copied, each student will see a link to the resource on the assignment.</span></span> <span data-ttu-id="2b249-108">Учащийся не сможет обновить этот ресурс.</span><span class="sxs-lookup"><span data-stu-id="2b249-108">The student will not be able to update this resource.</span></span> <span data-ttu-id="2b249-109">Это выдача от преподавателя к студенту, которую не следует включать.</span><span class="sxs-lookup"><span data-stu-id="2b249-109">This is a handout from the teacher to the student with nothing to be turned in.</span></span> <span data-ttu-id="2b249-110">Если ресурс распространяется, каждый учащийся получит копию этого ресурса в списке ресурсов их отправки.</span><span class="sxs-lookup"><span data-stu-id="2b249-110">If the resource is distributed, each student will receive a copy of this resource in the resource list of their submission.</span></span> <span data-ttu-id="2b249-111">Каждый студент сможет изменить свою копию и отправит их для ступенчатого.</span><span class="sxs-lookup"><span data-stu-id="2b249-111">Each student will be able to modify their copy and submit it for grading.</span></span>


## <a name="methods"></a><span data-ttu-id="2b249-112">Методы</span><span class="sxs-lookup"><span data-stu-id="2b249-112">Methods</span></span>

| <span data-ttu-id="2b249-113">Метод</span><span class="sxs-lookup"><span data-stu-id="2b249-113">Method</span></span>           | <span data-ttu-id="2b249-114">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="2b249-114">Return Type</span></span>    |<span data-ttu-id="2b249-115">Описание</span><span class="sxs-lookup"><span data-stu-id="2b249-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2b249-116">Получение Едукатионассигнментресаурце</span><span class="sxs-lookup"><span data-stu-id="2b249-116">Get educationAssignmentResource</span></span>](../api/educationassignmentresource-get.md) | [<span data-ttu-id="2b249-117">Едукатионассигнментресаурце</span><span class="sxs-lookup"><span data-stu-id="2b249-117">educationAssignmentResource</span></span>](educationassignmentresource.md) |<span data-ttu-id="2b249-118">Чтение свойств и связей объекта **едукатионассигнментресаурце** .</span><span class="sxs-lookup"><span data-stu-id="2b249-118">Read properties and relationships of an **educationAssignmentResource** object.</span></span>|
|[<span data-ttu-id="2b249-119">Обновление</span><span class="sxs-lookup"><span data-stu-id="2b249-119">Update</span></span>](../api/educationassignmentresource-update.md) | [<span data-ttu-id="2b249-120">Едукатионассигнментресаурце</span><span class="sxs-lookup"><span data-stu-id="2b249-120">educationAssignmentResource</span></span>](educationassignmentresource.md) |<span data-ttu-id="2b249-121">Обновление объекта **едукатионассигнментресаурце** .</span><span class="sxs-lookup"><span data-stu-id="2b249-121">Update an **educationAssignmentResource** object.</span></span> |
|[<span data-ttu-id="2b249-122">Удаление</span><span class="sxs-lookup"><span data-stu-id="2b249-122">Delete</span></span>](../api/educationassignmentresource-delete.md) | <span data-ttu-id="2b249-123">Нет</span><span class="sxs-lookup"><span data-stu-id="2b249-123">None</span></span> |<span data-ttu-id="2b249-124">Удаление объекта **едукатионассигнментресаурце** .</span><span class="sxs-lookup"><span data-stu-id="2b249-124">Delete an **educationAssignmentResource** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="2b249-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="2b249-125">Properties</span></span>
| <span data-ttu-id="2b249-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="2b249-126">Property</span></span>     | <span data-ttu-id="2b249-127">Тип</span><span class="sxs-lookup"><span data-stu-id="2b249-127">Type</span></span>   |<span data-ttu-id="2b249-128">Описание</span><span class="sxs-lookup"><span data-stu-id="2b249-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2b249-129">Дистрибутефорстудентворк</span><span class="sxs-lookup"><span data-stu-id="2b249-129">distributeForStudentWork</span></span>|<span data-ttu-id="2b249-130">Логический</span><span class="sxs-lookup"><span data-stu-id="2b249-130">Boolean</span></span>|<span data-ttu-id="2b249-131">Указывает, следует ли копировать этот ресурс в каждую отправку учащегося для изменения и отправки.</span><span class="sxs-lookup"><span data-stu-id="2b249-131">Indicates whether this resource should be copied to each student submission for modification and submission.</span></span>|
|<span data-ttu-id="2b249-132">id</span><span class="sxs-lookup"><span data-stu-id="2b249-132">id</span></span>|<span data-ttu-id="2b249-133">String</span><span class="sxs-lookup"><span data-stu-id="2b249-133">String</span></span>| <span data-ttu-id="2b249-134">ИДЕНТИФИКАТОР этого ресурса.</span><span class="sxs-lookup"><span data-stu-id="2b249-134">ID of this resource.</span></span> <span data-ttu-id="2b249-135">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2b249-135">Read-only.</span></span>|
|<span data-ttu-id="2b249-136">resource</span><span class="sxs-lookup"><span data-stu-id="2b249-136">resource</span></span>|[<span data-ttu-id="2b249-137">Едукатионресаурце</span><span class="sxs-lookup"><span data-stu-id="2b249-137">educationResource</span></span>](educationresource.md)|<span data-ttu-id="2b249-138">Объект ресурса, связанный с этим назначением.</span><span class="sxs-lookup"><span data-stu-id="2b249-138">Resource object that has been associated with this assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2b249-139">Связи</span><span class="sxs-lookup"><span data-stu-id="2b249-139">Relationships</span></span>
<span data-ttu-id="2b249-140">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="2b249-140">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="2b249-141">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="2b249-141">JSON representation</span></span>

<span data-ttu-id="2b249-142">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2b249-142">The following is a JSON representation of the resource.</span></span>

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
