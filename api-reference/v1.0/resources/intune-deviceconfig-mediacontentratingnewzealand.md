---
title: Тип ресурса mediaContentRatingNewZealand
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7d6556409f0893430813d2e9dbd753f97fa76886
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27932247"
---
# <a name="mediacontentratingnewzealand-resource-type"></a><span data-ttu-id="62de0-103">Тип ресурса mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="62de0-103">mediaContentRatingNewZealand resource type</span></span>

> <span data-ttu-id="62de0-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="62de0-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="62de0-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="62de0-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="62de0-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="62de0-106">Properties</span></span>
|<span data-ttu-id="62de0-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="62de0-107">Property</span></span>|<span data-ttu-id="62de0-108">Тип</span><span class="sxs-lookup"><span data-stu-id="62de0-108">Type</span></span>|<span data-ttu-id="62de0-109">Описание</span><span class="sxs-lookup"><span data-stu-id="62de0-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62de0-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="62de0-110">movieRating</span></span>|[<span data-ttu-id="62de0-111">ratingNewZealandMoviesType</span><span class="sxs-lookup"><span data-stu-id="62de0-111">ratingNewZealandMoviesType</span></span>](../resources/intune-deviceconfig-ratingnewzealandmoviestype.md)|<span data-ttu-id="62de0-112">Оценка выбранных для новой Зеландии фильмы.</span><span class="sxs-lookup"><span data-stu-id="62de0-112">Movies rating selected for New Zealand.</span></span> <span data-ttu-id="62de0-113">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span><span class="sxs-lookup"><span data-stu-id="62de0-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span></span>|
|<span data-ttu-id="62de0-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="62de0-114">tvRating</span></span>|[<span data-ttu-id="62de0-115">ratingNewZealandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="62de0-115">ratingNewZealandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingnewzealandtelevisiontype.md)|<span data-ttu-id="62de0-116">Оценка TV, выбранной для новой Зеландии.</span><span class="sxs-lookup"><span data-stu-id="62de0-116">TV rating selected for New Zealand.</span></span> <span data-ttu-id="62de0-117">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="62de0-117">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="62de0-118">Связи</span><span class="sxs-lookup"><span data-stu-id="62de0-118">Relationships</span></span>
<span data-ttu-id="62de0-119">Нет</span><span class="sxs-lookup"><span data-stu-id="62de0-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="62de0-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="62de0-120">JSON Representation</span></span>
<span data-ttu-id="62de0-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="62de0-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingNewZealand"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingNewZealand",
  "movieRating": "String",
  "tvRating": "String"
}
```



