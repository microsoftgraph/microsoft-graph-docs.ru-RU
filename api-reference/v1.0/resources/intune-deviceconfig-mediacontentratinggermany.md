---
title: Тип ресурса mediaContentRatingGermany
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9f60f7fa3abfd5cb23735ba8d87d492e5b752d16
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27945134"
---
# <a name="mediacontentratinggermany-resource-type"></a><span data-ttu-id="8617a-103">Тип ресурса mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="8617a-103">mediaContentRatingGermany resource type</span></span>

> <span data-ttu-id="8617a-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8617a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8617a-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="8617a-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="8617a-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="8617a-106">Properties</span></span>
|<span data-ttu-id="8617a-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="8617a-107">Property</span></span>|<span data-ttu-id="8617a-108">Тип</span><span class="sxs-lookup"><span data-stu-id="8617a-108">Type</span></span>|<span data-ttu-id="8617a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="8617a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8617a-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="8617a-110">movieRating</span></span>|[<span data-ttu-id="8617a-111">ratingGermanyMoviesType</span><span class="sxs-lookup"><span data-stu-id="8617a-111">ratingGermanyMoviesType</span></span>](../resources/intune-deviceconfig-ratinggermanymoviestype.md)|<span data-ttu-id="8617a-112">Оценка выбранных для Германии фильмы.</span><span class="sxs-lookup"><span data-stu-id="8617a-112">Movies rating selected for Germany.</span></span> <span data-ttu-id="8617a-113">Возможные значения: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="8617a-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="8617a-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="8617a-114">tvRating</span></span>|[<span data-ttu-id="8617a-115">ratingGermanyTelevisionType</span><span class="sxs-lookup"><span data-stu-id="8617a-115">ratingGermanyTelevisionType</span></span>](../resources/intune-deviceconfig-ratinggermanytelevisiontype.md)|<span data-ttu-id="8617a-116">Оценка TV, выбранной для Германии.</span><span class="sxs-lookup"><span data-stu-id="8617a-116">TV rating selected for Germany.</span></span> <span data-ttu-id="8617a-117">Возможные значения: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="8617a-117">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8617a-118">Связи</span><span class="sxs-lookup"><span data-stu-id="8617a-118">Relationships</span></span>
<span data-ttu-id="8617a-119">Нет</span><span class="sxs-lookup"><span data-stu-id="8617a-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8617a-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8617a-120">JSON Representation</span></span>
<span data-ttu-id="8617a-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8617a-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingGermany"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingGermany",
  "movieRating": "String",
  "tvRating": "String"
}
```



