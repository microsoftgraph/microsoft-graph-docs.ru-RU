---
title: Тип ресурса mediaContentRatingNewZealand
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5d4a22f9510a615dab746912aed1de5123184ca3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27850549"
---
# <a name="mediacontentratingnewzealand-resource-type"></a><span data-ttu-id="68298-103">Тип ресурса mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="68298-103">mediaContentRatingNewZealand resource type</span></span>

> <span data-ttu-id="68298-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="68298-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="68298-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="68298-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="68298-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="68298-106">Properties</span></span>
|<span data-ttu-id="68298-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="68298-107">Property</span></span>|<span data-ttu-id="68298-108">Тип</span><span class="sxs-lookup"><span data-stu-id="68298-108">Type</span></span>|<span data-ttu-id="68298-109">Описание</span><span class="sxs-lookup"><span data-stu-id="68298-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68298-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="68298-110">movieRating</span></span>|[<span data-ttu-id="68298-111">ratingNewZealandMoviesType</span><span class="sxs-lookup"><span data-stu-id="68298-111">ratingNewZealandMoviesType</span></span>](../resources/intune-deviceconfig-ratingnewzealandmoviestype.md)|<span data-ttu-id="68298-112">Оценка выбранных для новой Зеландии фильмы.</span><span class="sxs-lookup"><span data-stu-id="68298-112">Movies rating selected for New Zealand.</span></span> <span data-ttu-id="68298-113">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span><span class="sxs-lookup"><span data-stu-id="68298-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span></span>|
|<span data-ttu-id="68298-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="68298-114">tvRating</span></span>|[<span data-ttu-id="68298-115">ratingNewZealandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="68298-115">ratingNewZealandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingnewzealandtelevisiontype.md)|<span data-ttu-id="68298-116">Оценка TV, выбранной для новой Зеландии.</span><span class="sxs-lookup"><span data-stu-id="68298-116">TV rating selected for New Zealand.</span></span> <span data-ttu-id="68298-117">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="68298-117">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="68298-118">Связи</span><span class="sxs-lookup"><span data-stu-id="68298-118">Relationships</span></span>
<span data-ttu-id="68298-119">Нет</span><span class="sxs-lookup"><span data-stu-id="68298-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="68298-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="68298-120">JSON Representation</span></span>
<span data-ttu-id="68298-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="68298-121">Here is a JSON representation of the resource.</span></span>
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



