---
title: Тип ресурса mediaContentRatingIreland
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: cb96a239ff31a0d6843b690d063361a65099e65e
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760024"
---
# <a name="mediacontentratingireland-resource-type"></a><span data-ttu-id="b31f0-103">Тип ресурса mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="b31f0-103">mediaContentRatingIreland resource type</span></span>

<span data-ttu-id="b31f0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b31f0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b31f0-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b31f0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b31f0-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="b31f0-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="b31f0-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="b31f0-107">Properties</span></span>
|<span data-ttu-id="b31f0-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="b31f0-108">Property</span></span>|<span data-ttu-id="b31f0-109">Тип</span><span class="sxs-lookup"><span data-stu-id="b31f0-109">Type</span></span>|<span data-ttu-id="b31f0-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b31f0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b31f0-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="b31f0-111">movieRating</span></span>|[<span data-ttu-id="b31f0-112">ratingIrelandMoviesType</span><span class="sxs-lookup"><span data-stu-id="b31f0-112">ratingIrelandMoviesType</span></span>](../resources/intune-deviceconfig-ratingirelandmoviestype.md)|<span data-ttu-id="b31f0-113">Рейтинг фильмов, выбранный для Ирландии.</span><span class="sxs-lookup"><span data-stu-id="b31f0-113">Movies rating selected for Ireland.</span></span> <span data-ttu-id="b31f0-114">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="b31f0-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="b31f0-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="b31f0-115">tvRating</span></span>|[<span data-ttu-id="b31f0-116">ratingIrelandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="b31f0-116">ratingIrelandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingirelandtelevisiontype.md)|<span data-ttu-id="b31f0-117">Телевизионный рейтинг, выбранный для Ирландии.</span><span class="sxs-lookup"><span data-stu-id="b31f0-117">TV rating selected for Ireland.</span></span> <span data-ttu-id="b31f0-118">Возможные значения: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span><span class="sxs-lookup"><span data-stu-id="b31f0-118">Possible values are: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b31f0-119">Связи</span><span class="sxs-lookup"><span data-stu-id="b31f0-119">Relationships</span></span>
<span data-ttu-id="b31f0-120">Нет</span><span class="sxs-lookup"><span data-stu-id="b31f0-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b31f0-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b31f0-121">JSON Representation</span></span>
<span data-ttu-id="b31f0-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b31f0-122">Here is a JSON representation of the resource.</span></span>
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




