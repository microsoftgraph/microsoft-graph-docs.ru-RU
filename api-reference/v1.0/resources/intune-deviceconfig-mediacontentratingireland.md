---
title: Тип ресурса mediaContentRatingIreland
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 531768883b88e8fc89fe00c1df7a8a9e8767a408
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27934879"
---
# <a name="mediacontentratingireland-resource-type"></a><span data-ttu-id="a4b86-103">Тип ресурса mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="a4b86-103">mediaContentRatingIreland resource type</span></span>

> <span data-ttu-id="a4b86-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a4b86-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a4b86-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="a4b86-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="a4b86-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="a4b86-106">Properties</span></span>
|<span data-ttu-id="a4b86-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="a4b86-107">Property</span></span>|<span data-ttu-id="a4b86-108">Тип</span><span class="sxs-lookup"><span data-stu-id="a4b86-108">Type</span></span>|<span data-ttu-id="a4b86-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a4b86-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a4b86-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="a4b86-110">movieRating</span></span>|[<span data-ttu-id="a4b86-111">ratingIrelandMoviesType</span><span class="sxs-lookup"><span data-stu-id="a4b86-111">ratingIrelandMoviesType</span></span>](../resources/intune-deviceconfig-ratingirelandmoviestype.md)|<span data-ttu-id="a4b86-112">Оценка выбранных для Ирландия фильмы.</span><span class="sxs-lookup"><span data-stu-id="a4b86-112">Movies rating selected for Ireland.</span></span> <span data-ttu-id="a4b86-113">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="a4b86-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="a4b86-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="a4b86-114">tvRating</span></span>|[<span data-ttu-id="a4b86-115">ratingIrelandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="a4b86-115">ratingIrelandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingirelandtelevisiontype.md)|<span data-ttu-id="a4b86-116">Оценка TV, выбранной для Ирландия.</span><span class="sxs-lookup"><span data-stu-id="a4b86-116">TV rating selected for Ireland.</span></span> <span data-ttu-id="a4b86-117">Возможные значения: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span><span class="sxs-lookup"><span data-stu-id="a4b86-117">Possible values are: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a4b86-118">Связи</span><span class="sxs-lookup"><span data-stu-id="a4b86-118">Relationships</span></span>
<span data-ttu-id="a4b86-119">Нет</span><span class="sxs-lookup"><span data-stu-id="a4b86-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a4b86-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a4b86-120">JSON Representation</span></span>
<span data-ttu-id="a4b86-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a4b86-121">Here is a JSON representation of the resource.</span></span>
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



