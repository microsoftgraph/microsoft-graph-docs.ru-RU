---
title: Тип ресурса Едукатионрубрик
description: Rubricа, который можно прикрепить к назначению
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 6c448652719f20ab2edd7c283ea18e99a37edbbd
ms.sourcegitcommit: fc818699566f03493937be95447eb9f656a1f950
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42534435"
---
# <a name="educationrubric-resource-type"></a><span data-ttu-id="37346-103">Тип ресурса Едукатионрубрик</span><span class="sxs-lookup"><span data-stu-id="37346-103">educationRubric resource type</span></span>

<span data-ttu-id="37346-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="37346-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="37346-105">Rubricа, который можно прикрепить к назначению.</span><span class="sxs-lookup"><span data-stu-id="37346-105">A grading rubric that can be attached to an assignment.</span></span> <span data-ttu-id="37346-106">Rubric связан с **educationUser** (преподавателем) и подключен к одному или нескольким ресурсам **educationAssignment** .</span><span class="sxs-lookup"><span data-stu-id="37346-106">A rubric is associated with an **educationUser** (teacher), and attached to one or more **educationAssignment** resources.</span></span> 

<span data-ttu-id="37346-107">Более подробную информацию вы найдете в статье [образование Rubric Overview](https://developer.microsoft.com/graph/docs/concepts/education-rubric-overview) .</span><span class="sxs-lookup"><span data-stu-id="37346-107">See [Education rubric overview](https://developer.microsoft.com/graph/docs/concepts/education-rubric-overview) for more information.</span></span>

## <a name="methods"></a><span data-ttu-id="37346-108">Методы</span><span class="sxs-lookup"><span data-stu-id="37346-108">Methods</span></span>

| <span data-ttu-id="37346-109">Метод</span><span class="sxs-lookup"><span data-stu-id="37346-109">Method</span></span>       | <span data-ttu-id="37346-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="37346-110">Return Type</span></span> | <span data-ttu-id="37346-111">Описание</span><span class="sxs-lookup"><span data-stu-id="37346-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="37346-112">Создание Едукатионрубрик</span><span class="sxs-lookup"><span data-stu-id="37346-112">Create educationRubric</span></span>](../api/educationuser-post-rubrics.md) | [<span data-ttu-id="37346-113">едукатионрубрик</span><span class="sxs-lookup"><span data-stu-id="37346-113">educationRubric</span></span>](educationrubric.md) | <span data-ttu-id="37346-114">Создание нового объекта Едукатионрубрик.</span><span class="sxs-lookup"><span data-stu-id="37346-114">Create a new educationRubric object.</span></span> |
| [<span data-ttu-id="37346-115">Получение Едукатионрубрик</span><span class="sxs-lookup"><span data-stu-id="37346-115">Get educationRubric</span></span>](../api/educationrubric-get.md) | [<span data-ttu-id="37346-116">едукатионрубрик</span><span class="sxs-lookup"><span data-stu-id="37346-116">educationRubric</span></span>](educationrubric.md) | <span data-ttu-id="37346-117">Чтение свойств и связей объекта Едукатионрубрик.</span><span class="sxs-lookup"><span data-stu-id="37346-117">Read properties and relationships of educationRubric object.</span></span> |
| [<span data-ttu-id="37346-118">Обновление Едукатионрубрик</span><span class="sxs-lookup"><span data-stu-id="37346-118">Update educationRubric</span></span>](../api/educationrubric-update.md) | [<span data-ttu-id="37346-119">едукатионрубрик</span><span class="sxs-lookup"><span data-stu-id="37346-119">educationRubric</span></span>](educationrubric.md) | <span data-ttu-id="37346-120">Обновление объекта Едукатионрубрик.</span><span class="sxs-lookup"><span data-stu-id="37346-120">Update educationRubric object.</span></span> |
| [<span data-ttu-id="37346-121">Удаление Едукатионрубрик</span><span class="sxs-lookup"><span data-stu-id="37346-121">Delete educationRubric</span></span>](../api/educationrubric-delete.md) | <span data-ttu-id="37346-122">Нет</span><span class="sxs-lookup"><span data-stu-id="37346-122">None</span></span> | <span data-ttu-id="37346-123">Удаление объекта Едукатионрубрик.</span><span class="sxs-lookup"><span data-stu-id="37346-123">Delete educationRubric object.</span></span> |

## <a name="properties"></a><span data-ttu-id="37346-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="37346-124">Properties</span></span>

| <span data-ttu-id="37346-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="37346-125">Property</span></span>     | <span data-ttu-id="37346-126">Тип</span><span class="sxs-lookup"><span data-stu-id="37346-126">Type</span></span>        | <span data-ttu-id="37346-127">Описание</span><span class="sxs-lookup"><span data-stu-id="37346-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="37346-128">createdBy</span><span class="sxs-lookup"><span data-stu-id="37346-128">createdBy</span></span>|[<span data-ttu-id="37346-129">identitySet</span><span class="sxs-lookup"><span data-stu-id="37346-129">identitySet</span></span>](identityset.md)|<span data-ttu-id="37346-130">Пользователь, создавший этот ресурс.</span><span class="sxs-lookup"><span data-stu-id="37346-130">The user who created this resource.</span></span>|
|<span data-ttu-id="37346-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="37346-131">createdDateTime</span></span>|<span data-ttu-id="37346-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="37346-132">DateTimeOffset</span></span>|<span data-ttu-id="37346-p102">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="37346-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="37346-135">description</span><span class="sxs-lookup"><span data-stu-id="37346-135">description</span></span>|[<span data-ttu-id="37346-136">itemBody</span><span class="sxs-lookup"><span data-stu-id="37346-136">itemBody</span></span>](itembody.md)|<span data-ttu-id="37346-137">Описание этого Rubric.</span><span class="sxs-lookup"><span data-stu-id="37346-137">The description of this rubric.</span></span>|
|<span data-ttu-id="37346-138">displayName</span><span class="sxs-lookup"><span data-stu-id="37346-138">displayName</span></span>|<span data-ttu-id="37346-139">String</span><span class="sxs-lookup"><span data-stu-id="37346-139">String</span></span>|<span data-ttu-id="37346-140">Имя этого Rubric.</span><span class="sxs-lookup"><span data-stu-id="37346-140">The name of this rubric.</span></span>|
|<span data-ttu-id="37346-141">снижения</span><span class="sxs-lookup"><span data-stu-id="37346-141">grading</span></span>|[<span data-ttu-id="37346-142">едукатионассигнментградетипе</span><span class="sxs-lookup"><span data-stu-id="37346-142">educationAssignmentGradeType</span></span>](educationassignmentgradetype.md)|<span data-ttu-id="37346-143">Тип ступенчатости этого Rubric — NULL для нулевых точек Rubric или [едукатионассигнментпоинтсградетипе](educationassignmentpointsgradetype.md) для точек Rubric.</span><span class="sxs-lookup"><span data-stu-id="37346-143">The grading type of this rubric -- null for a no-points rubric, or [educationAssignmentPointsGradeType](educationassignmentpointsgradetype.md) for a points rubric.</span></span>|
|<span data-ttu-id="37346-144">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="37346-144">lastModifiedBy</span></span>|[<span data-ttu-id="37346-145">identitySet</span><span class="sxs-lookup"><span data-stu-id="37346-145">identitySet</span></span>](identityset.md)|<span data-ttu-id="37346-146">Последний пользователь для изменения ресурса.</span><span class="sxs-lookup"><span data-stu-id="37346-146">The last user to modify the resource.</span></span>|
|<span data-ttu-id="37346-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="37346-147">lastModifiedDateTime</span></span>|<span data-ttu-id="37346-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="37346-148">DateTimeOffset</span></span>|<span data-ttu-id="37346-149">Момент времени последнего изменения ресурса.</span><span class="sxs-lookup"><span data-stu-id="37346-149">Moment in time when the resource was last modified.</span></span>  <span data-ttu-id="37346-150">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="37346-150">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="37346-151">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="37346-151">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="37346-152">тонов</span><span class="sxs-lookup"><span data-stu-id="37346-152">levels</span></span>|<span data-ttu-id="37346-153">Коллекция [рубриклевел](rubriclevel.md)</span><span class="sxs-lookup"><span data-stu-id="37346-153">[rubricLevel](rubriclevel.md) collection</span></span>|<span data-ttu-id="37346-154">Коллекция уровней, составляющих данный Rubric.</span><span class="sxs-lookup"><span data-stu-id="37346-154">The collection of levels making up this rubric.</span></span>|
|<span data-ttu-id="37346-155">являются</span><span class="sxs-lookup"><span data-stu-id="37346-155">qualities</span></span>|<span data-ttu-id="37346-156">Коллекция [рубриккуалити](rubricquality.md)</span><span class="sxs-lookup"><span data-stu-id="37346-156">[rubricQuality](rubricquality.md) collection</span></span>|<span data-ttu-id="37346-157">Коллекция качеств, составляющих этот Rubric.</span><span class="sxs-lookup"><span data-stu-id="37346-157">The collection of qualities making up this rubric.</span></span>|

## <a name="relationships"></a><span data-ttu-id="37346-158">Связи</span><span class="sxs-lookup"><span data-stu-id="37346-158">Relationships</span></span>

<span data-ttu-id="37346-159">Нет</span><span class="sxs-lookup"><span data-stu-id="37346-159">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="37346-160">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="37346-160">JSON representation</span></span>

<span data-ttu-id="37346-161">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="37346-161">The following is a JSON representation of the resource.</span></span>

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
