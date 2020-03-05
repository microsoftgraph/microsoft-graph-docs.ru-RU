---
title: Тип ресурса mediaContentRatingFrance
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4f7505ad8413fbcbb57c809ed1db9fa8510124c1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42418141"
---
# <a name="mediacontentratingfrance-resource-type"></a><span data-ttu-id="b2cd6-103">Тип ресурса mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="b2cd6-103">mediaContentRatingFrance resource type</span></span>

<span data-ttu-id="b2cd6-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b2cd6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b2cd6-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b2cd6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2cd6-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="b2cd6-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="b2cd6-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="b2cd6-107">Properties</span></span>
|<span data-ttu-id="b2cd6-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="b2cd6-108">Property</span></span>|<span data-ttu-id="b2cd6-109">Тип</span><span class="sxs-lookup"><span data-stu-id="b2cd6-109">Type</span></span>|<span data-ttu-id="b2cd6-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b2cd6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2cd6-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="b2cd6-111">movieRating</span></span>|[<span data-ttu-id="b2cd6-112">ратингфранцемовиестипе</span><span class="sxs-lookup"><span data-stu-id="b2cd6-112">ratingFranceMoviesType</span></span>](../resources/intune-deviceconfig-ratingfrancemoviestype.md)|<span data-ttu-id="b2cd6-113">Оценка фильмов выбрана для Франции.</span><span class="sxs-lookup"><span data-stu-id="b2cd6-113">Movies rating selected for France.</span></span> <span data-ttu-id="b2cd6-114">Возможные значения: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="b2cd6-114">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|
|<span data-ttu-id="b2cd6-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="b2cd6-115">tvRating</span></span>|[<span data-ttu-id="b2cd6-116">ратингфранцетелевисионтипе</span><span class="sxs-lookup"><span data-stu-id="b2cd6-116">ratingFranceTelevisionType</span></span>](../resources/intune-deviceconfig-ratingfrancetelevisiontype.md)|<span data-ttu-id="b2cd6-117">Рейтинг телевизора выбран для Франции.</span><span class="sxs-lookup"><span data-stu-id="b2cd6-117">TV rating selected for France.</span></span> <span data-ttu-id="b2cd6-118">Возможные значения: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="b2cd6-118">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b2cd6-119">Связи</span><span class="sxs-lookup"><span data-stu-id="b2cd6-119">Relationships</span></span>
<span data-ttu-id="b2cd6-120">Нет</span><span class="sxs-lookup"><span data-stu-id="b2cd6-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b2cd6-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b2cd6-121">JSON Representation</span></span>
<span data-ttu-id="b2cd6-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b2cd6-122">Here is a JSON representation of the resource.</span></span>
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




