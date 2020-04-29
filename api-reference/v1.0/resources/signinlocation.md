---
title: Тип ресурса signInLocation
description: Предоставляет город, область и страну или регион, из которых выполняется вход.
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 58c3dc2b25b85963e6a0f6f88552dbf2a121d5f7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446858"
---
# <a name="signinlocation-resource-type"></a><span data-ttu-id="9ce52-103">Тип ресурса signInLocation</span><span class="sxs-lookup"><span data-stu-id="9ce52-103">signInLocation resource type</span></span>

<span data-ttu-id="9ce52-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9ce52-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9ce52-105">Предоставляет город, область и страну или регион, из которых выполняется вход.</span><span class="sxs-lookup"><span data-stu-id="9ce52-105">Provides the city, state and country/region from where the sign-in happened.</span></span>

## <a name="properties"></a><span data-ttu-id="9ce52-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="9ce52-106">Properties</span></span>

| <span data-ttu-id="9ce52-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="9ce52-107">Property</span></span>     | <span data-ttu-id="9ce52-108">Тип</span><span class="sxs-lookup"><span data-stu-id="9ce52-108">Type</span></span>   |<span data-ttu-id="9ce52-109">Описание</span><span class="sxs-lookup"><span data-stu-id="9ce52-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9ce52-110">city</span><span class="sxs-lookup"><span data-stu-id="9ce52-110">city</span></span>|<span data-ttu-id="9ce52-111">String</span><span class="sxs-lookup"><span data-stu-id="9ce52-111">String</span></span>|<span data-ttu-id="9ce52-112">Предоставляет город, в котором поступил вход.</span><span class="sxs-lookup"><span data-stu-id="9ce52-112">Provides the city where the sign-in originated.</span></span> <span data-ttu-id="9ce52-113">Рассчитывается с использованием информации о широте и долготе из действия, выполняемого при входе.</span><span class="sxs-lookup"><span data-stu-id="9ce52-113">This is calculated using latitude/longitude information from the sign-in activity.</span></span>|
|<span data-ttu-id="9ce52-114">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="9ce52-114">countryOrRegion</span></span>|<span data-ttu-id="9ce52-115">String</span><span class="sxs-lookup"><span data-stu-id="9ce52-115">String</span></span>|<span data-ttu-id="9ce52-116">Предоставляет сведения о коде страны (код из 2 букв), где поступил вход.</span><span class="sxs-lookup"><span data-stu-id="9ce52-116">Provides the country code info (2 letter code) where the sign-in originated.</span></span>  <span data-ttu-id="9ce52-117">Рассчитывается с использованием информации о широте и долготе из действия, выполняемого при входе.</span><span class="sxs-lookup"><span data-stu-id="9ce52-117">This is calculated using latitude/longitude information from the sign-in activity.</span></span>|
|<span data-ttu-id="9ce52-118">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="9ce52-118">geoCoordinates</span></span>|[<span data-ttu-id="9ce52-119">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="9ce52-119">geoCoordinates</span></span>](geocoordinates.md)|<span data-ttu-id="9ce52-120">Предоставляет широту, долготу и высоту, на которой поступил вход.</span><span class="sxs-lookup"><span data-stu-id="9ce52-120">Provides the latitude, longitude and altitude where the sign-in originated.</span></span>|
|<span data-ttu-id="9ce52-121">state</span><span class="sxs-lookup"><span data-stu-id="9ce52-121">state</span></span>|<span data-ttu-id="9ce52-122">String</span><span class="sxs-lookup"><span data-stu-id="9ce52-122">String</span></span>|<span data-ttu-id="9ce52-123">Предоставляет состояние, в котором поступил вход.</span><span class="sxs-lookup"><span data-stu-id="9ce52-123">Provides the State where the sign-in originated.</span></span> <span data-ttu-id="9ce52-124">Рассчитывается с использованием информации о широте и долготе из действия, выполняемого при входе.</span><span class="sxs-lookup"><span data-stu-id="9ce52-124">This is calculated using latitude/longitude information from the sign-in activity.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9ce52-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9ce52-125">JSON representation</span></span>

<span data-ttu-id="9ce52-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9ce52-126">Here is a JSON representation of the resource.</span></span>

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
