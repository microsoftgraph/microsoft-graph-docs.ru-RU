---
title: Тип ресурса mediaContentRatingIreland
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: dc67f39a0cbb42dc42d942bd17387ba1f4e99fd6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530631"
---
# <a name="mediacontentratingireland-resource-type"></a><span data-ttu-id="b22a5-103">Тип ресурса mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="b22a5-103">mediaContentRatingIreland resource type</span></span>

<span data-ttu-id="b22a5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b22a5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b22a5-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b22a5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b22a5-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="b22a5-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="b22a5-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="b22a5-107">Properties</span></span>
|<span data-ttu-id="b22a5-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="b22a5-108">Property</span></span>|<span data-ttu-id="b22a5-109">Тип</span><span class="sxs-lookup"><span data-stu-id="b22a5-109">Type</span></span>|<span data-ttu-id="b22a5-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b22a5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b22a5-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="b22a5-111">movieRating</span></span>|[<span data-ttu-id="b22a5-112">ратингиреландмовиестипе</span><span class="sxs-lookup"><span data-stu-id="b22a5-112">ratingIrelandMoviesType</span></span>](../resources/intune-deviceconfig-ratingirelandmoviestype.md)|<span data-ttu-id="b22a5-113">Оценка фильмов выбрана для Ирландии.</span><span class="sxs-lookup"><span data-stu-id="b22a5-113">Movies rating selected for Ireland.</span></span> <span data-ttu-id="b22a5-114">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="b22a5-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="b22a5-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="b22a5-115">tvRating</span></span>|[<span data-ttu-id="b22a5-116">ратингиреландтелевисионтипе</span><span class="sxs-lookup"><span data-stu-id="b22a5-116">ratingIrelandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingirelandtelevisiontype.md)|<span data-ttu-id="b22a5-117">Рейтинг телевизора выбран для Ирландии.</span><span class="sxs-lookup"><span data-stu-id="b22a5-117">TV rating selected for Ireland.</span></span> <span data-ttu-id="b22a5-118">Возможные значения: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span><span class="sxs-lookup"><span data-stu-id="b22a5-118">Possible values are: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b22a5-119">Связи</span><span class="sxs-lookup"><span data-stu-id="b22a5-119">Relationships</span></span>
<span data-ttu-id="b22a5-120">Нет</span><span class="sxs-lookup"><span data-stu-id="b22a5-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b22a5-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b22a5-121">JSON Representation</span></span>
<span data-ttu-id="b22a5-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b22a5-122">Here is a JSON representation of the resource.</span></span>
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




