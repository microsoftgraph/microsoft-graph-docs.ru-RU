---
title: Тип ресурса mediaContentRatingJapan
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0543aec86312d90a5896ed3f06f004c87d8e6a58
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30250308"
---
# <a name="mediacontentratingjapan-resource-type"></a><span data-ttu-id="927bf-103">Тип ресурса mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="927bf-103">mediaContentRatingJapan resource type</span></span>

> <span data-ttu-id="927bf-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="927bf-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="927bf-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="927bf-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="927bf-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="927bf-106">Properties</span></span>
|<span data-ttu-id="927bf-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="927bf-107">Property</span></span>|<span data-ttu-id="927bf-108">Тип</span><span class="sxs-lookup"><span data-stu-id="927bf-108">Type</span></span>|<span data-ttu-id="927bf-109">Описание</span><span class="sxs-lookup"><span data-stu-id="927bf-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="927bf-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="927bf-110">movieRating</span></span>|[<span data-ttu-id="927bf-111">Ратингжапанмовиестипе</span><span class="sxs-lookup"><span data-stu-id="927bf-111">ratingJapanMoviesType</span></span>](../resources/intune-deviceconfig-ratingjapanmoviestype.md)|<span data-ttu-id="927bf-112">Оценка фильмов выбрана для Японии.</span><span class="sxs-lookup"><span data-stu-id="927bf-112">Movies rating selected for Japan.</span></span> <span data-ttu-id="927bf-113">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="927bf-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="927bf-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="927bf-114">tvRating</span></span>|[<span data-ttu-id="927bf-115">Ратингжапантелевисионтипе</span><span class="sxs-lookup"><span data-stu-id="927bf-115">ratingJapanTelevisionType</span></span>](../resources/intune-deviceconfig-ratingjapantelevisiontype.md)|<span data-ttu-id="927bf-116">Рейтинг для телевизора выбран для Японии.</span><span class="sxs-lookup"><span data-stu-id="927bf-116">TV rating selected for Japan.</span></span> <span data-ttu-id="927bf-117">Возможные значения: `allAllowed`, `allBlocked`, `explicitAllowed`.</span><span class="sxs-lookup"><span data-stu-id="927bf-117">Possible values are: `allAllowed`, `allBlocked`, `explicitAllowed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="927bf-118">Связи</span><span class="sxs-lookup"><span data-stu-id="927bf-118">Relationships</span></span>
<span data-ttu-id="927bf-119">Нет</span><span class="sxs-lookup"><span data-stu-id="927bf-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="927bf-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="927bf-120">JSON Representation</span></span>
<span data-ttu-id="927bf-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="927bf-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingJapan"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingJapan",
  "movieRating": "String",
  "tvRating": "String"
}
```



