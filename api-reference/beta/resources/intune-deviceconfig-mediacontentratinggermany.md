---
title: Тип ресурса mediaContentRatingGermany
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a43f919bb24d25d0e22dab0ecc192b2b6757f9e7
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30147098"
---
# <a name="mediacontentratinggermany-resource-type"></a><span data-ttu-id="b7211-103">Тип ресурса mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="b7211-103">mediaContentRatingGermany resource type</span></span>

> <span data-ttu-id="b7211-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b7211-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b7211-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b7211-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b7211-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="b7211-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="b7211-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="b7211-107">Properties</span></span>
|<span data-ttu-id="b7211-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="b7211-108">Property</span></span>|<span data-ttu-id="b7211-109">Тип</span><span class="sxs-lookup"><span data-stu-id="b7211-109">Type</span></span>|<span data-ttu-id="b7211-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b7211-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b7211-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="b7211-111">movieRating</span></span>|[<span data-ttu-id="b7211-112">Ратингжерманимовиестипе</span><span class="sxs-lookup"><span data-stu-id="b7211-112">ratingGermanyMoviesType</span></span>](../resources/intune-deviceconfig-ratinggermanymoviestype.md)|<span data-ttu-id="b7211-113">Оценка фильмов выбрана для Германии.</span><span class="sxs-lookup"><span data-stu-id="b7211-113">Movies rating selected for Germany.</span></span> <span data-ttu-id="b7211-114">Возможные значения: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="b7211-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="b7211-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="b7211-115">tvRating</span></span>|[<span data-ttu-id="b7211-116">Ратингжерманителевисионтипе</span><span class="sxs-lookup"><span data-stu-id="b7211-116">ratingGermanyTelevisionType</span></span>](../resources/intune-deviceconfig-ratinggermanytelevisiontype.md)|<span data-ttu-id="b7211-117">Рейтинг для телевизора выбран в Германии.</span><span class="sxs-lookup"><span data-stu-id="b7211-117">TV rating selected for Germany.</span></span> <span data-ttu-id="b7211-118">Возможные значения: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="b7211-118">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b7211-119">Связи</span><span class="sxs-lookup"><span data-stu-id="b7211-119">Relationships</span></span>
<span data-ttu-id="b7211-120">Нет</span><span class="sxs-lookup"><span data-stu-id="b7211-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b7211-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b7211-121">JSON Representation</span></span>
<span data-ttu-id="b7211-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b7211-122">Here is a JSON representation of the resource.</span></span>
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




