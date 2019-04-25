---
title: " Тип ресурса Аверажекомпаративескоре"
description: Этот ресурс содержит различные показатели, основанные на разных областях (например, усреднение по отраслевым вертикали, среднее значение по размеру компании и т. д.) и категории элементов управления (идентификация, данные, устройство, приложения, инфраструктура).
localization_priority: Normal
ms.openlocfilehash: c32c1349edd70e80c1bf0fb12a36bd07e06ed39f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535440"
---
#  <a name="averagecomparativescore-resource-type"></a><span data-ttu-id="b7870-103">Тип ресурса Аверажекомпаративескоре</span><span class="sxs-lookup"><span data-stu-id="b7870-103">averageComparativeScore resource type</span></span>

<span data-ttu-id="b7870-104">Этот ресурс содержит различные показатели, основанные на разных областях (например, усреднение по отраслевым вертикали, среднее значение по размеру компании и т. д.) и категории элементов управления (идентификация, данные, устройство, приложения, инфраструктура).</span><span class="sxs-lookup"><span data-stu-id="b7870-104">This resource contains various different scores based by different scopes (for example, average by industry vertical, average by company seat size, and so on) and control category (Identity, Data, Device, Apps, Infrastructure).</span></span>

|<span data-ttu-id="b7870-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="b7870-105">Property</span></span> |<span data-ttu-id="b7870-106">Тип</span><span class="sxs-lookup"><span data-stu-id="b7870-106">Type</span></span> |<span data-ttu-id="b7870-107">Описание</span><span class="sxs-lookup"><span data-stu-id="b7870-107">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="b7870-108">бы</span><span class="sxs-lookup"><span data-stu-id="b7870-108">basis</span></span>   |   <span data-ttu-id="b7870-109">String</span><span class="sxs-lookup"><span data-stu-id="b7870-109">String</span></span>  |   <span data-ttu-id="b7870-110">Тип области (по Аллтенантс, Тоталсеатс, Индустритипес).</span><span class="sxs-lookup"><span data-stu-id="b7870-110">Scope type (By AllTenants, TotalSeats, IndustryTypes).</span></span>  |
|   <span data-ttu-id="b7870-111">Аверажескоре</span><span class="sxs-lookup"><span data-stu-id="b7870-111">averageScore</span></span>    |   <span data-ttu-id="b7870-112">Двойное</span><span class="sxs-lookup"><span data-stu-id="b7870-112">Double</span></span>  | <span data-ttu-id="b7870-113">Средняя оценка в указанном базисе.</span><span class="sxs-lookup"><span data-stu-id="b7870-113">Average score within specified basis.</span></span> |
|   <span data-ttu-id="b7870-114">Девицескоре</span><span class="sxs-lookup"><span data-stu-id="b7870-114">deviceScore</span></span> |   <span data-ttu-id="b7870-115">Двойное</span><span class="sxs-lookup"><span data-stu-id="b7870-115">Double</span></span>  | <span data-ttu-id="b7870-116">Средняя оценка в указанном базисе.</span><span class="sxs-lookup"><span data-stu-id="b7870-116">Average score within specified basis.</span></span> |
|   <span data-ttu-id="b7870-117">Score</span><span class="sxs-lookup"><span data-stu-id="b7870-117">dataScore</span></span>   |   <span data-ttu-id="b7870-118">Двойное</span><span class="sxs-lookup"><span data-stu-id="b7870-118">Double</span></span>  | <span data-ttu-id="b7870-119">Средняя оценка в указанном базисе.</span><span class="sxs-lookup"><span data-stu-id="b7870-119">Average score within specified basis.</span></span> |
|   <span data-ttu-id="b7870-120">Идентитискоре</span><span class="sxs-lookup"><span data-stu-id="b7870-120">identityScore</span></span>   |   <span data-ttu-id="b7870-121">Двойное</span><span class="sxs-lookup"><span data-stu-id="b7870-121">Double</span></span>  | <span data-ttu-id="b7870-122">Средняя оценка в указанном базисе.</span><span class="sxs-lookup"><span data-stu-id="b7870-122">Average score within specified basis.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b7870-123">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="b7870-123">JSON representation</span></span>

<span data-ttu-id="b7870-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b7870-124">The following is a JSON representation of the resource.</span></span>

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
