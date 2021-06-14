---
title: тип ресурса educationRubric
description: Рубрика классификации, которую можно прикрепить к назначению.
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: f70fded2c35576d31f3c5b17edf0342d97a88302
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912853"
---
# <a name="educationrubric-resource-type"></a><span data-ttu-id="99b48-103">тип ресурса educationRubric</span><span class="sxs-lookup"><span data-stu-id="99b48-103">educationRubric resource type</span></span>

<span data-ttu-id="99b48-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="99b48-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="99b48-105">Рубрика классификации, которую можно прикрепить к назначению.</span><span class="sxs-lookup"><span data-stu-id="99b48-105">A grading rubric that can be attached to an assignment.</span></span> <span data-ttu-id="99b48-106">Рубрика связана с **educationUser** (учителем) и присоединена к одному или более ресурсам **educationAssignment.**</span><span class="sxs-lookup"><span data-stu-id="99b48-106">A rubric is associated with an **educationUser** (teacher), and attached to one or more **educationAssignment** resources.</span></span> 

<span data-ttu-id="99b48-107">Дополнительные [сведения см. в рубрике Образование.](/graph/education-rubric-overview)</span><span class="sxs-lookup"><span data-stu-id="99b48-107">See [Education rubric overview](/graph/education-rubric-overview) for more information.</span></span>

## <a name="methods"></a><span data-ttu-id="99b48-108">Методы</span><span class="sxs-lookup"><span data-stu-id="99b48-108">Methods</span></span>

| <span data-ttu-id="99b48-109">Метод</span><span class="sxs-lookup"><span data-stu-id="99b48-109">Method</span></span>       | <span data-ttu-id="99b48-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="99b48-110">Return Type</span></span> | <span data-ttu-id="99b48-111">Описание</span><span class="sxs-lookup"><span data-stu-id="99b48-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="99b48-112">Создание educationRubric</span><span class="sxs-lookup"><span data-stu-id="99b48-112">Create educationRubric</span></span>](../api/educationuser-post-rubrics.md) | [<span data-ttu-id="99b48-113">educationRubric</span><span class="sxs-lookup"><span data-stu-id="99b48-113">educationRubric</span></span>](educationrubric.md) | <span data-ttu-id="99b48-114">Создайте новый объект educationRubric.</span><span class="sxs-lookup"><span data-stu-id="99b48-114">Create a new educationRubric object.</span></span> |
| [<span data-ttu-id="99b48-115">Get educationRubric</span><span class="sxs-lookup"><span data-stu-id="99b48-115">Get educationRubric</span></span>](../api/educationrubric-get.md) | [<span data-ttu-id="99b48-116">educationRubric</span><span class="sxs-lookup"><span data-stu-id="99b48-116">educationRubric</span></span>](educationrubric.md) | <span data-ttu-id="99b48-117">Чтение свойств и связей объекта educationRubric.</span><span class="sxs-lookup"><span data-stu-id="99b48-117">Read properties and relationships of educationRubric object.</span></span> |
| [<span data-ttu-id="99b48-118">Обновление educationRubric</span><span class="sxs-lookup"><span data-stu-id="99b48-118">Update educationRubric</span></span>](../api/educationrubric-update.md) | [<span data-ttu-id="99b48-119">educationRubric</span><span class="sxs-lookup"><span data-stu-id="99b48-119">educationRubric</span></span>](educationrubric.md) | <span data-ttu-id="99b48-120">Обновление объекта educationRubric.</span><span class="sxs-lookup"><span data-stu-id="99b48-120">Update educationRubric object.</span></span> |
| [<span data-ttu-id="99b48-121">Удаление educationRubric</span><span class="sxs-lookup"><span data-stu-id="99b48-121">Delete educationRubric</span></span>](../api/educationrubric-delete.md) | <span data-ttu-id="99b48-122">Нет</span><span class="sxs-lookup"><span data-stu-id="99b48-122">None</span></span> | <span data-ttu-id="99b48-123">Удаление объекта educationRubric.</span><span class="sxs-lookup"><span data-stu-id="99b48-123">Delete educationRubric object.</span></span> |

## <a name="properties"></a><span data-ttu-id="99b48-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="99b48-124">Properties</span></span>

| <span data-ttu-id="99b48-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="99b48-125">Property</span></span>     | <span data-ttu-id="99b48-126">Тип</span><span class="sxs-lookup"><span data-stu-id="99b48-126">Type</span></span>        | <span data-ttu-id="99b48-127">Описание</span><span class="sxs-lookup"><span data-stu-id="99b48-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="99b48-128">createdBy</span><span class="sxs-lookup"><span data-stu-id="99b48-128">createdBy</span></span>|[<span data-ttu-id="99b48-129">identitySet</span><span class="sxs-lookup"><span data-stu-id="99b48-129">identitySet</span></span>](identityset.md)|<span data-ttu-id="99b48-130">Пользователь, создавший этот ресурс.</span><span class="sxs-lookup"><span data-stu-id="99b48-130">The user who created this resource.</span></span>|
|<span data-ttu-id="99b48-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="99b48-131">createdDateTime</span></span>|<span data-ttu-id="99b48-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99b48-132">DateTimeOffset</span></span>|<span data-ttu-id="99b48-133">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="99b48-133">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="99b48-134">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="99b48-134">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="99b48-135">description</span><span class="sxs-lookup"><span data-stu-id="99b48-135">description</span></span>|[<span data-ttu-id="99b48-136">itemBody</span><span class="sxs-lookup"><span data-stu-id="99b48-136">itemBody</span></span>](itembody.md)|<span data-ttu-id="99b48-137">Описание этой рубрики.</span><span class="sxs-lookup"><span data-stu-id="99b48-137">The description of this rubric.</span></span>|
|<span data-ttu-id="99b48-138">displayName</span><span class="sxs-lookup"><span data-stu-id="99b48-138">displayName</span></span>|<span data-ttu-id="99b48-139">String</span><span class="sxs-lookup"><span data-stu-id="99b48-139">String</span></span>|<span data-ttu-id="99b48-140">Название этой рубрики.</span><span class="sxs-lookup"><span data-stu-id="99b48-140">The name of this rubric.</span></span>|
|<span data-ttu-id="99b48-141">классификация</span><span class="sxs-lookup"><span data-stu-id="99b48-141">grading</span></span>|[<span data-ttu-id="99b48-142">educationAssignmentGradeType</span><span class="sxs-lookup"><span data-stu-id="99b48-142">educationAssignmentGradeType</span></span>](educationassignmentgradetype.md)|<span data-ttu-id="99b48-143">Тип классификации этой рубрики — null для неочковой рубрики или [educationAssignmentPointsGradeType](educationassignmentpointsgradetype.md) для рубрики точек.</span><span class="sxs-lookup"><span data-stu-id="99b48-143">The grading type of this rubric -- null for a no-points rubric, or [educationAssignmentPointsGradeType](educationassignmentpointsgradetype.md) for a points rubric.</span></span>|
|<span data-ttu-id="99b48-144">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="99b48-144">lastModifiedBy</span></span>|[<span data-ttu-id="99b48-145">identitySet</span><span class="sxs-lookup"><span data-stu-id="99b48-145">identitySet</span></span>](identityset.md)|<span data-ttu-id="99b48-146">Последний пользователь, который изменит ресурс.</span><span class="sxs-lookup"><span data-stu-id="99b48-146">The last user to modify the resource.</span></span>|
|<span data-ttu-id="99b48-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="99b48-147">lastModifiedDateTime</span></span>|<span data-ttu-id="99b48-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99b48-148">DateTimeOffset</span></span>|<span data-ttu-id="99b48-149">Время последнего изменения ресурса.</span><span class="sxs-lookup"><span data-stu-id="99b48-149">Moment in time when the resource was last modified.</span></span>  <span data-ttu-id="99b48-150">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="99b48-150">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="99b48-151">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="99b48-151">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="99b48-152">уровни</span><span class="sxs-lookup"><span data-stu-id="99b48-152">levels</span></span>|<span data-ttu-id="99b48-153">[коллекция rubricLevel](rubriclevel.md)</span><span class="sxs-lookup"><span data-stu-id="99b48-153">[rubricLevel](rubriclevel.md) collection</span></span>|<span data-ttu-id="99b48-154">Коллекция уровней, в которые состоит эта рубрика.</span><span class="sxs-lookup"><span data-stu-id="99b48-154">The collection of levels making up this rubric.</span></span>|
|<span data-ttu-id="99b48-155">качества</span><span class="sxs-lookup"><span data-stu-id="99b48-155">qualities</span></span>|<span data-ttu-id="99b48-156">[rubricQuality](rubricquality.md) collection</span><span class="sxs-lookup"><span data-stu-id="99b48-156">[rubricQuality](rubricquality.md) collection</span></span>|<span data-ttu-id="99b48-157">Коллекция качеств, из которых состоит эта рубрика.</span><span class="sxs-lookup"><span data-stu-id="99b48-157">The collection of qualities making up this rubric.</span></span>|

## <a name="relationships"></a><span data-ttu-id="99b48-158">Связи</span><span class="sxs-lookup"><span data-stu-id="99b48-158">Relationships</span></span>

<span data-ttu-id="99b48-159">Нет</span><span class="sxs-lookup"><span data-stu-id="99b48-159">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="99b48-160">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="99b48-160">JSON representation</span></span>

<span data-ttu-id="99b48-161">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="99b48-161">The following is a JSON representation of the resource.</span></span>

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