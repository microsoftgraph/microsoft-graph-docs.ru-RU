---
title: Тип ресурса signInLocation
description: Предоставляет город, штат и страну или регион, из которых произошел вход.
localization_priority: Normal
author: dhanyahk
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: c003fda44e54bbee5957e794d02b90f008f4b8f5
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137097"
---
# <a name="signinlocation-resource-type"></a><span data-ttu-id="d6146-103">Тип ресурса signInLocation</span><span class="sxs-lookup"><span data-stu-id="d6146-103">signInLocation resource type</span></span>

<span data-ttu-id="d6146-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d6146-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d6146-105">Предоставляет город, штат и страну или регион, из которых произошел вход.</span><span class="sxs-lookup"><span data-stu-id="d6146-105">Provides the city, state and country/region from where the sign-in happened.</span></span>

## <a name="properties"></a><span data-ttu-id="d6146-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="d6146-106">Properties</span></span>

| <span data-ttu-id="d6146-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="d6146-107">Property</span></span>     | <span data-ttu-id="d6146-108">Тип</span><span class="sxs-lookup"><span data-stu-id="d6146-108">Type</span></span>   |<span data-ttu-id="d6146-109">Описание</span><span class="sxs-lookup"><span data-stu-id="d6146-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d6146-110">city</span><span class="sxs-lookup"><span data-stu-id="d6146-110">city</span></span>|<span data-ttu-id="d6146-111">String</span><span class="sxs-lookup"><span data-stu-id="d6146-111">String</span></span>|<span data-ttu-id="d6146-112">Предоставляет город, в котором был произведен вход.</span><span class="sxs-lookup"><span data-stu-id="d6146-112">Provides the city where the sign-in originated.</span></span> <span data-ttu-id="d6146-113">Этот метод вычисляется с использованием сведений о широте и долготе из действия при входе.</span><span class="sxs-lookup"><span data-stu-id="d6146-113">This is calculated using latitude/longitude information from the sign-in activity.</span></span>|
|<span data-ttu-id="d6146-114">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="d6146-114">countryOrRegion</span></span>|<span data-ttu-id="d6146-115">String</span><span class="sxs-lookup"><span data-stu-id="d6146-115">String</span></span>|<span data-ttu-id="d6146-116">Предоставляет сведения о коде страны (2 буквы), с которых был произведен вход.</span><span class="sxs-lookup"><span data-stu-id="d6146-116">Provides the country code info (2 letter code) where the sign-in originated.</span></span>  <span data-ttu-id="d6146-117">Этот метод вычисляется с использованием сведений о широте и долготе из действия при входе.</span><span class="sxs-lookup"><span data-stu-id="d6146-117">This is calculated using latitude/longitude information from the sign-in activity.</span></span>|
|<span data-ttu-id="d6146-118">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="d6146-118">geoCoordinates</span></span>|[<span data-ttu-id="d6146-119">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="d6146-119">geoCoordinates</span></span>](geocoordinates.md)|<span data-ttu-id="d6146-120">Предоставляет широту, долготу и высоту, в которой был произведен вход.</span><span class="sxs-lookup"><span data-stu-id="d6146-120">Provides the latitude, longitude and altitude where the sign-in originated.</span></span>|
|<span data-ttu-id="d6146-121">state</span><span class="sxs-lookup"><span data-stu-id="d6146-121">state</span></span>|<span data-ttu-id="d6146-122">String</span><span class="sxs-lookup"><span data-stu-id="d6146-122">String</span></span>|<span data-ttu-id="d6146-123">Предоставляет состояние, в котором был произведен вход.</span><span class="sxs-lookup"><span data-stu-id="d6146-123">Provides the State where the sign-in originated.</span></span> <span data-ttu-id="d6146-124">Это вычисляется с использованием сведений о широте и долготе из действия при входе.</span><span class="sxs-lookup"><span data-stu-id="d6146-124">This is calculated using latitude/longitude information from the sign-in activity.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d6146-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d6146-125">JSON representation</span></span>

<span data-ttu-id="d6146-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d6146-126">Here is a JSON representation of the resource.</span></span>

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

