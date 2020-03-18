---
title: Тип ресурса mediaContentRatingIreland
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5b6e6dc939672d855b2fd25b47a54ea3f62d4280
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42788578"
---
# <a name="mediacontentratingireland-resource-type"></a><span data-ttu-id="bfeb9-103">Тип ресурса mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="bfeb9-103">mediaContentRatingIreland resource type</span></span>

> <span data-ttu-id="bfeb9-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bfeb9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bfeb9-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bfeb9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bfeb9-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="bfeb9-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="bfeb9-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="bfeb9-107">Properties</span></span>
|<span data-ttu-id="bfeb9-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="bfeb9-108">Property</span></span>|<span data-ttu-id="bfeb9-109">Тип</span><span class="sxs-lookup"><span data-stu-id="bfeb9-109">Type</span></span>|<span data-ttu-id="bfeb9-110">Описание</span><span class="sxs-lookup"><span data-stu-id="bfeb9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bfeb9-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="bfeb9-111">movieRating</span></span>|[<span data-ttu-id="bfeb9-112">ратингиреландмовиестипе</span><span class="sxs-lookup"><span data-stu-id="bfeb9-112">ratingIrelandMoviesType</span></span>](../resources/intune-deviceconfig-ratingirelandmoviestype.md)|<span data-ttu-id="bfeb9-113">Оценка фильмов выбрана для Ирландии.</span><span class="sxs-lookup"><span data-stu-id="bfeb9-113">Movies rating selected for Ireland.</span></span> <span data-ttu-id="bfeb9-114">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="bfeb9-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="bfeb9-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="bfeb9-115">tvRating</span></span>|[<span data-ttu-id="bfeb9-116">ратингиреландтелевисионтипе</span><span class="sxs-lookup"><span data-stu-id="bfeb9-116">ratingIrelandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingirelandtelevisiontype.md)|<span data-ttu-id="bfeb9-117">Рейтинг телевизора выбран для Ирландии.</span><span class="sxs-lookup"><span data-stu-id="bfeb9-117">TV rating selected for Ireland.</span></span> <span data-ttu-id="bfeb9-118">Возможные значения: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span><span class="sxs-lookup"><span data-stu-id="bfeb9-118">Possible values are: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bfeb9-119">Связи</span><span class="sxs-lookup"><span data-stu-id="bfeb9-119">Relationships</span></span>
<span data-ttu-id="bfeb9-120">Нет</span><span class="sxs-lookup"><span data-stu-id="bfeb9-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bfeb9-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bfeb9-121">JSON Representation</span></span>
<span data-ttu-id="bfeb9-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bfeb9-122">Here is a JSON representation of the resource.</span></span>
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



