---
title: Тип ресурса Едукатионпоинтсауткоме
description: Объект Едукатионауткоме, который дает числовой уровень
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 12e288e49fffd3cf385111878483408b5c6610c1
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173246"
---
# <a name="educationpointsoutcome-resource-type"></a><span data-ttu-id="17e23-103">Тип ресурса Едукатионпоинтсауткоме</span><span class="sxs-lookup"><span data-stu-id="17e23-103">educationPointsOutcome resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="17e23-104">[Едукатионауткоме](educationoutcome.md) , который предоставляет числовой уровень.</span><span class="sxs-lookup"><span data-stu-id="17e23-104">An [educationOutcome](educationoutcome.md) that gives a numerical grade.</span></span>

## <a name="methods"></a><span data-ttu-id="17e23-105">Методы</span><span class="sxs-lookup"><span data-stu-id="17e23-105">Methods</span></span>

| <span data-ttu-id="17e23-106">Метод</span><span class="sxs-lookup"><span data-stu-id="17e23-106">Method</span></span>       | <span data-ttu-id="17e23-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="17e23-107">Return Type</span></span> | <span data-ttu-id="17e23-108">Описание</span><span class="sxs-lookup"><span data-stu-id="17e23-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="17e23-109">Обновление Едукатионауткоме</span><span class="sxs-lookup"><span data-stu-id="17e23-109">Update educationOutcome</span></span>](../api/educationoutcome-update.md) | [<span data-ttu-id="17e23-110">Едукатионауткоме</span><span class="sxs-lookup"><span data-stu-id="17e23-110">educationOutcome</span></span>](educationoutcome.md) | <span data-ttu-id="17e23-111">Обновление объекта Едукатионауткоме.</span><span class="sxs-lookup"><span data-stu-id="17e23-111">Update educationOutcome object.</span></span> |

## <a name="properties"></a><span data-ttu-id="17e23-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="17e23-112">Properties</span></span>

| <span data-ttu-id="17e23-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="17e23-113">Property</span></span>     | <span data-ttu-id="17e23-114">Тип</span><span class="sxs-lookup"><span data-stu-id="17e23-114">Type</span></span>        | <span data-ttu-id="17e23-115">Описание</span><span class="sxs-lookup"><span data-stu-id="17e23-115">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="17e23-116">points</span><span class="sxs-lookup"><span data-stu-id="17e23-116">points</span></span>|[<span data-ttu-id="17e23-117">Едукатионассигнментпоинтсграде</span><span class="sxs-lookup"><span data-stu-id="17e23-117">educationAssignmentPointsGrade</span></span>](educationassignmentpointsgrade.md)|<span data-ttu-id="17e23-118">Числовое значение, которое преподаватель приделил студенту для этого назначения.</span><span class="sxs-lookup"><span data-stu-id="17e23-118">The numeric grade the teacher has given the student for this assignment.</span></span>|
|<span data-ttu-id="17e23-119">Публишедпоинтс</span><span class="sxs-lookup"><span data-stu-id="17e23-119">publishedPoints</span></span>|[<span data-ttu-id="17e23-120">Едукатионассигнментпоинтсграде</span><span class="sxs-lookup"><span data-stu-id="17e23-120">educationAssignmentPointsGrade</span></span>](educationassignmentpointsgrade.md)|<span data-ttu-id="17e23-121">Копия свойства Points, которое устанавливается при отпадении уровня на учащийся.</span><span class="sxs-lookup"><span data-stu-id="17e23-121">A copy of the points property that is made when the grade is released to the student.</span></span>|

## <a name="relationships"></a><span data-ttu-id="17e23-122">Отношения</span><span class="sxs-lookup"><span data-stu-id="17e23-122">Relationships</span></span>

<span data-ttu-id="17e23-123">Нет</span><span class="sxs-lookup"><span data-stu-id="17e23-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="17e23-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="17e23-124">JSON representation</span></span>

<span data-ttu-id="17e23-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="17e23-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationPointsOutcome",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "points": {"@odata.type": "microsoft.graph.educationAssignmentPointsGrade"},
  "publishedPoints": {"@odata.type": "microsoft.graph.educationAssignmentPointsGrade"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationPointsOutcome resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->