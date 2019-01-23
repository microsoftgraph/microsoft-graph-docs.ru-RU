---
title: Тип ресурса mediaContentRatingGermany
description: Н/Д
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7a5a1b61069aa3568c8cb017c6c28bb3e992c38b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394518"
---
# <a name="mediacontentratinggermany-resource-type"></a><span data-ttu-id="775cb-103">Тип ресурса mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="775cb-103">mediaContentRatingGermany resource type</span></span>

> <span data-ttu-id="775cb-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="775cb-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="775cb-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="775cb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="775cb-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="775cb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="775cb-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="775cb-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="775cb-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="775cb-108">Properties</span></span>
|<span data-ttu-id="775cb-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="775cb-109">Property</span></span>|<span data-ttu-id="775cb-110">Тип</span><span class="sxs-lookup"><span data-stu-id="775cb-110">Type</span></span>|<span data-ttu-id="775cb-111">Описание</span><span class="sxs-lookup"><span data-stu-id="775cb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="775cb-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="775cb-112">movieRating</span></span>|[<span data-ttu-id="775cb-113">ratingGermanyMoviesType</span><span class="sxs-lookup"><span data-stu-id="775cb-113">ratingGermanyMoviesType</span></span>](../resources/intune-deviceconfig-ratinggermanymoviestype.md)|<span data-ttu-id="775cb-114">Оценка выбранных для Германии фильмы.</span><span class="sxs-lookup"><span data-stu-id="775cb-114">Movies rating selected for Germany.</span></span> <span data-ttu-id="775cb-115">Возможные значения: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="775cb-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="775cb-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="775cb-116">tvRating</span></span>|[<span data-ttu-id="775cb-117">ratingGermanyTelevisionType</span><span class="sxs-lookup"><span data-stu-id="775cb-117">ratingGermanyTelevisionType</span></span>](../resources/intune-deviceconfig-ratinggermanytelevisiontype.md)|<span data-ttu-id="775cb-118">Оценка TV, выбранной для Германии.</span><span class="sxs-lookup"><span data-stu-id="775cb-118">TV rating selected for Germany.</span></span> <span data-ttu-id="775cb-119">Возможные значения: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="775cb-119">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="775cb-120">Связи</span><span class="sxs-lookup"><span data-stu-id="775cb-120">Relationships</span></span>
<span data-ttu-id="775cb-121">Нет</span><span class="sxs-lookup"><span data-stu-id="775cb-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="775cb-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="775cb-122">JSON Representation</span></span>
<span data-ttu-id="775cb-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="775cb-123">Here is a JSON representation of the resource.</span></span>
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




