---
title: Тип ресурса mediaContentRatingIreland
description: Пока не задокументировано.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 153164010b6beda5d38779f67ffcd0654a1c986a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32572362"
---
# <a name="mediacontentratingireland-resource-type"></a><span data-ttu-id="a7992-103">Тип ресурса mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="a7992-103">mediaContentRatingIreland resource type</span></span>

> <span data-ttu-id="a7992-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a7992-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a7992-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="a7992-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="a7992-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="a7992-106">Properties</span></span>
|<span data-ttu-id="a7992-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="a7992-107">Property</span></span>|<span data-ttu-id="a7992-108">Тип</span><span class="sxs-lookup"><span data-stu-id="a7992-108">Type</span></span>|<span data-ttu-id="a7992-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a7992-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7992-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="a7992-110">movieRating</span></span>|[<span data-ttu-id="a7992-111">Ратингиреландмовиестипе</span><span class="sxs-lookup"><span data-stu-id="a7992-111">ratingIrelandMoviesType</span></span>](../resources/intune-deviceconfig-ratingirelandmoviestype.md)|<span data-ttu-id="a7992-112">Оценка фильмов выбрана для Ирландии.</span><span class="sxs-lookup"><span data-stu-id="a7992-112">Movies rating selected for Ireland.</span></span> <span data-ttu-id="a7992-113">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="a7992-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="a7992-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="a7992-114">tvRating</span></span>|[<span data-ttu-id="a7992-115">Ратингиреландтелевисионтипе</span><span class="sxs-lookup"><span data-stu-id="a7992-115">ratingIrelandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingirelandtelevisiontype.md)|<span data-ttu-id="a7992-116">Рейтинг телевизора выбран для Ирландии.</span><span class="sxs-lookup"><span data-stu-id="a7992-116">TV rating selected for Ireland.</span></span> <span data-ttu-id="a7992-117">Возможные значения: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span><span class="sxs-lookup"><span data-stu-id="a7992-117">Possible values are: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a7992-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="a7992-118">Relationships</span></span>
<span data-ttu-id="a7992-119">Нет</span><span class="sxs-lookup"><span data-stu-id="a7992-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a7992-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a7992-120">JSON Representation</span></span>
<span data-ttu-id="a7992-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a7992-121">Here is a JSON representation of the resource.</span></span>
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



