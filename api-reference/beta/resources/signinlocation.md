---
title: Тип ресурса signInLocation
description: Предоставляет город, область и страну или регион, из которых выполняется вход.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: SarahBar
ms.openlocfilehash: eb4208820c1654a5b8db0d4afa2eeb1df4fb2b53
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46808594"
---
# <a name="signinlocation-resource-type"></a><span data-ttu-id="67ce4-103">Тип ресурса signInLocation</span><span class="sxs-lookup"><span data-stu-id="67ce4-103">signInLocation resource type</span></span>

<span data-ttu-id="67ce4-104">Пространство имен: Microsoft. Graph предоставляет город, область и страну или регион, из которого выполняется вход.</span><span class="sxs-lookup"><span data-stu-id="67ce4-104">Namespace: microsoft.graph Provides the city, state and country/region from where the sign-in happened.</span></span>



## <a name="properties"></a><span data-ttu-id="67ce4-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="67ce4-105">Properties</span></span>
| <span data-ttu-id="67ce4-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="67ce4-106">Property</span></span>     | <span data-ttu-id="67ce4-107">Тип</span><span class="sxs-lookup"><span data-stu-id="67ce4-107">Type</span></span>   |<span data-ttu-id="67ce4-108">Описание</span><span class="sxs-lookup"><span data-stu-id="67ce4-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="67ce4-109">city</span><span class="sxs-lookup"><span data-stu-id="67ce4-109">city</span></span>|<span data-ttu-id="67ce4-110">String</span><span class="sxs-lookup"><span data-stu-id="67ce4-110">String</span></span>|<span data-ttu-id="67ce4-111">Предоставляет город, в котором поступил вход.</span><span class="sxs-lookup"><span data-stu-id="67ce4-111">Provides the city where the sign-in originated.</span></span> <span data-ttu-id="67ce4-112">Рассчитывается с использованием информации о широте и долготе из действия, выполняемого при входе.</span><span class="sxs-lookup"><span data-stu-id="67ce4-112">This is calculated using latitude/longitude information from the sign-in activity.</span></span>|
|<span data-ttu-id="67ce4-113">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="67ce4-113">countryOrRegion</span></span>|<span data-ttu-id="67ce4-114">String</span><span class="sxs-lookup"><span data-stu-id="67ce4-114">String</span></span>|<span data-ttu-id="67ce4-115">Предоставляет сведения о коде страны (код из 2 букв), где поступил вход.</span><span class="sxs-lookup"><span data-stu-id="67ce4-115">Provides the country code info (2 letter code) where the sign-in originated.</span></span>  <span data-ttu-id="67ce4-116">Рассчитывается с использованием информации о широте и долготе из действия, выполняемого при входе.</span><span class="sxs-lookup"><span data-stu-id="67ce4-116">This is calculated using latitude/longitude information from the sign-in activity.</span></span>|
|<span data-ttu-id="67ce4-117">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="67ce4-117">geoCoordinates</span></span>|[<span data-ttu-id="67ce4-118">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="67ce4-118">geoCoordinates</span></span>](geocoordinates.md)|<span data-ttu-id="67ce4-119">Предоставляет широту, долготу и высоту, на которой поступил вход.</span><span class="sxs-lookup"><span data-stu-id="67ce4-119">Provides the latitude, longitude and altitude where the sign-in originated.</span></span>|
|<span data-ttu-id="67ce4-120">state</span><span class="sxs-lookup"><span data-stu-id="67ce4-120">state</span></span>|<span data-ttu-id="67ce4-121">String</span><span class="sxs-lookup"><span data-stu-id="67ce4-121">String</span></span>|<span data-ttu-id="67ce4-122">Предоставляет состояние, в котором поступил вход.</span><span class="sxs-lookup"><span data-stu-id="67ce4-122">Provides the State where the sign-in originated.</span></span> <span data-ttu-id="67ce4-123">Рассчитывается с использованием информации о широте и долготе из действия, выполняемого при входе.</span><span class="sxs-lookup"><span data-stu-id="67ce4-123">This is calculated using latitude/longitude information from the sign-in activity.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="67ce4-124">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="67ce4-124">JSON representation</span></span>

<span data-ttu-id="67ce4-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="67ce4-125">Here is a JSON representation of the resource.</span></span>

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
