---
title: " Тип ресурса averageComparativeScore"
description: Этот ресурс содержит различные различных показателям на основе, различные области (например, среднее число по вертикали отрасли, Средний размер рабочее место компании и т. п.) и элемент управления категории (удостоверения, данные, устройства, приложения, инфраструктуры).
ms.openlocfilehash: 08e4ec60788b21476d8f1491ab5548c7a4ca2e01
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076110"
---
#  <a name="averagecomparativescore-resource-type"></a><span data-ttu-id="f4c65-103">Тип ресурса averageComparativeScore</span><span class="sxs-lookup"><span data-stu-id="f4c65-103">averageComparativeScore resource type</span></span>

<span data-ttu-id="f4c65-104">Этот ресурс содержит различные различных показателям на основе, различные области (например, среднее число по вертикали отрасли, Средний размер рабочее место компании и т. п.) и элемент управления категории (удостоверения, данные, устройства, приложения, инфраструктуры).</span><span class="sxs-lookup"><span data-stu-id="f4c65-104">This resource contains various different scores based by different scopes (for example, average by industry vertical, average by company seat size, and so on) and control category (Identity, Data, Device, Apps, Infrastructure).</span></span>

|<span data-ttu-id="f4c65-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="f4c65-105">Property</span></span> |<span data-ttu-id="f4c65-106">Тип</span><span class="sxs-lookup"><span data-stu-id="f4c65-106">Type</span></span> |<span data-ttu-id="f4c65-107">Description</span><span class="sxs-lookup"><span data-stu-id="f4c65-107">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="f4c65-108">Основы</span><span class="sxs-lookup"><span data-stu-id="f4c65-108">basis</span></span>   |   <span data-ttu-id="f4c65-109">String</span><span class="sxs-lookup"><span data-stu-id="f4c65-109">String</span></span>  |   <span data-ttu-id="f4c65-110">Тип области (с AllTenants, Общее_число_мест, IndustryTypes).</span><span class="sxs-lookup"><span data-stu-id="f4c65-110">Scope type (By AllTenants, TotalSeats, IndustryTypes).</span></span>  |
|   <span data-ttu-id="f4c65-111">«СреднийБалл»</span><span class="sxs-lookup"><span data-stu-id="f4c65-111">averageScore</span></span>    |   <span data-ttu-id="f4c65-112">Double</span><span class="sxs-lookup"><span data-stu-id="f4c65-112">Double</span></span>  | <span data-ttu-id="f4c65-113">Средняя оценка в рамках указанного основы.</span><span class="sxs-lookup"><span data-stu-id="f4c65-113">Average score within specified basis.</span></span> |
|   <span data-ttu-id="f4c65-114">deviceScore</span><span class="sxs-lookup"><span data-stu-id="f4c65-114">deviceScore</span></span> |   <span data-ttu-id="f4c65-115">Double</span><span class="sxs-lookup"><span data-stu-id="f4c65-115">Double</span></span>  | <span data-ttu-id="f4c65-116">Средняя оценка в рамках указанного основы.</span><span class="sxs-lookup"><span data-stu-id="f4c65-116">Average score within specified basis.</span></span> |
|   <span data-ttu-id="f4c65-117">dataScore</span><span class="sxs-lookup"><span data-stu-id="f4c65-117">dataScore</span></span>   |   <span data-ttu-id="f4c65-118">Double</span><span class="sxs-lookup"><span data-stu-id="f4c65-118">Double</span></span>  | <span data-ttu-id="f4c65-119">Средняя оценка в рамках указанного основы.</span><span class="sxs-lookup"><span data-stu-id="f4c65-119">Average score within specified basis.</span></span> |
|   <span data-ttu-id="f4c65-120">identityScore</span><span class="sxs-lookup"><span data-stu-id="f4c65-120">identityScore</span></span>   |   <span data-ttu-id="f4c65-121">Double</span><span class="sxs-lookup"><span data-stu-id="f4c65-121">Double</span></span>  | <span data-ttu-id="f4c65-122">Средняя оценка в рамках указанного основы.</span><span class="sxs-lookup"><span data-stu-id="f4c65-122">Average score within specified basis.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f4c65-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f4c65-123">JSON representation</span></span>

<span data-ttu-id="f4c65-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f4c65-124">The following is a JSON representation of the resource.</span></span>

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
