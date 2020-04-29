---
title: Тип ресурса mediaContentRatingIreland
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 01135bb6c5a19ae837a834a51a5857b5f54baac0
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43473162"
---
# <a name="mediacontentratingireland-resource-type"></a><span data-ttu-id="a2fe5-103">Тип ресурса mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="a2fe5-103">mediaContentRatingIreland resource type</span></span>

<span data-ttu-id="a2fe5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2fe5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a2fe5-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a2fe5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a2fe5-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="a2fe5-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="a2fe5-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="a2fe5-107">Properties</span></span>
|<span data-ttu-id="a2fe5-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="a2fe5-108">Property</span></span>|<span data-ttu-id="a2fe5-109">Тип</span><span class="sxs-lookup"><span data-stu-id="a2fe5-109">Type</span></span>|<span data-ttu-id="a2fe5-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a2fe5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2fe5-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="a2fe5-111">movieRating</span></span>|[<span data-ttu-id="a2fe5-112">ратингиреландмовиестипе</span><span class="sxs-lookup"><span data-stu-id="a2fe5-112">ratingIrelandMoviesType</span></span>](../resources/intune-deviceconfig-ratingirelandmoviestype.md)|<span data-ttu-id="a2fe5-113">Оценка фильмов выбрана для Ирландии.</span><span class="sxs-lookup"><span data-stu-id="a2fe5-113">Movies rating selected for Ireland.</span></span> <span data-ttu-id="a2fe5-114">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="a2fe5-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="a2fe5-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="a2fe5-115">tvRating</span></span>|[<span data-ttu-id="a2fe5-116">ратингиреландтелевисионтипе</span><span class="sxs-lookup"><span data-stu-id="a2fe5-116">ratingIrelandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingirelandtelevisiontype.md)|<span data-ttu-id="a2fe5-117">Рейтинг телевизора выбран для Ирландии.</span><span class="sxs-lookup"><span data-stu-id="a2fe5-117">TV rating selected for Ireland.</span></span> <span data-ttu-id="a2fe5-118">Возможные значения: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span><span class="sxs-lookup"><span data-stu-id="a2fe5-118">Possible values are: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a2fe5-119">Связи</span><span class="sxs-lookup"><span data-stu-id="a2fe5-119">Relationships</span></span>
<span data-ttu-id="a2fe5-120">Нет</span><span class="sxs-lookup"><span data-stu-id="a2fe5-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a2fe5-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a2fe5-121">JSON Representation</span></span>
<span data-ttu-id="a2fe5-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a2fe5-122">Here is a JSON representation of the resource.</span></span>
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







