---
title: Тип ресурса mediaContentRatingNewZealand
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9328ccc8b3c6b7ce6af220d8f798497e00448a8b
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30159278"
---
# <a name="mediacontentratingnewzealand-resource-type"></a><span data-ttu-id="2b21b-103">Тип ресурса mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="2b21b-103">mediaContentRatingNewZealand resource type</span></span>

> <span data-ttu-id="2b21b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b21b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2b21b-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2b21b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2b21b-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="2b21b-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="2b21b-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="2b21b-107">Properties</span></span>
|<span data-ttu-id="2b21b-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="2b21b-108">Property</span></span>|<span data-ttu-id="2b21b-109">Тип</span><span class="sxs-lookup"><span data-stu-id="2b21b-109">Type</span></span>|<span data-ttu-id="2b21b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2b21b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b21b-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="2b21b-111">movieRating</span></span>|[<span data-ttu-id="2b21b-112">Ратингневзеаландмовиестипе</span><span class="sxs-lookup"><span data-stu-id="2b21b-112">ratingNewZealandMoviesType</span></span>](../resources/intune-deviceconfig-ratingnewzealandmoviestype.md)|<span data-ttu-id="2b21b-113">Рейтинг фильмов, выбранный для Новой Зеландии.</span><span class="sxs-lookup"><span data-stu-id="2b21b-113">Movies rating selected for New Zealand.</span></span> <span data-ttu-id="2b21b-114">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span><span class="sxs-lookup"><span data-stu-id="2b21b-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span></span>|
|<span data-ttu-id="2b21b-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="2b21b-115">tvRating</span></span>|[<span data-ttu-id="2b21b-116">Ратингневзеаландтелевисионтипе</span><span class="sxs-lookup"><span data-stu-id="2b21b-116">ratingNewZealandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingnewzealandtelevisiontype.md)|<span data-ttu-id="2b21b-117">Рейтинг для телевизора, выбранный для Новой Зеландии.</span><span class="sxs-lookup"><span data-stu-id="2b21b-117">TV rating selected for New Zealand.</span></span> <span data-ttu-id="2b21b-118">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="2b21b-118">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2b21b-119">Отношения</span><span class="sxs-lookup"><span data-stu-id="2b21b-119">Relationships</span></span>
<span data-ttu-id="2b21b-120">Нет</span><span class="sxs-lookup"><span data-stu-id="2b21b-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2b21b-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2b21b-121">JSON Representation</span></span>
<span data-ttu-id="2b21b-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2b21b-122">Here is a JSON representation of the resource.</span></span>
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




