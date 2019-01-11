---
title: " Тип ресурса averageComparativeScore"
description: Этот ресурс содержит различные различных показателям на основе, различные области (например, среднее число по вертикали отрасли, Средний размер рабочее место компании и т. п.) и элемент управления категории (удостоверения, данные, устройства, приложения, инфраструктуры).
localization_priority: Normal
ms.openlocfilehash: c32c1349edd70e80c1bf0fb12a36bd07e06ed39f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834596"
---
#  <a name="averagecomparativescore-resource-type"></a><span data-ttu-id="ada5b-103">Тип ресурса averageComparativeScore</span><span class="sxs-lookup"><span data-stu-id="ada5b-103">averageComparativeScore resource type</span></span>

<span data-ttu-id="ada5b-104">Этот ресурс содержит различные различных показателям на основе, различные области (например, среднее число по вертикали отрасли, Средний размер рабочее место компании и т. п.) и элемент управления категории (удостоверения, данные, устройства, приложения, инфраструктуры).</span><span class="sxs-lookup"><span data-stu-id="ada5b-104">This resource contains various different scores based by different scopes (for example, average by industry vertical, average by company seat size, and so on) and control category (Identity, Data, Device, Apps, Infrastructure).</span></span>

|<span data-ttu-id="ada5b-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="ada5b-105">Property</span></span> |<span data-ttu-id="ada5b-106">Тип</span><span class="sxs-lookup"><span data-stu-id="ada5b-106">Type</span></span> |<span data-ttu-id="ada5b-107">Описание</span><span class="sxs-lookup"><span data-stu-id="ada5b-107">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="ada5b-108">Основы</span><span class="sxs-lookup"><span data-stu-id="ada5b-108">basis</span></span>   |   <span data-ttu-id="ada5b-109">Строка</span><span class="sxs-lookup"><span data-stu-id="ada5b-109">String</span></span>  |   <span data-ttu-id="ada5b-110">Тип области (с AllTenants, Общее_число_мест, IndustryTypes).</span><span class="sxs-lookup"><span data-stu-id="ada5b-110">Scope type (By AllTenants, TotalSeats, IndustryTypes).</span></span>  |
|   <span data-ttu-id="ada5b-111">«СреднийБалл»</span><span class="sxs-lookup"><span data-stu-id="ada5b-111">averageScore</span></span>    |   <span data-ttu-id="ada5b-112">Double</span><span class="sxs-lookup"><span data-stu-id="ada5b-112">Double</span></span>  | <span data-ttu-id="ada5b-113">Средняя оценка в рамках указанного основы.</span><span class="sxs-lookup"><span data-stu-id="ada5b-113">Average score within specified basis.</span></span> |
|   <span data-ttu-id="ada5b-114">deviceScore</span><span class="sxs-lookup"><span data-stu-id="ada5b-114">deviceScore</span></span> |   <span data-ttu-id="ada5b-115">Double</span><span class="sxs-lookup"><span data-stu-id="ada5b-115">Double</span></span>  | <span data-ttu-id="ada5b-116">Средняя оценка в рамках указанного основы.</span><span class="sxs-lookup"><span data-stu-id="ada5b-116">Average score within specified basis.</span></span> |
|   <span data-ttu-id="ada5b-117">dataScore</span><span class="sxs-lookup"><span data-stu-id="ada5b-117">dataScore</span></span>   |   <span data-ttu-id="ada5b-118">Double</span><span class="sxs-lookup"><span data-stu-id="ada5b-118">Double</span></span>  | <span data-ttu-id="ada5b-119">Средняя оценка в рамках указанного основы.</span><span class="sxs-lookup"><span data-stu-id="ada5b-119">Average score within specified basis.</span></span> |
|   <span data-ttu-id="ada5b-120">identityScore</span><span class="sxs-lookup"><span data-stu-id="ada5b-120">identityScore</span></span>   |   <span data-ttu-id="ada5b-121">Double</span><span class="sxs-lookup"><span data-stu-id="ada5b-121">Double</span></span>  | <span data-ttu-id="ada5b-122">Средняя оценка в рамках указанного основы.</span><span class="sxs-lookup"><span data-stu-id="ada5b-122">Average score within specified basis.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ada5b-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ada5b-123">JSON representation</span></span>

<span data-ttu-id="ada5b-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ada5b-124">The following is a JSON representation of the resource.</span></span>

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
