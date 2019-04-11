---
title: Тип ресурса mediaContentRatingNewZealand
description: Пока не задокументировано.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d1d2b608a285413e8ad4f7049d06982a06878450
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31807170"
---
# <a name="mediacontentratingnewzealand-resource-type"></a><span data-ttu-id="c072d-103">Тип ресурса mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="c072d-103">mediaContentRatingNewZealand resource type</span></span>

> <span data-ttu-id="c072d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c072d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c072d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c072d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c072d-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="c072d-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="c072d-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="c072d-107">Properties</span></span>
|<span data-ttu-id="c072d-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="c072d-108">Property</span></span>|<span data-ttu-id="c072d-109">Тип</span><span class="sxs-lookup"><span data-stu-id="c072d-109">Type</span></span>|<span data-ttu-id="c072d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c072d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c072d-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="c072d-111">movieRating</span></span>|[<span data-ttu-id="c072d-112">Ратингневзеаландмовиестипе</span><span class="sxs-lookup"><span data-stu-id="c072d-112">ratingNewZealandMoviesType</span></span>](../resources/intune-deviceconfig-ratingnewzealandmoviestype.md)|<span data-ttu-id="c072d-113">Рейтинг фильмов, выбранный для Новой Зеландии.</span><span class="sxs-lookup"><span data-stu-id="c072d-113">Movies rating selected for New Zealand.</span></span> <span data-ttu-id="c072d-114">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span><span class="sxs-lookup"><span data-stu-id="c072d-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span></span>|
|<span data-ttu-id="c072d-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="c072d-115">tvRating</span></span>|[<span data-ttu-id="c072d-116">Ратингневзеаландтелевисионтипе</span><span class="sxs-lookup"><span data-stu-id="c072d-116">ratingNewZealandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingnewzealandtelevisiontype.md)|<span data-ttu-id="c072d-117">Рейтинг для телевизора, выбранный для Новой Зеландии.</span><span class="sxs-lookup"><span data-stu-id="c072d-117">TV rating selected for New Zealand.</span></span> <span data-ttu-id="c072d-118">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="c072d-118">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c072d-119">Отношения</span><span class="sxs-lookup"><span data-stu-id="c072d-119">Relationships</span></span>
<span data-ttu-id="c072d-120">Нет</span><span class="sxs-lookup"><span data-stu-id="c072d-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c072d-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c072d-121">JSON Representation</span></span>
<span data-ttu-id="c072d-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c072d-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingNewZealand"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingNewZealand",
  "movieRating": "String",
  "tvRating": "String"
}
```





