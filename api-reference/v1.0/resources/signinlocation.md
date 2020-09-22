---
title: Тип ресурса signInLocation
description: Предоставляет город, область и страну или регион, из которых выполняется вход.
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4b14f26fff4721da499d108883f57db009ec42c3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47970609"
---
# <a name="signinlocation-resource-type"></a><span data-ttu-id="47c47-103">Тип ресурса signInLocation</span><span class="sxs-lookup"><span data-stu-id="47c47-103">signInLocation resource type</span></span>

<span data-ttu-id="47c47-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="47c47-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="47c47-105">Предоставляет город, область и страну или регион, из которых выполняется вход.</span><span class="sxs-lookup"><span data-stu-id="47c47-105">Provides the city, state and country/region from where the sign-in happened.</span></span>

## <a name="properties"></a><span data-ttu-id="47c47-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="47c47-106">Properties</span></span>

| <span data-ttu-id="47c47-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="47c47-107">Property</span></span>     | <span data-ttu-id="47c47-108">Тип</span><span class="sxs-lookup"><span data-stu-id="47c47-108">Type</span></span>   |<span data-ttu-id="47c47-109">Описание</span><span class="sxs-lookup"><span data-stu-id="47c47-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="47c47-110">city</span><span class="sxs-lookup"><span data-stu-id="47c47-110">city</span></span>|<span data-ttu-id="47c47-111">String</span><span class="sxs-lookup"><span data-stu-id="47c47-111">String</span></span>|<span data-ttu-id="47c47-112">Предоставляет город, в котором поступил вход.</span><span class="sxs-lookup"><span data-stu-id="47c47-112">Provides the city where the sign-in originated.</span></span> <span data-ttu-id="47c47-113">Рассчитывается с использованием информации о широте и долготе из действия, выполняемого при входе.</span><span class="sxs-lookup"><span data-stu-id="47c47-113">This is calculated using latitude/longitude information from the sign-in activity.</span></span>|
|<span data-ttu-id="47c47-114">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="47c47-114">countryOrRegion</span></span>|<span data-ttu-id="47c47-115">String</span><span class="sxs-lookup"><span data-stu-id="47c47-115">String</span></span>|<span data-ttu-id="47c47-116">Предоставляет сведения о коде страны (код из 2 букв), где поступил вход.</span><span class="sxs-lookup"><span data-stu-id="47c47-116">Provides the country code info (2 letter code) where the sign-in originated.</span></span>  <span data-ttu-id="47c47-117">Рассчитывается с использованием информации о широте и долготе из действия, выполняемого при входе.</span><span class="sxs-lookup"><span data-stu-id="47c47-117">This is calculated using latitude/longitude information from the sign-in activity.</span></span>|
|<span data-ttu-id="47c47-118">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="47c47-118">geoCoordinates</span></span>|[<span data-ttu-id="47c47-119">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="47c47-119">geoCoordinates</span></span>](geocoordinates.md)|<span data-ttu-id="47c47-120">Предоставляет широту, долготу и высоту, на которой поступил вход.</span><span class="sxs-lookup"><span data-stu-id="47c47-120">Provides the latitude, longitude and altitude where the sign-in originated.</span></span>|
|<span data-ttu-id="47c47-121">state</span><span class="sxs-lookup"><span data-stu-id="47c47-121">state</span></span>|<span data-ttu-id="47c47-122">String</span><span class="sxs-lookup"><span data-stu-id="47c47-122">String</span></span>|<span data-ttu-id="47c47-123">Предоставляет состояние, в котором поступил вход.</span><span class="sxs-lookup"><span data-stu-id="47c47-123">Provides the State where the sign-in originated.</span></span> <span data-ttu-id="47c47-124">Рассчитывается с использованием информации о широте и долготе из действия, выполняемого при входе.</span><span class="sxs-lookup"><span data-stu-id="47c47-124">This is calculated using latitude/longitude information from the sign-in activity.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="47c47-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="47c47-125">JSON representation</span></span>

<span data-ttu-id="47c47-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="47c47-126">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.signInLocation"
}-->

```json
{
  "city": "String",
  "countryOrRegion": "String",
  "geoCoordinates": {"@odata.type": "microsoft.graph.geoCoordinates"},
  "state": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "signInLocation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

