---
title: " Тип ресурса Аверажекомпаративескоре"
description: Этот ресурс содержит различные показатели, основанные на разных областях (например, усреднение по отраслевым вертикали, среднее значение по размеру компании и т. д.) и категории элементов управления (идентификация, данные, устройство, приложения, инфраструктура).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: f2ac965d4dae0b038f3aad9fe13ed57a283a42bc
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812557"
---
#  <a name="averagecomparativescore-resource-type"></a><span data-ttu-id="93b83-103">Тип ресурса Аверажекомпаративескоре</span><span class="sxs-lookup"><span data-stu-id="93b83-103">averageComparativeScore resource type</span></span>

<span data-ttu-id="93b83-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="93b83-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="93b83-105">Этот ресурс содержит различные показатели, основанные на разных областях (например, усреднение по отраслевым вертикали, среднее значение по размеру компании и т. д.) и категории элементов управления (идентификация, данные, устройство, приложения, инфраструктура).</span><span class="sxs-lookup"><span data-stu-id="93b83-105">This resource contains various different scores based by different scopes (for example, average by industry vertical, average by company seat size, and so on) and control category (Identity, Data, Device, Apps, Infrastructure).</span></span>

|<span data-ttu-id="93b83-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="93b83-106">Property</span></span> |<span data-ttu-id="93b83-107">Тип</span><span class="sxs-lookup"><span data-stu-id="93b83-107">Type</span></span> |<span data-ttu-id="93b83-108">Описание</span><span class="sxs-lookup"><span data-stu-id="93b83-108">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="93b83-109">бы</span><span class="sxs-lookup"><span data-stu-id="93b83-109">basis</span></span>   |   <span data-ttu-id="93b83-110">String</span><span class="sxs-lookup"><span data-stu-id="93b83-110">String</span></span>  |   <span data-ttu-id="93b83-111">Тип области (по Аллтенантс, Тоталсеатс, Индустритипес).</span><span class="sxs-lookup"><span data-stu-id="93b83-111">Scope type (By AllTenants, TotalSeats, IndustryTypes).</span></span>  |
|   <span data-ttu-id="93b83-112">аверажескоре</span><span class="sxs-lookup"><span data-stu-id="93b83-112">averageScore</span></span>    |   <span data-ttu-id="93b83-113">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="93b83-113">Double</span></span>  | <span data-ttu-id="93b83-114">Средняя оценка в указанном базисе.</span><span class="sxs-lookup"><span data-stu-id="93b83-114">Average score within specified basis.</span></span> |
|   <span data-ttu-id="93b83-115">девицескоре</span><span class="sxs-lookup"><span data-stu-id="93b83-115">deviceScore</span></span> |   <span data-ttu-id="93b83-116">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="93b83-116">Double</span></span>  | <span data-ttu-id="93b83-117">Средняя оценка в указанном базисе.</span><span class="sxs-lookup"><span data-stu-id="93b83-117">Average score within specified basis.</span></span> |
|   <span data-ttu-id="93b83-118">Score</span><span class="sxs-lookup"><span data-stu-id="93b83-118">dataScore</span></span>   |   <span data-ttu-id="93b83-119">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="93b83-119">Double</span></span>  | <span data-ttu-id="93b83-120">Средняя оценка в указанном базисе.</span><span class="sxs-lookup"><span data-stu-id="93b83-120">Average score within specified basis.</span></span> |
|   <span data-ttu-id="93b83-121">идентитискоре</span><span class="sxs-lookup"><span data-stu-id="93b83-121">identityScore</span></span>   |   <span data-ttu-id="93b83-122">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="93b83-122">Double</span></span>  | <span data-ttu-id="93b83-123">Средняя оценка в указанном базисе.</span><span class="sxs-lookup"><span data-stu-id="93b83-123">Average score within specified basis.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="93b83-124">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="93b83-124">JSON representation</span></span>

<span data-ttu-id="93b83-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="93b83-125">The following is a JSON representation of the resource.</span></span>

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
