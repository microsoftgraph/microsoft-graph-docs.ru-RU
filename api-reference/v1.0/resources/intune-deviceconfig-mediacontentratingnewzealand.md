---
title: Тип ресурса mediaContentRatingNewZealand
description: Пока не задокументировано.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9d06658905a5a6e5aaab79bb159a87fe4cb5cf7a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031397"
---
# <a name="mediacontentratingnewzealand-resource-type"></a><span data-ttu-id="e4917-103">Тип ресурса mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="e4917-103">mediaContentRatingNewZealand resource type</span></span>

> <span data-ttu-id="e4917-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e4917-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e4917-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="e4917-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="e4917-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="e4917-106">Properties</span></span>
|<span data-ttu-id="e4917-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="e4917-107">Property</span></span>|<span data-ttu-id="e4917-108">Тип</span><span class="sxs-lookup"><span data-stu-id="e4917-108">Type</span></span>|<span data-ttu-id="e4917-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e4917-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4917-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="e4917-110">movieRating</span></span>|[<span data-ttu-id="e4917-111">Ратингневзеаландмовиестипе</span><span class="sxs-lookup"><span data-stu-id="e4917-111">ratingNewZealandMoviesType</span></span>](../resources/intune-deviceconfig-ratingnewzealandmoviestype.md)|<span data-ttu-id="e4917-112">Рейтинг фильмов, выбранный для Новой Зеландии.</span><span class="sxs-lookup"><span data-stu-id="e4917-112">Movies rating selected for New Zealand.</span></span> <span data-ttu-id="e4917-113">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span><span class="sxs-lookup"><span data-stu-id="e4917-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span></span>|
|<span data-ttu-id="e4917-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="e4917-114">tvRating</span></span>|[<span data-ttu-id="e4917-115">Ратингневзеаландтелевисионтипе</span><span class="sxs-lookup"><span data-stu-id="e4917-115">ratingNewZealandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingnewzealandtelevisiontype.md)|<span data-ttu-id="e4917-116">Рейтинг для телевизора, выбранный для Новой Зеландии.</span><span class="sxs-lookup"><span data-stu-id="e4917-116">TV rating selected for New Zealand.</span></span> <span data-ttu-id="e4917-117">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="e4917-117">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e4917-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="e4917-118">Relationships</span></span>
<span data-ttu-id="e4917-119">Нет</span><span class="sxs-lookup"><span data-stu-id="e4917-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e4917-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e4917-120">JSON Representation</span></span>
<span data-ttu-id="e4917-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e4917-121">Here is a JSON representation of the resource.</span></span>
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



