---
title: Тип ресурса mediaContentRatingIreland
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a7c808cd6c614837acbb863e92323429d5b4a110
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48003124"
---
# <a name="mediacontentratingireland-resource-type"></a><span data-ttu-id="e7118-103">Тип ресурса mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="e7118-103">mediaContentRatingIreland resource type</span></span>

<span data-ttu-id="e7118-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e7118-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e7118-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e7118-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e7118-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="e7118-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="e7118-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="e7118-107">Properties</span></span>
|<span data-ttu-id="e7118-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="e7118-108">Property</span></span>|<span data-ttu-id="e7118-109">Тип</span><span class="sxs-lookup"><span data-stu-id="e7118-109">Type</span></span>|<span data-ttu-id="e7118-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e7118-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7118-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="e7118-111">movieRating</span></span>|[<span data-ttu-id="e7118-112">ратингиреландмовиестипе</span><span class="sxs-lookup"><span data-stu-id="e7118-112">ratingIrelandMoviesType</span></span>](../resources/intune-deviceconfig-ratingirelandmoviestype.md)|<span data-ttu-id="e7118-113">Оценка фильмов выбрана для Ирландии.</span><span class="sxs-lookup"><span data-stu-id="e7118-113">Movies rating selected for Ireland.</span></span> <span data-ttu-id="e7118-114">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="e7118-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="e7118-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="e7118-115">tvRating</span></span>|[<span data-ttu-id="e7118-116">ратингиреландтелевисионтипе</span><span class="sxs-lookup"><span data-stu-id="e7118-116">ratingIrelandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingirelandtelevisiontype.md)|<span data-ttu-id="e7118-117">Рейтинг телевизора выбран для Ирландии.</span><span class="sxs-lookup"><span data-stu-id="e7118-117">TV rating selected for Ireland.</span></span> <span data-ttu-id="e7118-118">Возможные значения: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span><span class="sxs-lookup"><span data-stu-id="e7118-118">Possible values are: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e7118-119">Связи</span><span class="sxs-lookup"><span data-stu-id="e7118-119">Relationships</span></span>
<span data-ttu-id="e7118-120">Нет</span><span class="sxs-lookup"><span data-stu-id="e7118-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e7118-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e7118-121">JSON Representation</span></span>
<span data-ttu-id="e7118-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e7118-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingIreland"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingIreland",
  "movieRating": "String",
  "tvRating": "String"
}
```









