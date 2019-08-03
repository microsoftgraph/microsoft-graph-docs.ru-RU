---
title: Тип ресурса Едукатионрубрик
description: Rubricа, который можно прикрепить к назначению
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: b43b611465af4dabb62d9dd741eb9a8670f241b9
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173239"
---
# <a name="educationrubric-resource-type"></a><span data-ttu-id="14641-103">Тип ресурса Едукатионрубрик</span><span class="sxs-lookup"><span data-stu-id="14641-103">educationRubric resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="14641-104">Rubricа, который можно прикрепить к назначению.</span><span class="sxs-lookup"><span data-stu-id="14641-104">A grading rubric that can be attached to an assignment.</span></span> <span data-ttu-id="14641-105">Rubric связан с **educationUser** (преподавателем) и подключен к одному или нескольким ресурсам **educationAssignment** .</span><span class="sxs-lookup"><span data-stu-id="14641-105">A rubric is associated with an **educationUser** (teacher), and attached to one or more **educationAssignment** resources.</span></span> 

<span data-ttu-id="14641-106">Более подробную информацию вы найдете в статье [образование Rubric Overview](https://developer.microsoft.com/graph/docs/concepts/education-rubric-overview) .</span><span class="sxs-lookup"><span data-stu-id="14641-106">See [Education rubric overview](https://developer.microsoft.com/graph/docs/concepts/education-rubric-overview) for more information.</span></span>

## <a name="methods"></a><span data-ttu-id="14641-107">Методы</span><span class="sxs-lookup"><span data-stu-id="14641-107">Methods</span></span>

| <span data-ttu-id="14641-108">Метод</span><span class="sxs-lookup"><span data-stu-id="14641-108">Method</span></span>       | <span data-ttu-id="14641-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="14641-109">Return Type</span></span> | <span data-ttu-id="14641-110">Описание</span><span class="sxs-lookup"><span data-stu-id="14641-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="14641-111">Получение Едукатионрубрик</span><span class="sxs-lookup"><span data-stu-id="14641-111">Get educationRubric</span></span>](../api/educationrubric-get.md) | [<span data-ttu-id="14641-112">Едукатионрубрик</span><span class="sxs-lookup"><span data-stu-id="14641-112">educationRubric</span></span>](educationrubric.md) | <span data-ttu-id="14641-113">Чтение свойств и связей объекта Едукатионрубрик.</span><span class="sxs-lookup"><span data-stu-id="14641-113">Read properties and relationships of educationRubric object.</span></span> |
| [<span data-ttu-id="14641-114">Обновление Едукатионрубрик</span><span class="sxs-lookup"><span data-stu-id="14641-114">Update educationRubric</span></span>](../api/educationrubric-update.md) | [<span data-ttu-id="14641-115">Едукатионрубрик</span><span class="sxs-lookup"><span data-stu-id="14641-115">educationRubric</span></span>](educationrubric.md) | <span data-ttu-id="14641-116">Обновление объекта Едукатионрубрик.</span><span class="sxs-lookup"><span data-stu-id="14641-116">Update educationRubric object.</span></span> |
| [<span data-ttu-id="14641-117">Удаление Едукатионрубрик</span><span class="sxs-lookup"><span data-stu-id="14641-117">Delete educationRubric</span></span>](../api/educationrubric-delete.md) | <span data-ttu-id="14641-118">Нет</span><span class="sxs-lookup"><span data-stu-id="14641-118">None</span></span> | <span data-ttu-id="14641-119">Удаление объекта Едукатионрубрик.</span><span class="sxs-lookup"><span data-stu-id="14641-119">Delete educationRubric object.</span></span> |

## <a name="properties"></a><span data-ttu-id="14641-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="14641-120">Properties</span></span>

| <span data-ttu-id="14641-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="14641-121">Property</span></span>     | <span data-ttu-id="14641-122">Тип</span><span class="sxs-lookup"><span data-stu-id="14641-122">Type</span></span>        | <span data-ttu-id="14641-123">Описание</span><span class="sxs-lookup"><span data-stu-id="14641-123">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="14641-124">createdBy</span><span class="sxs-lookup"><span data-stu-id="14641-124">createdBy</span></span>|[<span data-ttu-id="14641-125">identitySet</span><span class="sxs-lookup"><span data-stu-id="14641-125">identitySet</span></span>](identityset.md)|<span data-ttu-id="14641-126">Пользователь, создавший этот ресурс.</span><span class="sxs-lookup"><span data-stu-id="14641-126">The user who created this resource.</span></span>|
|<span data-ttu-id="14641-127">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="14641-127">createdDateTime</span></span>|<span data-ttu-id="14641-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="14641-128">DateTimeOffset</span></span>|<span data-ttu-id="14641-p102">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="14641-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="14641-131">description</span><span class="sxs-lookup"><span data-stu-id="14641-131">description</span></span>|[<span data-ttu-id="14641-132">itemBody</span><span class="sxs-lookup"><span data-stu-id="14641-132">itemBody</span></span>](itembody.md)|<span data-ttu-id="14641-133">Описание этого Rubric.</span><span class="sxs-lookup"><span data-stu-id="14641-133">The description of this rubric.</span></span>|
|<span data-ttu-id="14641-134">displayName</span><span class="sxs-lookup"><span data-stu-id="14641-134">displayName</span></span>|<span data-ttu-id="14641-135">String</span><span class="sxs-lookup"><span data-stu-id="14641-135">String</span></span>|<span data-ttu-id="14641-136">Имя этого Rubric.</span><span class="sxs-lookup"><span data-stu-id="14641-136">The name of this rubric.</span></span>|
|<span data-ttu-id="14641-137">снижения</span><span class="sxs-lookup"><span data-stu-id="14641-137">grading</span></span>|[<span data-ttu-id="14641-138">Едукатионассигнментградетипе</span><span class="sxs-lookup"><span data-stu-id="14641-138">educationAssignmentGradeType</span></span>](educationassignmentgradetype.md)|<span data-ttu-id="14641-139">Тип ступенчатости этого Rubric — NULL для нулевых точек Rubric или [едукатионассигнментпоинтсградетипе](educationassignmentpointsgradetype.md) для точек Rubric.</span><span class="sxs-lookup"><span data-stu-id="14641-139">The grading type of this rubric -- null for a no-points rubric, or [educationAssignmentPointsGradeType](educationassignmentpointsgradetype.md) for a points rubric.</span></span>|
|<span data-ttu-id="14641-140">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="14641-140">lastModifiedBy</span></span>|[<span data-ttu-id="14641-141">identitySet</span><span class="sxs-lookup"><span data-stu-id="14641-141">identitySet</span></span>](identityset.md)|<span data-ttu-id="14641-142">Последний пользователь для изменения ресурса.</span><span class="sxs-lookup"><span data-stu-id="14641-142">The last user to modify the resource.</span></span>|
|<span data-ttu-id="14641-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="14641-143">lastModifiedDateTime</span></span>|<span data-ttu-id="14641-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="14641-144">DateTimeOffset</span></span>|<span data-ttu-id="14641-145">Момент времени последнего изменения ресурса.</span><span class="sxs-lookup"><span data-stu-id="14641-145">Moment in time when the resource was last modified.</span></span>  <span data-ttu-id="14641-146">Тип Timestamp представляет сведения о дате и времени с использованием формата ISO 8601, причем всегда используется время в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="14641-146">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="14641-147">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="14641-147">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="14641-148">тонов</span><span class="sxs-lookup"><span data-stu-id="14641-148">levels</span></span>|<span data-ttu-id="14641-149">Коллекция [рубриклевел](rubriclevel.md)</span><span class="sxs-lookup"><span data-stu-id="14641-149">[rubricLevel](rubriclevel.md) collection</span></span>|<span data-ttu-id="14641-150">Коллекция уровней, составляющих данный Rubric.</span><span class="sxs-lookup"><span data-stu-id="14641-150">The collection of levels making up this rubric.</span></span>|
|<span data-ttu-id="14641-151">являются</span><span class="sxs-lookup"><span data-stu-id="14641-151">qualities</span></span>|<span data-ttu-id="14641-152">Коллекция [рубриккуалити](rubricquality.md)</span><span class="sxs-lookup"><span data-stu-id="14641-152">[rubricQuality](rubricquality.md) collection</span></span>|<span data-ttu-id="14641-153">Коллекция качеств, составляющих этот Rubric.</span><span class="sxs-lookup"><span data-stu-id="14641-153">The collection of qualities making up this rubric.</span></span>|

## <a name="relationships"></a><span data-ttu-id="14641-154">Отношения</span><span class="sxs-lookup"><span data-stu-id="14641-154">Relationships</span></span>

<span data-ttu-id="14641-155">Нет</span><span class="sxs-lookup"><span data-stu-id="14641-155">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="14641-156">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="14641-156">JSON representation</span></span>

<span data-ttu-id="14641-157">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="14641-157">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationRubric",
  "baseType": "",
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