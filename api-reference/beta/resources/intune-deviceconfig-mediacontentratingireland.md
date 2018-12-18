---
title: Тип ресурса mediaContentRatingIreland
description: Н/Д
author: tfitzmac
ms.openlocfilehash: 6ade4ea9d5f2236803a8515b94ebc57f32ce3cd7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27337494"
---
# <a name="mediacontentratingireland-resource-type"></a><span data-ttu-id="e5b46-103">Тип ресурса mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="e5b46-103">mediaContentRatingIreland resource type</span></span>

> <span data-ttu-id="e5b46-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e5b46-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e5b46-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5b46-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e5b46-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e5b46-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e5b46-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="e5b46-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="e5b46-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="e5b46-108">Properties</span></span>
|<span data-ttu-id="e5b46-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="e5b46-109">Property</span></span>|<span data-ttu-id="e5b46-110">Тип</span><span class="sxs-lookup"><span data-stu-id="e5b46-110">Type</span></span>|<span data-ttu-id="e5b46-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e5b46-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5b46-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="e5b46-112">movieRating</span></span>|[<span data-ttu-id="e5b46-113">ratingIrelandMoviesType</span><span class="sxs-lookup"><span data-stu-id="e5b46-113">ratingIrelandMoviesType</span></span>](../resources/intune-deviceconfig-ratingirelandmoviestype.md)|<span data-ttu-id="e5b46-114">Оценка выбранных для Ирландия фильмы.</span><span class="sxs-lookup"><span data-stu-id="e5b46-114">Movies rating selected for Ireland.</span></span> <span data-ttu-id="e5b46-115">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="e5b46-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="e5b46-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="e5b46-116">tvRating</span></span>|[<span data-ttu-id="e5b46-117">ratingIrelandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="e5b46-117">ratingIrelandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingirelandtelevisiontype.md)|<span data-ttu-id="e5b46-118">Оценка TV, выбранной для Ирландия.</span><span class="sxs-lookup"><span data-stu-id="e5b46-118">TV rating selected for Ireland.</span></span> <span data-ttu-id="e5b46-119">Возможные значения: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span><span class="sxs-lookup"><span data-stu-id="e5b46-119">Possible values are: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e5b46-120">Связи</span><span class="sxs-lookup"><span data-stu-id="e5b46-120">Relationships</span></span>
<span data-ttu-id="e5b46-121">Нет</span><span class="sxs-lookup"><span data-stu-id="e5b46-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e5b46-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e5b46-122">JSON Representation</span></span>
<span data-ttu-id="e5b46-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e5b46-123">Here is a JSON representation of the resource.</span></span>
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





