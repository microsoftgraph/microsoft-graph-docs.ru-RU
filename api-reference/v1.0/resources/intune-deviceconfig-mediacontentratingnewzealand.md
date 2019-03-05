---
title: Тип ресурса mediaContentRatingNewZealand
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4c2d9d58413153699f93841470364cb673979a17
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30253402"
---
# <a name="mediacontentratingnewzealand-resource-type"></a><span data-ttu-id="3fd23-103">Тип ресурса mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="3fd23-103">mediaContentRatingNewZealand resource type</span></span>

> <span data-ttu-id="3fd23-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3fd23-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3fd23-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="3fd23-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="3fd23-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="3fd23-106">Properties</span></span>
|<span data-ttu-id="3fd23-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="3fd23-107">Property</span></span>|<span data-ttu-id="3fd23-108">Тип</span><span class="sxs-lookup"><span data-stu-id="3fd23-108">Type</span></span>|<span data-ttu-id="3fd23-109">Описание</span><span class="sxs-lookup"><span data-stu-id="3fd23-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3fd23-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="3fd23-110">movieRating</span></span>|[<span data-ttu-id="3fd23-111">Ратингневзеаландмовиестипе</span><span class="sxs-lookup"><span data-stu-id="3fd23-111">ratingNewZealandMoviesType</span></span>](../resources/intune-deviceconfig-ratingnewzealandmoviestype.md)|<span data-ttu-id="3fd23-112">Рейтинг фильмов, выбранный для Новой Зеландии.</span><span class="sxs-lookup"><span data-stu-id="3fd23-112">Movies rating selected for New Zealand.</span></span> <span data-ttu-id="3fd23-113">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span><span class="sxs-lookup"><span data-stu-id="3fd23-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span></span>|
|<span data-ttu-id="3fd23-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="3fd23-114">tvRating</span></span>|[<span data-ttu-id="3fd23-115">Ратингневзеаландтелевисионтипе</span><span class="sxs-lookup"><span data-stu-id="3fd23-115">ratingNewZealandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingnewzealandtelevisiontype.md)|<span data-ttu-id="3fd23-116">Рейтинг для телевизора, выбранный для Новой Зеландии.</span><span class="sxs-lookup"><span data-stu-id="3fd23-116">TV rating selected for New Zealand.</span></span> <span data-ttu-id="3fd23-117">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="3fd23-117">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3fd23-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="3fd23-118">Relationships</span></span>
<span data-ttu-id="3fd23-119">Нет</span><span class="sxs-lookup"><span data-stu-id="3fd23-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3fd23-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3fd23-120">JSON Representation</span></span>
<span data-ttu-id="3fd23-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3fd23-121">Here is a JSON representation of the resource.</span></span>
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



