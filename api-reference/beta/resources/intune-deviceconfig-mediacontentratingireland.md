---
title: Тип ресурса mediaContentRatingIreland
description: Н/Д
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b3efd96cc8ad015989365dff10b1659ef50c4fb7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422602"
---
# <a name="mediacontentratingireland-resource-type"></a><span data-ttu-id="b7aa9-103">Тип ресурса mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="b7aa9-103">mediaContentRatingIreland resource type</span></span>

> <span data-ttu-id="b7aa9-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b7aa9-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b7aa9-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b7aa9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b7aa9-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b7aa9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b7aa9-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="b7aa9-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="b7aa9-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="b7aa9-108">Properties</span></span>
|<span data-ttu-id="b7aa9-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="b7aa9-109">Property</span></span>|<span data-ttu-id="b7aa9-110">Тип</span><span class="sxs-lookup"><span data-stu-id="b7aa9-110">Type</span></span>|<span data-ttu-id="b7aa9-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b7aa9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b7aa9-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="b7aa9-112">movieRating</span></span>|[<span data-ttu-id="b7aa9-113">ratingIrelandMoviesType</span><span class="sxs-lookup"><span data-stu-id="b7aa9-113">ratingIrelandMoviesType</span></span>](../resources/intune-deviceconfig-ratingirelandmoviestype.md)|<span data-ttu-id="b7aa9-114">Оценка выбранных для Ирландия фильмы.</span><span class="sxs-lookup"><span data-stu-id="b7aa9-114">Movies rating selected for Ireland.</span></span> <span data-ttu-id="b7aa9-115">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="b7aa9-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="b7aa9-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="b7aa9-116">tvRating</span></span>|[<span data-ttu-id="b7aa9-117">ratingIrelandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="b7aa9-117">ratingIrelandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingirelandtelevisiontype.md)|<span data-ttu-id="b7aa9-118">Оценка TV, выбранной для Ирландия.</span><span class="sxs-lookup"><span data-stu-id="b7aa9-118">TV rating selected for Ireland.</span></span> <span data-ttu-id="b7aa9-119">Возможные значения: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span><span class="sxs-lookup"><span data-stu-id="b7aa9-119">Possible values are: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b7aa9-120">Связи</span><span class="sxs-lookup"><span data-stu-id="b7aa9-120">Relationships</span></span>
<span data-ttu-id="b7aa9-121">Нет</span><span class="sxs-lookup"><span data-stu-id="b7aa9-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b7aa9-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b7aa9-122">JSON Representation</span></span>
<span data-ttu-id="b7aa9-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b7aa9-123">Here is a JSON representation of the resource.</span></span>
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




