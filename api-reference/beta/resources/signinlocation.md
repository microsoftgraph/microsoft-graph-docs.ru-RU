---
title: Тип ресурса signInLocation
description: Предоставляет город, штат и страну или регион, из которых произошел вход.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-access-reports
author: SarahBar
ms.openlocfilehash: bc45d94896cbd822cdad4e3451f471bc3b540888
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134682"
---
# <a name="signinlocation-resource-type"></a><span data-ttu-id="97a70-103">Тип ресурса signInLocation</span><span class="sxs-lookup"><span data-stu-id="97a70-103">signInLocation resource type</span></span>

<span data-ttu-id="97a70-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="97a70-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="97a70-105">Предоставляет город, штат и страну или регион, из которых произошел вход.</span><span class="sxs-lookup"><span data-stu-id="97a70-105">Provides the city, state and country/region from where the sign-in happened.</span></span>



## <a name="properties"></a><span data-ttu-id="97a70-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="97a70-106">Properties</span></span>
| <span data-ttu-id="97a70-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="97a70-107">Property</span></span>     | <span data-ttu-id="97a70-108">Тип</span><span class="sxs-lookup"><span data-stu-id="97a70-108">Type</span></span>   |<span data-ttu-id="97a70-109">Описание</span><span class="sxs-lookup"><span data-stu-id="97a70-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="97a70-110">city</span><span class="sxs-lookup"><span data-stu-id="97a70-110">city</span></span>|<span data-ttu-id="97a70-111">String</span><span class="sxs-lookup"><span data-stu-id="97a70-111">String</span></span>|<span data-ttu-id="97a70-112">Предоставляет город, в котором был произведен вход.</span><span class="sxs-lookup"><span data-stu-id="97a70-112">Provides the city where the sign-in originated.</span></span> <span data-ttu-id="97a70-113">Этот метод вычисляется с использованием сведений о широте и долготе из действия при входе.</span><span class="sxs-lookup"><span data-stu-id="97a70-113">This is calculated using latitude/longitude information from the sign-in activity.</span></span>|
|<span data-ttu-id="97a70-114">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="97a70-114">countryOrRegion</span></span>|<span data-ttu-id="97a70-115">String</span><span class="sxs-lookup"><span data-stu-id="97a70-115">String</span></span>|<span data-ttu-id="97a70-116">Предоставляет сведения о коде страны (2 буквы), с которых был произведен вход.</span><span class="sxs-lookup"><span data-stu-id="97a70-116">Provides the country code info (2 letter code) where the sign-in originated.</span></span>  <span data-ttu-id="97a70-117">Это вычисляется с использованием сведений о широте и долготе из действия при входе.</span><span class="sxs-lookup"><span data-stu-id="97a70-117">This is calculated using latitude/longitude information from the sign-in activity.</span></span>|
|<span data-ttu-id="97a70-118">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="97a70-118">geoCoordinates</span></span>|[<span data-ttu-id="97a70-119">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="97a70-119">geoCoordinates</span></span>](geocoordinates.md)|<span data-ttu-id="97a70-120">Предоставляет широту, долготу и высоту, в которой был произведен вход.</span><span class="sxs-lookup"><span data-stu-id="97a70-120">Provides the latitude, longitude and altitude where the sign-in originated.</span></span>|
|<span data-ttu-id="97a70-121">state</span><span class="sxs-lookup"><span data-stu-id="97a70-121">state</span></span>|<span data-ttu-id="97a70-122">String</span><span class="sxs-lookup"><span data-stu-id="97a70-122">String</span></span>|<span data-ttu-id="97a70-123">Предоставляет состояние, в котором был произведен вход.</span><span class="sxs-lookup"><span data-stu-id="97a70-123">Provides the State where the sign-in originated.</span></span> <span data-ttu-id="97a70-124">Этот метод вычисляется с использованием сведений о широте и долготе из действия при входе.</span><span class="sxs-lookup"><span data-stu-id="97a70-124">This is calculated using latitude/longitude information from the sign-in activity.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="97a70-125">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="97a70-125">JSON representation</span></span>

<span data-ttu-id="97a70-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="97a70-126">Here is a JSON representation of the resource.</span></span>

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


