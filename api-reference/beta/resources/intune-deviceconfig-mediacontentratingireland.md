---
title: Тип ресурса mediaContentRatingIreland
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 2d8decd8df49867a44ac8a9d7a6b9c0d454eece1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826264"
---
# <a name="mediacontentratingireland-resource-type"></a><span data-ttu-id="fbe29-103">Тип ресурса mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="fbe29-103">mediaContentRatingIreland resource type</span></span>

> <span data-ttu-id="fbe29-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fbe29-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fbe29-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fbe29-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fbe29-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="fbe29-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fbe29-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="fbe29-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="fbe29-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="fbe29-108">Properties</span></span>
|<span data-ttu-id="fbe29-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="fbe29-109">Property</span></span>|<span data-ttu-id="fbe29-110">Тип</span><span class="sxs-lookup"><span data-stu-id="fbe29-110">Type</span></span>|<span data-ttu-id="fbe29-111">Описание</span><span class="sxs-lookup"><span data-stu-id="fbe29-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fbe29-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="fbe29-112">movieRating</span></span>|[<span data-ttu-id="fbe29-113">ratingIrelandMoviesType</span><span class="sxs-lookup"><span data-stu-id="fbe29-113">ratingIrelandMoviesType</span></span>](../resources/intune-deviceconfig-ratingirelandmoviestype.md)|<span data-ttu-id="fbe29-114">Оценка выбранных для Ирландия фильмы.</span><span class="sxs-lookup"><span data-stu-id="fbe29-114">Movies rating selected for Ireland.</span></span> <span data-ttu-id="fbe29-115">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="fbe29-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="fbe29-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="fbe29-116">tvRating</span></span>|[<span data-ttu-id="fbe29-117">ratingIrelandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="fbe29-117">ratingIrelandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingirelandtelevisiontype.md)|<span data-ttu-id="fbe29-118">Оценка TV, выбранной для Ирландия.</span><span class="sxs-lookup"><span data-stu-id="fbe29-118">TV rating selected for Ireland.</span></span> <span data-ttu-id="fbe29-119">Возможные значения: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span><span class="sxs-lookup"><span data-stu-id="fbe29-119">Possible values are: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fbe29-120">Связи</span><span class="sxs-lookup"><span data-stu-id="fbe29-120">Relationships</span></span>
<span data-ttu-id="fbe29-121">Нет</span><span class="sxs-lookup"><span data-stu-id="fbe29-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="fbe29-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fbe29-122">JSON Representation</span></span>
<span data-ttu-id="fbe29-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fbe29-123">Here is a JSON representation of the resource.</span></span>
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





