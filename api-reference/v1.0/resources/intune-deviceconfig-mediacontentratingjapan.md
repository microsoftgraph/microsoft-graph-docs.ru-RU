---
title: Тип ресурса mediaContentRatingJapan
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 398192d54c2e377d6d6a4cfad2e519b78d84420d
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37359966"
---
# <a name="mediacontentratingjapan-resource-type"></a><span data-ttu-id="08254-103">Тип ресурса mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="08254-103">mediaContentRatingJapan resource type</span></span>

> <span data-ttu-id="08254-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="08254-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="08254-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="08254-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="08254-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="08254-106">Properties</span></span>
|<span data-ttu-id="08254-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="08254-107">Property</span></span>|<span data-ttu-id="08254-108">Тип</span><span class="sxs-lookup"><span data-stu-id="08254-108">Type</span></span>|<span data-ttu-id="08254-109">Описание</span><span class="sxs-lookup"><span data-stu-id="08254-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08254-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="08254-110">movieRating</span></span>|[<span data-ttu-id="08254-111">ратингжапанмовиестипе</span><span class="sxs-lookup"><span data-stu-id="08254-111">ratingJapanMoviesType</span></span>](../resources/intune-deviceconfig-ratingjapanmoviestype.md)|<span data-ttu-id="08254-112">Оценка фильмов выбрана для Японии.</span><span class="sxs-lookup"><span data-stu-id="08254-112">Movies rating selected for Japan.</span></span> <span data-ttu-id="08254-113">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="08254-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="08254-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="08254-114">tvRating</span></span>|[<span data-ttu-id="08254-115">ратингжапантелевисионтипе</span><span class="sxs-lookup"><span data-stu-id="08254-115">ratingJapanTelevisionType</span></span>](../resources/intune-deviceconfig-ratingjapantelevisiontype.md)|<span data-ttu-id="08254-116">Рейтинг для телевизора выбран для Японии.</span><span class="sxs-lookup"><span data-stu-id="08254-116">TV rating selected for Japan.</span></span> <span data-ttu-id="08254-117">Возможные значения: `allAllowed`, `allBlocked`, `explicitAllowed`.</span><span class="sxs-lookup"><span data-stu-id="08254-117">Possible values are: `allAllowed`, `allBlocked`, `explicitAllowed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="08254-118">Связи</span><span class="sxs-lookup"><span data-stu-id="08254-118">Relationships</span></span>
<span data-ttu-id="08254-119">Нет</span><span class="sxs-lookup"><span data-stu-id="08254-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="08254-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="08254-120">JSON Representation</span></span>
<span data-ttu-id="08254-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="08254-121">Here is a JSON representation of the resource.</span></span>
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




