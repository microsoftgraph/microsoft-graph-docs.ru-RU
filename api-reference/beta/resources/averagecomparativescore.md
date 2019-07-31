---
title: " Тип ресурса Аверажекомпаративескоре"
description: Этот ресурс содержит различные показатели, основанные на разных областях (например, усреднение по отраслевым вертикали, среднее значение по размеру компании и т. д.) и категории элементов управления (идентификация, данные, устройство, приложения, инфраструктура).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 3e2256e7edefd0670bb697ec6d89c9fb80a5beeb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013152"
---
#  <a name="averagecomparativescore-resource-type"></a><span data-ttu-id="b3047-103">Тип ресурса Аверажекомпаративескоре</span><span class="sxs-lookup"><span data-stu-id="b3047-103">averageComparativeScore resource type</span></span>

<span data-ttu-id="b3047-104">Этот ресурс содержит различные показатели, основанные на разных областях (например, усреднение по отраслевым вертикали, среднее значение по размеру компании и т. д.) и категории элементов управления (идентификация, данные, устройство, приложения, инфраструктура).</span><span class="sxs-lookup"><span data-stu-id="b3047-104">This resource contains various different scores based by different scopes (for example, average by industry vertical, average by company seat size, and so on) and control category (Identity, Data, Device, Apps, Infrastructure).</span></span>

|<span data-ttu-id="b3047-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="b3047-105">Property</span></span> |<span data-ttu-id="b3047-106">Тип</span><span class="sxs-lookup"><span data-stu-id="b3047-106">Type</span></span> |<span data-ttu-id="b3047-107">Описание</span><span class="sxs-lookup"><span data-stu-id="b3047-107">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="b3047-108">бы</span><span class="sxs-lookup"><span data-stu-id="b3047-108">basis</span></span>   |   <span data-ttu-id="b3047-109">String</span><span class="sxs-lookup"><span data-stu-id="b3047-109">String</span></span>  |   <span data-ttu-id="b3047-110">Тип области (по Аллтенантс, Тоталсеатс, Индустритипес).</span><span class="sxs-lookup"><span data-stu-id="b3047-110">Scope type (By AllTenants, TotalSeats, IndustryTypes).</span></span>  |
|   <span data-ttu-id="b3047-111">Аверажескоре</span><span class="sxs-lookup"><span data-stu-id="b3047-111">averageScore</span></span>    |   <span data-ttu-id="b3047-112">Двойное</span><span class="sxs-lookup"><span data-stu-id="b3047-112">Double</span></span>  | <span data-ttu-id="b3047-113">Средняя оценка в указанном базисе.</span><span class="sxs-lookup"><span data-stu-id="b3047-113">Average score within specified basis.</span></span> |
|   <span data-ttu-id="b3047-114">Девицескоре</span><span class="sxs-lookup"><span data-stu-id="b3047-114">deviceScore</span></span> |   <span data-ttu-id="b3047-115">Двойное</span><span class="sxs-lookup"><span data-stu-id="b3047-115">Double</span></span>  | <span data-ttu-id="b3047-116">Средняя оценка в указанном базисе.</span><span class="sxs-lookup"><span data-stu-id="b3047-116">Average score within specified basis.</span></span> |
|   <span data-ttu-id="b3047-117">Score</span><span class="sxs-lookup"><span data-stu-id="b3047-117">dataScore</span></span>   |   <span data-ttu-id="b3047-118">Двойное</span><span class="sxs-lookup"><span data-stu-id="b3047-118">Double</span></span>  | <span data-ttu-id="b3047-119">Средняя оценка в указанном базисе.</span><span class="sxs-lookup"><span data-stu-id="b3047-119">Average score within specified basis.</span></span> |
|   <span data-ttu-id="b3047-120">Идентитискоре</span><span class="sxs-lookup"><span data-stu-id="b3047-120">identityScore</span></span>   |   <span data-ttu-id="b3047-121">Двойное</span><span class="sxs-lookup"><span data-stu-id="b3047-121">Double</span></span>  | <span data-ttu-id="b3047-122">Средняя оценка в указанном базисе.</span><span class="sxs-lookup"><span data-stu-id="b3047-122">Average score within specified basis.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b3047-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b3047-123">JSON representation</span></span>

<span data-ttu-id="b3047-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b3047-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.averageComparativeScore"
}-->

```json
{
  "basis": "String",
  "averageScore": "Double",
  "deviceScore": "Double",
  "dataScore": "Double",
  "identityScore": "Double"
}

```


<!-- {
  "type": "#page.annotation",
  "description": "averageComparativeScore resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
