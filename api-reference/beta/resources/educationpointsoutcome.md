---
title: Тип ресурса Едукатионпоинтсауткоме
description: Объект Едукатионауткоме, который дает числовой уровень
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 51f57683e06f90e877b4cd72e62d0898d0ef8013
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42501432"
---
# <a name="educationpointsoutcome-resource-type"></a><span data-ttu-id="22eb9-103">Тип ресурса Едукатионпоинтсауткоме</span><span class="sxs-lookup"><span data-stu-id="22eb9-103">educationPointsOutcome resource type</span></span>

<span data-ttu-id="22eb9-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="22eb9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="22eb9-105">[Едукатионауткоме](educationoutcome.md) , который предоставляет числовой уровень.</span><span class="sxs-lookup"><span data-stu-id="22eb9-105">An [educationOutcome](educationoutcome.md) that gives a numerical grade.</span></span>

## <a name="methods"></a><span data-ttu-id="22eb9-106">Методы</span><span class="sxs-lookup"><span data-stu-id="22eb9-106">Methods</span></span>

| <span data-ttu-id="22eb9-107">Метод</span><span class="sxs-lookup"><span data-stu-id="22eb9-107">Method</span></span>       | <span data-ttu-id="22eb9-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="22eb9-108">Return Type</span></span> | <span data-ttu-id="22eb9-109">Описание</span><span class="sxs-lookup"><span data-stu-id="22eb9-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="22eb9-110">Обновление Едукатионауткоме</span><span class="sxs-lookup"><span data-stu-id="22eb9-110">Update educationOutcome</span></span>](../api/educationoutcome-update.md) | [<span data-ttu-id="22eb9-111">едукатионауткоме</span><span class="sxs-lookup"><span data-stu-id="22eb9-111">educationOutcome</span></span>](educationoutcome.md) | <span data-ttu-id="22eb9-112">Обновление объекта Едукатионауткоме.</span><span class="sxs-lookup"><span data-stu-id="22eb9-112">Update educationOutcome object.</span></span> |

## <a name="properties"></a><span data-ttu-id="22eb9-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="22eb9-113">Properties</span></span>

| <span data-ttu-id="22eb9-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="22eb9-114">Property</span></span>     | <span data-ttu-id="22eb9-115">Тип</span><span class="sxs-lookup"><span data-stu-id="22eb9-115">Type</span></span>        | <span data-ttu-id="22eb9-116">Описание</span><span class="sxs-lookup"><span data-stu-id="22eb9-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="22eb9-117">points</span><span class="sxs-lookup"><span data-stu-id="22eb9-117">points</span></span>|[<span data-ttu-id="22eb9-118">едукатионассигнментпоинтсграде</span><span class="sxs-lookup"><span data-stu-id="22eb9-118">educationAssignmentPointsGrade</span></span>](educationassignmentpointsgrade.md)|<span data-ttu-id="22eb9-119">Числовое значение, которое преподаватель приделил студенту для этого назначения.</span><span class="sxs-lookup"><span data-stu-id="22eb9-119">The numeric grade the teacher has given the student for this assignment.</span></span>|
|<span data-ttu-id="22eb9-120">публишедпоинтс</span><span class="sxs-lookup"><span data-stu-id="22eb9-120">publishedPoints</span></span>|[<span data-ttu-id="22eb9-121">едукатионассигнментпоинтсграде</span><span class="sxs-lookup"><span data-stu-id="22eb9-121">educationAssignmentPointsGrade</span></span>](educationassignmentpointsgrade.md)|<span data-ttu-id="22eb9-122">Копия свойства Points, которое устанавливается при отпадении уровня на учащийся.</span><span class="sxs-lookup"><span data-stu-id="22eb9-122">A copy of the points property that is made when the grade is released to the student.</span></span>|

## <a name="relationships"></a><span data-ttu-id="22eb9-123">Связи</span><span class="sxs-lookup"><span data-stu-id="22eb9-123">Relationships</span></span>

<span data-ttu-id="22eb9-124">Нет</span><span class="sxs-lookup"><span data-stu-id="22eb9-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="22eb9-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="22eb9-125">JSON representation</span></span>

<span data-ttu-id="22eb9-126">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="22eb9-126">The following is a JSON representation of the resource.</span></span>

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