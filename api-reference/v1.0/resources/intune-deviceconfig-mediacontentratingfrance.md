---
title: Тип ресурса mediaContentRatingFrance
description: Н/Д
author: tfitzmac
ms.openlocfilehash: 0981a73fdc1e8468d9e8ab8590387dfa357a39c9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27361644"
---
# <a name="mediacontentratingfrance-resource-type"></a><span data-ttu-id="87aae-103">Тип ресурса mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="87aae-103">mediaContentRatingFrance resource type</span></span>

> <span data-ttu-id="87aae-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="87aae-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="87aae-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="87aae-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="87aae-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="87aae-106">Properties</span></span>
|<span data-ttu-id="87aae-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="87aae-107">Property</span></span>|<span data-ttu-id="87aae-108">Тип</span><span class="sxs-lookup"><span data-stu-id="87aae-108">Type</span></span>|<span data-ttu-id="87aae-109">Описание</span><span class="sxs-lookup"><span data-stu-id="87aae-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="87aae-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="87aae-110">movieRating</span></span>|[<span data-ttu-id="87aae-111">ratingFranceMoviesType</span><span class="sxs-lookup"><span data-stu-id="87aae-111">ratingFranceMoviesType</span></span>](../resources/intune-deviceconfig-ratingfrancemoviestype.md)|<span data-ttu-id="87aae-112">Оценка выбранных для Франции фильмы.</span><span class="sxs-lookup"><span data-stu-id="87aae-112">Movies rating selected for France.</span></span> <span data-ttu-id="87aae-113">Возможные значения: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="87aae-113">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|
|<span data-ttu-id="87aae-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="87aae-114">tvRating</span></span>|[<span data-ttu-id="87aae-115">ratingFranceTelevisionType</span><span class="sxs-lookup"><span data-stu-id="87aae-115">ratingFranceTelevisionType</span></span>](../resources/intune-deviceconfig-ratingfrancetelevisiontype.md)|<span data-ttu-id="87aae-116">Оценка TV, выбранной для Франции.</span><span class="sxs-lookup"><span data-stu-id="87aae-116">TV rating selected for France.</span></span> <span data-ttu-id="87aae-117">Возможные значения: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="87aae-117">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="87aae-118">Связи</span><span class="sxs-lookup"><span data-stu-id="87aae-118">Relationships</span></span>
<span data-ttu-id="87aae-119">Нет</span><span class="sxs-lookup"><span data-stu-id="87aae-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="87aae-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="87aae-120">JSON Representation</span></span>
<span data-ttu-id="87aae-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="87aae-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingFrance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingFrance",
  "movieRating": "String",
  "tvRating": "String"
}
```



