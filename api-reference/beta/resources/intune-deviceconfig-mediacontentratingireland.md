---
title: Тип ресурса mediaContentRatingIreland
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 97275ce5eac5fde8e2c2b3b440960e8d4d003c02
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34980413"
---
# <a name="mediacontentratingireland-resource-type"></a><span data-ttu-id="ca3e4-103">Тип ресурса mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="ca3e4-103">mediaContentRatingIreland resource type</span></span>

> <span data-ttu-id="ca3e4-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca3e4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ca3e4-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ca3e4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ca3e4-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="ca3e4-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="ca3e4-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="ca3e4-107">Properties</span></span>
|<span data-ttu-id="ca3e4-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="ca3e4-108">Property</span></span>|<span data-ttu-id="ca3e4-109">Тип</span><span class="sxs-lookup"><span data-stu-id="ca3e4-109">Type</span></span>|<span data-ttu-id="ca3e4-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ca3e4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca3e4-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="ca3e4-111">movieRating</span></span>|[<span data-ttu-id="ca3e4-112">Ратингиреландмовиестипе</span><span class="sxs-lookup"><span data-stu-id="ca3e4-112">ratingIrelandMoviesType</span></span>](../resources/intune-deviceconfig-ratingirelandmoviestype.md)|<span data-ttu-id="ca3e4-113">Оценка фильмов выбрана для Ирландии.</span><span class="sxs-lookup"><span data-stu-id="ca3e4-113">Movies rating selected for Ireland.</span></span> <span data-ttu-id="ca3e4-114">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="ca3e4-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="ca3e4-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="ca3e4-115">tvRating</span></span>|[<span data-ttu-id="ca3e4-116">Ратингиреландтелевисионтипе</span><span class="sxs-lookup"><span data-stu-id="ca3e4-116">ratingIrelandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingirelandtelevisiontype.md)|<span data-ttu-id="ca3e4-117">Рейтинг телевизора выбран для Ирландии.</span><span class="sxs-lookup"><span data-stu-id="ca3e4-117">TV rating selected for Ireland.</span></span> <span data-ttu-id="ca3e4-118">Возможные значения: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span><span class="sxs-lookup"><span data-stu-id="ca3e4-118">Possible values are: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ca3e4-119">Отношения</span><span class="sxs-lookup"><span data-stu-id="ca3e4-119">Relationships</span></span>
<span data-ttu-id="ca3e4-120">Нет</span><span class="sxs-lookup"><span data-stu-id="ca3e4-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ca3e4-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ca3e4-121">JSON Representation</span></span>
<span data-ttu-id="ca3e4-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ca3e4-122">Here is a JSON representation of the resource.</span></span>
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





