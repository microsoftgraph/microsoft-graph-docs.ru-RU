---
title: Тип ресурса mediaContentRatingFrance
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6f071f516174eb851712c2b162df4144c00a2b9a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43410074"
---
# <a name="mediacontentratingfrance-resource-type"></a><span data-ttu-id="e95fd-103">Тип ресурса mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="e95fd-103">mediaContentRatingFrance resource type</span></span>

<span data-ttu-id="e95fd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e95fd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e95fd-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e95fd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e95fd-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="e95fd-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="e95fd-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="e95fd-107">Properties</span></span>
|<span data-ttu-id="e95fd-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="e95fd-108">Property</span></span>|<span data-ttu-id="e95fd-109">Тип</span><span class="sxs-lookup"><span data-stu-id="e95fd-109">Type</span></span>|<span data-ttu-id="e95fd-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e95fd-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e95fd-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="e95fd-111">movieRating</span></span>|[<span data-ttu-id="e95fd-112">ратингфранцемовиестипе</span><span class="sxs-lookup"><span data-stu-id="e95fd-112">ratingFranceMoviesType</span></span>](../resources/intune-deviceconfig-ratingfrancemoviestype.md)|<span data-ttu-id="e95fd-113">Оценка фильмов выбрана для Франции.</span><span class="sxs-lookup"><span data-stu-id="e95fd-113">Movies rating selected for France.</span></span> <span data-ttu-id="e95fd-114">Возможные значения: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="e95fd-114">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|
|<span data-ttu-id="e95fd-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="e95fd-115">tvRating</span></span>|[<span data-ttu-id="e95fd-116">ратингфранцетелевисионтипе</span><span class="sxs-lookup"><span data-stu-id="e95fd-116">ratingFranceTelevisionType</span></span>](../resources/intune-deviceconfig-ratingfrancetelevisiontype.md)|<span data-ttu-id="e95fd-117">Рейтинг телевизора выбран для Франции.</span><span class="sxs-lookup"><span data-stu-id="e95fd-117">TV rating selected for France.</span></span> <span data-ttu-id="e95fd-118">Возможные значения: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="e95fd-118">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e95fd-119">Связи</span><span class="sxs-lookup"><span data-stu-id="e95fd-119">Relationships</span></span>
<span data-ttu-id="e95fd-120">Нет</span><span class="sxs-lookup"><span data-stu-id="e95fd-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e95fd-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e95fd-121">JSON Representation</span></span>
<span data-ttu-id="e95fd-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e95fd-122">Here is a JSON representation of the resource.</span></span>
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







