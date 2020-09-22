---
title: Тип ресурса mediaContentRatingNewZealand
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2860f308cb25b679ea12b2b2d978cf15dc87c40a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48003096"
---
# <a name="mediacontentratingnewzealand-resource-type"></a><span data-ttu-id="b98df-103">Тип ресурса mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="b98df-103">mediaContentRatingNewZealand resource type</span></span>

<span data-ttu-id="b98df-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b98df-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b98df-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b98df-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b98df-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="b98df-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="b98df-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="b98df-107">Properties</span></span>
|<span data-ttu-id="b98df-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="b98df-108">Property</span></span>|<span data-ttu-id="b98df-109">Тип</span><span class="sxs-lookup"><span data-stu-id="b98df-109">Type</span></span>|<span data-ttu-id="b98df-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b98df-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b98df-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="b98df-111">movieRating</span></span>|[<span data-ttu-id="b98df-112">ратингневзеаландмовиестипе</span><span class="sxs-lookup"><span data-stu-id="b98df-112">ratingNewZealandMoviesType</span></span>](../resources/intune-deviceconfig-ratingnewzealandmoviestype.md)|<span data-ttu-id="b98df-113">Рейтинг фильмов, выбранный для Новой Зеландии.</span><span class="sxs-lookup"><span data-stu-id="b98df-113">Movies rating selected for New Zealand.</span></span> <span data-ttu-id="b98df-114">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span><span class="sxs-lookup"><span data-stu-id="b98df-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span></span>|
|<span data-ttu-id="b98df-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="b98df-115">tvRating</span></span>|[<span data-ttu-id="b98df-116">ратингневзеаландтелевисионтипе</span><span class="sxs-lookup"><span data-stu-id="b98df-116">ratingNewZealandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingnewzealandtelevisiontype.md)|<span data-ttu-id="b98df-117">Рейтинг для телевизора, выбранный для Новой Зеландии.</span><span class="sxs-lookup"><span data-stu-id="b98df-117">TV rating selected for New Zealand.</span></span> <span data-ttu-id="b98df-118">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="b98df-118">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b98df-119">Связи</span><span class="sxs-lookup"><span data-stu-id="b98df-119">Relationships</span></span>
<span data-ttu-id="b98df-120">Нет</span><span class="sxs-lookup"><span data-stu-id="b98df-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b98df-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b98df-121">JSON Representation</span></span>
<span data-ttu-id="b98df-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b98df-122">Here is a JSON representation of the resource.</span></span>
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









