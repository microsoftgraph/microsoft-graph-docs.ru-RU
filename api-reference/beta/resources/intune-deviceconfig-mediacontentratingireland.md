---
title: Тип ресурса mediaContentRatingIreland
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2f6fee57eb4432781d7600f34b5ac444c498c3d2
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33944882"
---
# <a name="mediacontentratingireland-resource-type"></a><span data-ttu-id="db453-103">Тип ресурса mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="db453-103">mediaContentRatingIreland resource type</span></span>

> <span data-ttu-id="db453-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="db453-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="db453-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="db453-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="db453-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="db453-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="db453-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="db453-107">Properties</span></span>
|<span data-ttu-id="db453-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="db453-108">Property</span></span>|<span data-ttu-id="db453-109">Тип</span><span class="sxs-lookup"><span data-stu-id="db453-109">Type</span></span>|<span data-ttu-id="db453-110">Описание</span><span class="sxs-lookup"><span data-stu-id="db453-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="db453-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="db453-111">movieRating</span></span>|[<span data-ttu-id="db453-112">Ратингиреландмовиестипе</span><span class="sxs-lookup"><span data-stu-id="db453-112">ratingIrelandMoviesType</span></span>](../resources/intune-deviceconfig-ratingirelandmoviestype.md)|<span data-ttu-id="db453-113">Оценка фильмов выбрана для Ирландии.</span><span class="sxs-lookup"><span data-stu-id="db453-113">Movies rating selected for Ireland.</span></span> <span data-ttu-id="db453-114">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="db453-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="db453-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="db453-115">tvRating</span></span>|[<span data-ttu-id="db453-116">Ратингиреландтелевисионтипе</span><span class="sxs-lookup"><span data-stu-id="db453-116">ratingIrelandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingirelandtelevisiontype.md)|<span data-ttu-id="db453-117">Рейтинг телевизора выбран для Ирландии.</span><span class="sxs-lookup"><span data-stu-id="db453-117">TV rating selected for Ireland.</span></span> <span data-ttu-id="db453-118">Возможные значения: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span><span class="sxs-lookup"><span data-stu-id="db453-118">Possible values are: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="db453-119">Связи</span><span class="sxs-lookup"><span data-stu-id="db453-119">Relationships</span></span>
<span data-ttu-id="db453-120">Нет</span><span class="sxs-lookup"><span data-stu-id="db453-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="db453-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="db453-121">JSON Representation</span></span>
<span data-ttu-id="db453-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="db453-122">Here is a JSON representation of the resource.</span></span>
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




