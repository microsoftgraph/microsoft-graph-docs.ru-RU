---
title: Тип ресурса signInLocation
description: Предоставляет город, область и страну или регион, из которых выполняется вход.
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 35c6511b7dba69a362b44a9390974913c46b73ee
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034218"
---
# <a name="signinlocation-resource-type"></a><span data-ttu-id="7ff13-103">Тип ресурса signInLocation</span><span class="sxs-lookup"><span data-stu-id="7ff13-103">signInLocation resource type</span></span>

<span data-ttu-id="7ff13-104">Предоставляет город, область и страну или регион, из которых выполняется вход.</span><span class="sxs-lookup"><span data-stu-id="7ff13-104">Provides the city, state and country/region from where the sign-in happened.</span></span>

## <a name="properties"></a><span data-ttu-id="7ff13-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="7ff13-105">Properties</span></span>

| <span data-ttu-id="7ff13-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="7ff13-106">Property</span></span>     | <span data-ttu-id="7ff13-107">Тип</span><span class="sxs-lookup"><span data-stu-id="7ff13-107">Type</span></span>   |<span data-ttu-id="7ff13-108">Описание</span><span class="sxs-lookup"><span data-stu-id="7ff13-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7ff13-109">city</span><span class="sxs-lookup"><span data-stu-id="7ff13-109">city</span></span>|<span data-ttu-id="7ff13-110">String</span><span class="sxs-lookup"><span data-stu-id="7ff13-110">String</span></span>|<span data-ttu-id="7ff13-111">Предоставляет город, в котором поступил вход.</span><span class="sxs-lookup"><span data-stu-id="7ff13-111">Provides the city where the sign-in originated.</span></span> <span data-ttu-id="7ff13-112">Рассчитывается с использованием информации о широте и долготе из действия, выполняемого при входе.</span><span class="sxs-lookup"><span data-stu-id="7ff13-112">This is calculated using latitude/longitude information from the sign-in activity.</span></span>|
|<span data-ttu-id="7ff13-113">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="7ff13-113">countryOrRegion</span></span>|<span data-ttu-id="7ff13-114">String</span><span class="sxs-lookup"><span data-stu-id="7ff13-114">String</span></span>|<span data-ttu-id="7ff13-115">Предоставляет сведения о коде страны (код из 2 букв), где поступил вход.</span><span class="sxs-lookup"><span data-stu-id="7ff13-115">Provides the country code info (2 letter code) where the sign-in originated.</span></span>  <span data-ttu-id="7ff13-116">Рассчитывается с использованием информации о широте и долготе из действия, выполняемого при входе.</span><span class="sxs-lookup"><span data-stu-id="7ff13-116">This is calculated using latitude/longitude information from the sign-in activity.</span></span>|
|<span data-ttu-id="7ff13-117">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="7ff13-117">geoCoordinates</span></span>|[<span data-ttu-id="7ff13-118">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="7ff13-118">geoCoordinates</span></span>](geocoordinates.md)|<span data-ttu-id="7ff13-119">Предоставляет широту, долготу и высоту, на которой поступил вход.</span><span class="sxs-lookup"><span data-stu-id="7ff13-119">Provides the latitude, longitude and altitude where the sign-in originated.</span></span>|
|<span data-ttu-id="7ff13-120">state</span><span class="sxs-lookup"><span data-stu-id="7ff13-120">state</span></span>|<span data-ttu-id="7ff13-121">String</span><span class="sxs-lookup"><span data-stu-id="7ff13-121">String</span></span>|<span data-ttu-id="7ff13-122">Предоставляет состояние, в котором поступил вход.</span><span class="sxs-lookup"><span data-stu-id="7ff13-122">Provides the State where the sign-in originated.</span></span> <span data-ttu-id="7ff13-123">Рассчитывается с использованием информации о широте и долготе из действия, выполняемого при входе.</span><span class="sxs-lookup"><span data-stu-id="7ff13-123">This is calculated using latitude/longitude information from the sign-in activity.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7ff13-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7ff13-124">JSON representation</span></span>

<span data-ttu-id="7ff13-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7ff13-125">Here is a JSON representation of the resource.</span></span>

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
