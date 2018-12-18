---
title: Тип ресурса mediaContentRatingNewZealand
description: Н/Д
author: tfitzmac
ms.openlocfilehash: 5daba568ee435c32cc0b3d491c1cedcc61294603
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27356107"
---
# <a name="mediacontentratingnewzealand-resource-type"></a><span data-ttu-id="f13a7-103">Тип ресурса mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="f13a7-103">mediaContentRatingNewZealand resource type</span></span>

> <span data-ttu-id="f13a7-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f13a7-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f13a7-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="f13a7-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="f13a7-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="f13a7-106">Properties</span></span>
|<span data-ttu-id="f13a7-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="f13a7-107">Property</span></span>|<span data-ttu-id="f13a7-108">Тип</span><span class="sxs-lookup"><span data-stu-id="f13a7-108">Type</span></span>|<span data-ttu-id="f13a7-109">Описание</span><span class="sxs-lookup"><span data-stu-id="f13a7-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f13a7-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="f13a7-110">movieRating</span></span>|[<span data-ttu-id="f13a7-111">ratingNewZealandMoviesType</span><span class="sxs-lookup"><span data-stu-id="f13a7-111">ratingNewZealandMoviesType</span></span>](../resources/intune-deviceconfig-ratingnewzealandmoviestype.md)|<span data-ttu-id="f13a7-112">Оценка выбранных для новой Зеландии фильмы.</span><span class="sxs-lookup"><span data-stu-id="f13a7-112">Movies rating selected for New Zealand.</span></span> <span data-ttu-id="f13a7-113">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span><span class="sxs-lookup"><span data-stu-id="f13a7-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span></span>|
|<span data-ttu-id="f13a7-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="f13a7-114">tvRating</span></span>|[<span data-ttu-id="f13a7-115">ratingNewZealandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="f13a7-115">ratingNewZealandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingnewzealandtelevisiontype.md)|<span data-ttu-id="f13a7-116">Оценка TV, выбранной для новой Зеландии.</span><span class="sxs-lookup"><span data-stu-id="f13a7-116">TV rating selected for New Zealand.</span></span> <span data-ttu-id="f13a7-117">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="f13a7-117">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f13a7-118">Связи</span><span class="sxs-lookup"><span data-stu-id="f13a7-118">Relationships</span></span>
<span data-ttu-id="f13a7-119">Нет</span><span class="sxs-lookup"><span data-stu-id="f13a7-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f13a7-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f13a7-120">JSON Representation</span></span>
<span data-ttu-id="f13a7-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f13a7-121">Here is a JSON representation of the resource.</span></span>
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



