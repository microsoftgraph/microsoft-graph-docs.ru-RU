---
title: Тип ресурса mediaContentRatingFrance
description: Пока не задокументировано.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 979a5996b655ba13847e52dc09b083169ff0815a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32572348"
---
# <a name="mediacontentratingfrance-resource-type"></a><span data-ttu-id="3618c-103">Тип ресурса mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="3618c-103">mediaContentRatingFrance resource type</span></span>

> <span data-ttu-id="3618c-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3618c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3618c-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="3618c-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="3618c-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="3618c-106">Properties</span></span>
|<span data-ttu-id="3618c-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="3618c-107">Property</span></span>|<span data-ttu-id="3618c-108">Тип</span><span class="sxs-lookup"><span data-stu-id="3618c-108">Type</span></span>|<span data-ttu-id="3618c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="3618c-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3618c-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="3618c-110">movieRating</span></span>|[<span data-ttu-id="3618c-111">Ратингфранцемовиестипе</span><span class="sxs-lookup"><span data-stu-id="3618c-111">ratingFranceMoviesType</span></span>](../resources/intune-deviceconfig-ratingfrancemoviestype.md)|<span data-ttu-id="3618c-112">Оценка фильмов выбрана для Франции.</span><span class="sxs-lookup"><span data-stu-id="3618c-112">Movies rating selected for France.</span></span> <span data-ttu-id="3618c-113">Возможные значения: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="3618c-113">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|
|<span data-ttu-id="3618c-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="3618c-114">tvRating</span></span>|[<span data-ttu-id="3618c-115">Ратингфранцетелевисионтипе</span><span class="sxs-lookup"><span data-stu-id="3618c-115">ratingFranceTelevisionType</span></span>](../resources/intune-deviceconfig-ratingfrancetelevisiontype.md)|<span data-ttu-id="3618c-116">Рейтинг телевизора выбран для Франции.</span><span class="sxs-lookup"><span data-stu-id="3618c-116">TV rating selected for France.</span></span> <span data-ttu-id="3618c-117">Возможные значения: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="3618c-117">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3618c-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="3618c-118">Relationships</span></span>
<span data-ttu-id="3618c-119">Нет</span><span class="sxs-lookup"><span data-stu-id="3618c-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3618c-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3618c-120">JSON Representation</span></span>
<span data-ttu-id="3618c-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3618c-121">Here is a JSON representation of the resource.</span></span>
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



