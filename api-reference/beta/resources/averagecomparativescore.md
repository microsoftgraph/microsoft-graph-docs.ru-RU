---
title: " Тип ресурса Аверажекомпаративескоре"
description: Этот ресурс содержит различные показатели, основанные на разных областях (например, усреднение по отраслевым вертикали, среднее значение по размеру компании и т. д.) и категории элементов управления (идентификация, данные, устройство, приложения, инфраструктура).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: e051ee3d1265c1dc65a5ab0cb9352d9cd536b21c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508054"
---
#  <a name="averagecomparativescore-resource-type"></a><span data-ttu-id="73872-103">Тип ресурса Аверажекомпаративескоре</span><span class="sxs-lookup"><span data-stu-id="73872-103">averageComparativeScore resource type</span></span>

<span data-ttu-id="73872-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="73872-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="73872-105">Этот ресурс содержит различные показатели, основанные на разных областях (например, усреднение по отраслевым вертикали, среднее значение по размеру компании и т. д.) и категории элементов управления (идентификация, данные, устройство, приложения, инфраструктура).</span><span class="sxs-lookup"><span data-stu-id="73872-105">This resource contains various different scores based by different scopes (for example, average by industry vertical, average by company seat size, and so on) and control category (Identity, Data, Device, Apps, Infrastructure).</span></span>

|<span data-ttu-id="73872-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="73872-106">Property</span></span> |<span data-ttu-id="73872-107">Тип</span><span class="sxs-lookup"><span data-stu-id="73872-107">Type</span></span> |<span data-ttu-id="73872-108">Описание</span><span class="sxs-lookup"><span data-stu-id="73872-108">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="73872-109">бы</span><span class="sxs-lookup"><span data-stu-id="73872-109">basis</span></span>   |   <span data-ttu-id="73872-110">String</span><span class="sxs-lookup"><span data-stu-id="73872-110">String</span></span>  |   <span data-ttu-id="73872-111">Тип области (по Аллтенантс, Тоталсеатс, Индустритипес).</span><span class="sxs-lookup"><span data-stu-id="73872-111">Scope type (By AllTenants, TotalSeats, IndustryTypes).</span></span>  |
|   <span data-ttu-id="73872-112">аверажескоре</span><span class="sxs-lookup"><span data-stu-id="73872-112">averageScore</span></span>    |   <span data-ttu-id="73872-113">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="73872-113">Double</span></span>  | <span data-ttu-id="73872-114">Средняя оценка в указанном базисе.</span><span class="sxs-lookup"><span data-stu-id="73872-114">Average score within specified basis.</span></span> |
|   <span data-ttu-id="73872-115">девицескоре</span><span class="sxs-lookup"><span data-stu-id="73872-115">deviceScore</span></span> |   <span data-ttu-id="73872-116">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="73872-116">Double</span></span>  | <span data-ttu-id="73872-117">Средняя оценка в указанном базисе.</span><span class="sxs-lookup"><span data-stu-id="73872-117">Average score within specified basis.</span></span> |
|   <span data-ttu-id="73872-118">Score</span><span class="sxs-lookup"><span data-stu-id="73872-118">dataScore</span></span>   |   <span data-ttu-id="73872-119">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="73872-119">Double</span></span>  | <span data-ttu-id="73872-120">Средняя оценка в указанном базисе.</span><span class="sxs-lookup"><span data-stu-id="73872-120">Average score within specified basis.</span></span> |
|   <span data-ttu-id="73872-121">идентитискоре</span><span class="sxs-lookup"><span data-stu-id="73872-121">identityScore</span></span>   |   <span data-ttu-id="73872-122">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="73872-122">Double</span></span>  | <span data-ttu-id="73872-123">Средняя оценка в указанном базисе.</span><span class="sxs-lookup"><span data-stu-id="73872-123">Average score within specified basis.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="73872-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="73872-124">JSON representation</span></span>

<span data-ttu-id="73872-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="73872-125">The following is a JSON representation of the resource.</span></span>

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
