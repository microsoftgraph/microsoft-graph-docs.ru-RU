---
title: Тип ресурса signInLocation
description: Предоставляет Город, состояние и страны или региона, из которой входа в произошло.
ms.openlocfilehash: a3d4f6ca5ec18e70960f45a3da1bb06d51ee1e65
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078908"
---
# <a name="signinlocation-resource-type"></a><span data-ttu-id="a32c7-103">Тип ресурса signInLocation</span><span class="sxs-lookup"><span data-stu-id="a32c7-103">signInLocation resource type</span></span>
<span data-ttu-id="a32c7-104">Предоставляет Город, состояние и страны или региона, из которой входа в произошло.</span><span class="sxs-lookup"><span data-stu-id="a32c7-104">Provides the city, state and country/region from where the sign-in happened.</span></span>



## <a name="properties"></a><span data-ttu-id="a32c7-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="a32c7-105">Properties</span></span>
| <span data-ttu-id="a32c7-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="a32c7-106">Property</span></span>     | <span data-ttu-id="a32c7-107">Тип</span><span class="sxs-lookup"><span data-stu-id="a32c7-107">Type</span></span>   |<span data-ttu-id="a32c7-108">Описание</span><span class="sxs-lookup"><span data-stu-id="a32c7-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a32c7-109">city</span><span class="sxs-lookup"><span data-stu-id="a32c7-109">city</span></span>|<span data-ttu-id="a32c7-110">String</span><span class="sxs-lookup"><span data-stu-id="a32c7-110">String</span></span>|<span data-ttu-id="a32c7-111">Предоставляет Город, входа в источник.</span><span class="sxs-lookup"><span data-stu-id="a32c7-111">Provides the city where the sign-in originated.</span></span> <span data-ttu-id="a32c7-112">При расчете используется в операции регистрации Широта и долгота сведения.</span><span class="sxs-lookup"><span data-stu-id="a32c7-112">This is calculated using latitude/longitude information from the sign-in activity.</span></span>|
|<span data-ttu-id="a32c7-113">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="a32c7-113">countryOrRegion</span></span>|<span data-ttu-id="a32c7-114">String</span><span class="sxs-lookup"><span data-stu-id="a32c7-114">String</span></span>|<span data-ttu-id="a32c7-115">Предоставляет info код страны (2 код письма) входа в источник.</span><span class="sxs-lookup"><span data-stu-id="a32c7-115">Provides the country code info (2 letter code) where the sign-in originated.</span></span>  <span data-ttu-id="a32c7-116">При расчете используется в операции регистрации Широта и долгота сведения.</span><span class="sxs-lookup"><span data-stu-id="a32c7-116">This is calculated using latitude/longitude information from the sign-in activity.</span></span>|
|<span data-ttu-id="a32c7-117">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="a32c7-117">geoCoordinates</span></span>|[<span data-ttu-id="a32c7-118">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="a32c7-118">geoCoordinates</span></span>](geocoordinates.md)|<span data-ttu-id="a32c7-119">Предоставляет широта, долгота и высота входа в источник.</span><span class="sxs-lookup"><span data-stu-id="a32c7-119">Provides the latitude, longitude and altitude where the sign-in originated.</span></span>|
|<span data-ttu-id="a32c7-120">state</span><span class="sxs-lookup"><span data-stu-id="a32c7-120">state</span></span>|<span data-ttu-id="a32c7-121">String</span><span class="sxs-lookup"><span data-stu-id="a32c7-121">String</span></span>|<span data-ttu-id="a32c7-122">Предоставляет состояние входа в источник.</span><span class="sxs-lookup"><span data-stu-id="a32c7-122">Provides the State where the sign-in originated.</span></span> <span data-ttu-id="a32c7-123">При расчете используется в операции регистрации Широта и долгота сведения.</span><span class="sxs-lookup"><span data-stu-id="a32c7-123">This is calculated using latitude/longitude information from the sign-in activity.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a32c7-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a32c7-124">JSON representation</span></span>

<span data-ttu-id="a32c7-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a32c7-125">Here is a JSON representation of the resource.</span></span>

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