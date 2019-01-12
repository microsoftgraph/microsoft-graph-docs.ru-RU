---
title: Тип ресурса mediaContentRatingIreland
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9516c98350c239393e735008e91d966f8c6ae7a2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27958000"
---
# <a name="mediacontentratingireland-resource-type"></a><span data-ttu-id="31a73-103">Тип ресурса mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="31a73-103">mediaContentRatingIreland resource type</span></span>

> <span data-ttu-id="31a73-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="31a73-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="31a73-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="31a73-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="31a73-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="31a73-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="31a73-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="31a73-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="31a73-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="31a73-108">Properties</span></span>
|<span data-ttu-id="31a73-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="31a73-109">Property</span></span>|<span data-ttu-id="31a73-110">Тип</span><span class="sxs-lookup"><span data-stu-id="31a73-110">Type</span></span>|<span data-ttu-id="31a73-111">Описание</span><span class="sxs-lookup"><span data-stu-id="31a73-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31a73-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="31a73-112">movieRating</span></span>|[<span data-ttu-id="31a73-113">ratingIrelandMoviesType</span><span class="sxs-lookup"><span data-stu-id="31a73-113">ratingIrelandMoviesType</span></span>](../resources/intune-deviceconfig-ratingirelandmoviestype.md)|<span data-ttu-id="31a73-114">Оценка выбранных для Ирландия фильмы.</span><span class="sxs-lookup"><span data-stu-id="31a73-114">Movies rating selected for Ireland.</span></span> <span data-ttu-id="31a73-115">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="31a73-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="31a73-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="31a73-116">tvRating</span></span>|[<span data-ttu-id="31a73-117">ratingIrelandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="31a73-117">ratingIrelandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingirelandtelevisiontype.md)|<span data-ttu-id="31a73-118">Оценка TV, выбранной для Ирландия.</span><span class="sxs-lookup"><span data-stu-id="31a73-118">TV rating selected for Ireland.</span></span> <span data-ttu-id="31a73-119">Возможные значения: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span><span class="sxs-lookup"><span data-stu-id="31a73-119">Possible values are: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="31a73-120">Связи</span><span class="sxs-lookup"><span data-stu-id="31a73-120">Relationships</span></span>
<span data-ttu-id="31a73-121">Нет</span><span class="sxs-lookup"><span data-stu-id="31a73-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="31a73-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="31a73-122">JSON Representation</span></span>
<span data-ttu-id="31a73-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="31a73-123">Here is a JSON representation of the resource.</span></span>
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





