---
title: Тип ресурса mediaContentRatingFrance
description: Н/Д
ms.openlocfilehash: bd2f4933ea05c7db193d700799cdcbdc79490356
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025024"
---
# <a name="mediacontentratingfrance-resource-type"></a><span data-ttu-id="c0428-103">Тип ресурса mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="c0428-103">mediaContentRatingFrance resource type</span></span>

> <span data-ttu-id="c0428-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c0428-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c0428-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="c0428-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="c0428-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="c0428-106">Properties</span></span>
|<span data-ttu-id="c0428-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="c0428-107">Property</span></span>|<span data-ttu-id="c0428-108">Тип</span><span class="sxs-lookup"><span data-stu-id="c0428-108">Type</span></span>|<span data-ttu-id="c0428-109">Описание</span><span class="sxs-lookup"><span data-stu-id="c0428-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0428-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="c0428-110">movieRating</span></span>|[<span data-ttu-id="c0428-111">ratingFranceMoviesType</span><span class="sxs-lookup"><span data-stu-id="c0428-111">ratingFranceMoviesType</span></span>](../resources/intune-deviceconfig-ratingfrancemoviestype.md)|<span data-ttu-id="c0428-112">Оценка выбранных для Франции фильмы.</span><span class="sxs-lookup"><span data-stu-id="c0428-112">Movies rating selected for France.</span></span> <span data-ttu-id="c0428-113">Возможные значения: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="c0428-113">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|
|<span data-ttu-id="c0428-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="c0428-114">tvRating</span></span>|[<span data-ttu-id="c0428-115">ratingFranceTelevisionType</span><span class="sxs-lookup"><span data-stu-id="c0428-115">ratingFranceTelevisionType</span></span>](../resources/intune-deviceconfig-ratingfrancetelevisiontype.md)|<span data-ttu-id="c0428-116">Оценка TV, выбранной для Франции.</span><span class="sxs-lookup"><span data-stu-id="c0428-116">TV rating selected for France.</span></span> <span data-ttu-id="c0428-117">Возможные значения: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="c0428-117">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c0428-118">Связи</span><span class="sxs-lookup"><span data-stu-id="c0428-118">Relationships</span></span>
<span data-ttu-id="c0428-119">Нет</span><span class="sxs-lookup"><span data-stu-id="c0428-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c0428-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c0428-120">JSON Representation</span></span>
<span data-ttu-id="c0428-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c0428-121">Here is a JSON representation of the resource.</span></span>
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



