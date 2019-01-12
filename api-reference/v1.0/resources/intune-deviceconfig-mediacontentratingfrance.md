---
title: Тип ресурса mediaContentRatingFrance
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4f6fe2e4f4ca0f629ac0d4dbc387aab68122896c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27913116"
---
# <a name="mediacontentratingfrance-resource-type"></a><span data-ttu-id="18e57-103">Тип ресурса mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="18e57-103">mediaContentRatingFrance resource type</span></span>

> <span data-ttu-id="18e57-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="18e57-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="18e57-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="18e57-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="18e57-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="18e57-106">Properties</span></span>
|<span data-ttu-id="18e57-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="18e57-107">Property</span></span>|<span data-ttu-id="18e57-108">Тип</span><span class="sxs-lookup"><span data-stu-id="18e57-108">Type</span></span>|<span data-ttu-id="18e57-109">Описание</span><span class="sxs-lookup"><span data-stu-id="18e57-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18e57-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="18e57-110">movieRating</span></span>|[<span data-ttu-id="18e57-111">ratingFranceMoviesType</span><span class="sxs-lookup"><span data-stu-id="18e57-111">ratingFranceMoviesType</span></span>](../resources/intune-deviceconfig-ratingfrancemoviestype.md)|<span data-ttu-id="18e57-112">Оценка выбранных для Франции фильмы.</span><span class="sxs-lookup"><span data-stu-id="18e57-112">Movies rating selected for France.</span></span> <span data-ttu-id="18e57-113">Возможные значения: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="18e57-113">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|
|<span data-ttu-id="18e57-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="18e57-114">tvRating</span></span>|[<span data-ttu-id="18e57-115">ratingFranceTelevisionType</span><span class="sxs-lookup"><span data-stu-id="18e57-115">ratingFranceTelevisionType</span></span>](../resources/intune-deviceconfig-ratingfrancetelevisiontype.md)|<span data-ttu-id="18e57-116">Оценка TV, выбранной для Франции.</span><span class="sxs-lookup"><span data-stu-id="18e57-116">TV rating selected for France.</span></span> <span data-ttu-id="18e57-117">Возможные значения: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="18e57-117">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="18e57-118">Связи</span><span class="sxs-lookup"><span data-stu-id="18e57-118">Relationships</span></span>
<span data-ttu-id="18e57-119">Нет</span><span class="sxs-lookup"><span data-stu-id="18e57-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="18e57-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="18e57-120">JSON Representation</span></span>
<span data-ttu-id="18e57-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="18e57-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingFrance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingFrance",
  "movieRating": "String",
  "tvRating": "String"
}
```



