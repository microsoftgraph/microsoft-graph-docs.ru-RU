---
title: " Тип ресурса Аверажекомпаративескоре"
description: Этот ресурс содержит различные показатели, основанные на разных областях (например, усреднение по отраслевым вертикали, среднее значение по размеру компании и т. д.) и категории элементов управления (идентификация, данные, устройство, приложения, инфраструктура).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: 69a9e63960499fb50b34cd38986b1312a4313090
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48076486"
---
#  <a name="averagecomparativescore-resource-type"></a><span data-ttu-id="18613-103">Тип ресурса Аверажекомпаративескоре</span><span class="sxs-lookup"><span data-stu-id="18613-103">averageComparativeScore resource type</span></span>

<span data-ttu-id="18613-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18613-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="18613-105">Этот ресурс содержит различные показатели, основанные на разных областях (например, усреднение по отраслевым вертикали, среднее значение по размеру компании и т. д.) и категории элементов управления (идентификация, данные, устройство, приложения, инфраструктура).</span><span class="sxs-lookup"><span data-stu-id="18613-105">This resource contains various different scores based by different scopes (for example, average by industry vertical, average by company seat size, and so on) and control category (Identity, Data, Device, Apps, Infrastructure).</span></span>

|<span data-ttu-id="18613-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="18613-106">Property</span></span> |<span data-ttu-id="18613-107">Тип</span><span class="sxs-lookup"><span data-stu-id="18613-107">Type</span></span> |<span data-ttu-id="18613-108">Описание</span><span class="sxs-lookup"><span data-stu-id="18613-108">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="18613-109">бы</span><span class="sxs-lookup"><span data-stu-id="18613-109">basis</span></span>   |   <span data-ttu-id="18613-110">String</span><span class="sxs-lookup"><span data-stu-id="18613-110">String</span></span>  |   <span data-ttu-id="18613-111">Тип области (по Аллтенантс, Тоталсеатс, Индустритипес).</span><span class="sxs-lookup"><span data-stu-id="18613-111">Scope type (By AllTenants, TotalSeats, IndustryTypes).</span></span>  |
|   <span data-ttu-id="18613-112">аверажескоре</span><span class="sxs-lookup"><span data-stu-id="18613-112">averageScore</span></span>    |   <span data-ttu-id="18613-113">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="18613-113">Double</span></span>  | <span data-ttu-id="18613-114">Средняя оценка в указанном базисе.</span><span class="sxs-lookup"><span data-stu-id="18613-114">Average score within specified basis.</span></span> |
|   <span data-ttu-id="18613-115">девицескоре</span><span class="sxs-lookup"><span data-stu-id="18613-115">deviceScore</span></span> |   <span data-ttu-id="18613-116">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="18613-116">Double</span></span>  | <span data-ttu-id="18613-117">Средняя оценка в указанном базисе.</span><span class="sxs-lookup"><span data-stu-id="18613-117">Average score within specified basis.</span></span> |
|   <span data-ttu-id="18613-118">Score</span><span class="sxs-lookup"><span data-stu-id="18613-118">dataScore</span></span>   |   <span data-ttu-id="18613-119">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="18613-119">Double</span></span>  | <span data-ttu-id="18613-120">Средняя оценка в указанном базисе.</span><span class="sxs-lookup"><span data-stu-id="18613-120">Average score within specified basis.</span></span> |
|   <span data-ttu-id="18613-121">идентитискоре</span><span class="sxs-lookup"><span data-stu-id="18613-121">identityScore</span></span>   |   <span data-ttu-id="18613-122">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="18613-122">Double</span></span>  | <span data-ttu-id="18613-123">Средняя оценка в указанном базисе.</span><span class="sxs-lookup"><span data-stu-id="18613-123">Average score within specified basis.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="18613-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="18613-124">JSON representation</span></span>

<span data-ttu-id="18613-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="18613-125">The following is a JSON representation of the resource.</span></span>

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


