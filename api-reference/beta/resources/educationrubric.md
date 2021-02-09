---
title: Тип ресурса educationRubric
description: Рубрика ограды, которую можно прикрепить к назначению
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 37e1d4a6267f1f1292a72cc7f34b8135483091ec
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161938"
---
# <a name="educationrubric-resource-type"></a><span data-ttu-id="147f9-103">Тип ресурса educationRubric</span><span class="sxs-lookup"><span data-stu-id="147f9-103">educationRubric resource type</span></span>

<span data-ttu-id="147f9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="147f9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="147f9-105">Рубрика ограды, которую можно прикрепить к назначению.</span><span class="sxs-lookup"><span data-stu-id="147f9-105">A grading rubric that can be attached to an assignment.</span></span> <span data-ttu-id="147f9-106">Рубрика связана с **educationUser** (преподавателем) и прикреплена к одному или более **ресурсам educationAssignment.**</span><span class="sxs-lookup"><span data-stu-id="147f9-106">A rubric is associated with an **educationUser** (teacher), and attached to one or more **educationAssignment** resources.</span></span> 

<span data-ttu-id="147f9-107">Дополнительные [сведения см. в обзоре рубрики для](/graph/education-rubric-overview) образования.</span><span class="sxs-lookup"><span data-stu-id="147f9-107">See [Education rubric overview](/graph/education-rubric-overview) for more information.</span></span>

## <a name="methods"></a><span data-ttu-id="147f9-108">Методы</span><span class="sxs-lookup"><span data-stu-id="147f9-108">Methods</span></span>

| <span data-ttu-id="147f9-109">Метод</span><span class="sxs-lookup"><span data-stu-id="147f9-109">Method</span></span>       | <span data-ttu-id="147f9-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="147f9-110">Return Type</span></span> | <span data-ttu-id="147f9-111">Описание</span><span class="sxs-lookup"><span data-stu-id="147f9-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="147f9-112">Создание educationRubric</span><span class="sxs-lookup"><span data-stu-id="147f9-112">Create educationRubric</span></span>](../api/educationuser-post-rubrics.md) | [<span data-ttu-id="147f9-113">educationRubric</span><span class="sxs-lookup"><span data-stu-id="147f9-113">educationRubric</span></span>](educationrubric.md) | <span data-ttu-id="147f9-114">Создание объекта educationRubric.</span><span class="sxs-lookup"><span data-stu-id="147f9-114">Create a new educationRubric object.</span></span> |
| [<span data-ttu-id="147f9-115">Get educationRubric</span><span class="sxs-lookup"><span data-stu-id="147f9-115">Get educationRubric</span></span>](../api/educationrubric-get.md) | [<span data-ttu-id="147f9-116">educationRubric</span><span class="sxs-lookup"><span data-stu-id="147f9-116">educationRubric</span></span>](educationrubric.md) | <span data-ttu-id="147f9-117">Чтение свойств и связей объекта educationRubric.</span><span class="sxs-lookup"><span data-stu-id="147f9-117">Read properties and relationships of educationRubric object.</span></span> |
| [<span data-ttu-id="147f9-118">Обновление educationRubric</span><span class="sxs-lookup"><span data-stu-id="147f9-118">Update educationRubric</span></span>](../api/educationrubric-update.md) | [<span data-ttu-id="147f9-119">educationRubric</span><span class="sxs-lookup"><span data-stu-id="147f9-119">educationRubric</span></span>](educationrubric.md) | <span data-ttu-id="147f9-120">Обновление объекта educationRubric.</span><span class="sxs-lookup"><span data-stu-id="147f9-120">Update educationRubric object.</span></span> |
| [<span data-ttu-id="147f9-121">Удаление educationRubric</span><span class="sxs-lookup"><span data-stu-id="147f9-121">Delete educationRubric</span></span>](../api/educationrubric-delete.md) | <span data-ttu-id="147f9-122">Нет</span><span class="sxs-lookup"><span data-stu-id="147f9-122">None</span></span> | <span data-ttu-id="147f9-123">Удаление объекта educationRubric.</span><span class="sxs-lookup"><span data-stu-id="147f9-123">Delete educationRubric object.</span></span> |

## <a name="properties"></a><span data-ttu-id="147f9-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="147f9-124">Properties</span></span>

| <span data-ttu-id="147f9-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="147f9-125">Property</span></span>     | <span data-ttu-id="147f9-126">Тип</span><span class="sxs-lookup"><span data-stu-id="147f9-126">Type</span></span>        | <span data-ttu-id="147f9-127">Описание</span><span class="sxs-lookup"><span data-stu-id="147f9-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="147f9-128">createdBy</span><span class="sxs-lookup"><span data-stu-id="147f9-128">createdBy</span></span>|[<span data-ttu-id="147f9-129">identitySet</span><span class="sxs-lookup"><span data-stu-id="147f9-129">identitySet</span></span>](identityset.md)|<span data-ttu-id="147f9-130">Пользователь, создавший этот ресурс.</span><span class="sxs-lookup"><span data-stu-id="147f9-130">The user who created this resource.</span></span>|
|<span data-ttu-id="147f9-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="147f9-131">createdDateTime</span></span>|<span data-ttu-id="147f9-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="147f9-132">DateTimeOffset</span></span>|<span data-ttu-id="147f9-p102">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="147f9-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="147f9-135">(описание)</span><span class="sxs-lookup"><span data-stu-id="147f9-135">description</span></span>|[<span data-ttu-id="147f9-136">itemBody</span><span class="sxs-lookup"><span data-stu-id="147f9-136">itemBody</span></span>](itembody.md)|<span data-ttu-id="147f9-137">Описание этой рубрики.</span><span class="sxs-lookup"><span data-stu-id="147f9-137">The description of this rubric.</span></span>|
|<span data-ttu-id="147f9-138">displayName</span><span class="sxs-lookup"><span data-stu-id="147f9-138">displayName</span></span>|<span data-ttu-id="147f9-139">String</span><span class="sxs-lookup"><span data-stu-id="147f9-139">String</span></span>|<span data-ttu-id="147f9-140">Имя этой рубрики.</span><span class="sxs-lookup"><span data-stu-id="147f9-140">The name of this rubric.</span></span>|
|<span data-ttu-id="147f9-141">grading</span><span class="sxs-lookup"><span data-stu-id="147f9-141">grading</span></span>|[<span data-ttu-id="147f9-142">educationAssignmentGradeType</span><span class="sxs-lookup"><span data-stu-id="147f9-142">educationAssignmentGradeType</span></span>](educationassignmentgradetype.md)|<span data-ttu-id="147f9-143">Тип классификации этой рубрики — null для рубрики без пунктов или [educationAssignmentPointsGradeType](educationassignmentpointsgradetype.md) для рубрики точек.</span><span class="sxs-lookup"><span data-stu-id="147f9-143">The grading type of this rubric -- null for a no-points rubric, or [educationAssignmentPointsGradeType](educationassignmentpointsgradetype.md) for a points rubric.</span></span>|
|<span data-ttu-id="147f9-144">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="147f9-144">lastModifiedBy</span></span>|[<span data-ttu-id="147f9-145">identitySet</span><span class="sxs-lookup"><span data-stu-id="147f9-145">identitySet</span></span>](identityset.md)|<span data-ttu-id="147f9-146">Последний пользователь, который изменял ресурс.</span><span class="sxs-lookup"><span data-stu-id="147f9-146">The last user to modify the resource.</span></span>|
|<span data-ttu-id="147f9-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="147f9-147">lastModifiedDateTime</span></span>|<span data-ttu-id="147f9-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="147f9-148">DateTimeOffset</span></span>|<span data-ttu-id="147f9-149">Время последнего изменения ресурса.</span><span class="sxs-lookup"><span data-stu-id="147f9-149">Moment in time when the resource was last modified.</span></span>  <span data-ttu-id="147f9-150">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="147f9-150">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="147f9-151">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="147f9-151">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="147f9-152">levels</span><span class="sxs-lookup"><span data-stu-id="147f9-152">levels</span></span>|<span data-ttu-id="147f9-153">[Коллекция rubricLevel](rubriclevel.md)</span><span class="sxs-lookup"><span data-stu-id="147f9-153">[rubricLevel](rubriclevel.md) collection</span></span>|<span data-ttu-id="147f9-154">Коллекция уровней, которые составляет эта рубрика.</span><span class="sxs-lookup"><span data-stu-id="147f9-154">The collection of levels making up this rubric.</span></span>|
|<span data-ttu-id="147f9-155">qualities</span><span class="sxs-lookup"><span data-stu-id="147f9-155">qualities</span></span>|<span data-ttu-id="147f9-156">[Коллекция rubricQuality](rubricquality.md)</span><span class="sxs-lookup"><span data-stu-id="147f9-156">[rubricQuality](rubricquality.md) collection</span></span>|<span data-ttu-id="147f9-157">Коллекция качеств, из которых состоит эта рубрика.</span><span class="sxs-lookup"><span data-stu-id="147f9-157">The collection of qualities making up this rubric.</span></span>|

## <a name="relationships"></a><span data-ttu-id="147f9-158">Связи</span><span class="sxs-lookup"><span data-stu-id="147f9-158">Relationships</span></span>

<span data-ttu-id="147f9-159">Нет</span><span class="sxs-lookup"><span data-stu-id="147f9-159">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="147f9-160">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="147f9-160">JSON representation</span></span>

<span data-ttu-id="147f9-161">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="147f9-161">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationRubric",
  "keyProperty": "id"
}-->

```json
{
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "description": {"@odata.type": "microsoft.graph.itemBody"},
  "displayName": "String",
  "grading": {"@odata.type": "microsoft.graph.educationAssignmentGradeType"},
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "levels": [{"@odata.type": "microsoft.graph.rubricLevel"}],
  "qualities": [{"@odata.type": "microsoft.graph.rubricQuality"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationRubric resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->