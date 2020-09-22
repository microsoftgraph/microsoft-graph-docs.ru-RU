---
title: Тип ресурса mediaContentRatingFrance
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 44b6374d4831ca0b3b220f237a3c8d9938df18e7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48003145"
---
# <a name="mediacontentratingfrance-resource-type"></a><span data-ttu-id="0a588-103">Тип ресурса mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="0a588-103">mediaContentRatingFrance resource type</span></span>

<span data-ttu-id="0a588-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0a588-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0a588-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0a588-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0a588-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="0a588-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="0a588-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="0a588-107">Properties</span></span>
|<span data-ttu-id="0a588-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="0a588-108">Property</span></span>|<span data-ttu-id="0a588-109">Тип</span><span class="sxs-lookup"><span data-stu-id="0a588-109">Type</span></span>|<span data-ttu-id="0a588-110">Описание</span><span class="sxs-lookup"><span data-stu-id="0a588-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a588-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="0a588-111">movieRating</span></span>|[<span data-ttu-id="0a588-112">ратингфранцемовиестипе</span><span class="sxs-lookup"><span data-stu-id="0a588-112">ratingFranceMoviesType</span></span>](../resources/intune-deviceconfig-ratingfrancemoviestype.md)|<span data-ttu-id="0a588-113">Оценка фильмов выбрана для Франции.</span><span class="sxs-lookup"><span data-stu-id="0a588-113">Movies rating selected for France.</span></span> <span data-ttu-id="0a588-114">Возможные значения: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="0a588-114">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|
|<span data-ttu-id="0a588-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="0a588-115">tvRating</span></span>|[<span data-ttu-id="0a588-116">ратингфранцетелевисионтипе</span><span class="sxs-lookup"><span data-stu-id="0a588-116">ratingFranceTelevisionType</span></span>](../resources/intune-deviceconfig-ratingfrancetelevisiontype.md)|<span data-ttu-id="0a588-117">Рейтинг телевизора выбран для Франции.</span><span class="sxs-lookup"><span data-stu-id="0a588-117">TV rating selected for France.</span></span> <span data-ttu-id="0a588-118">Возможные значения: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="0a588-118">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0a588-119">Связи</span><span class="sxs-lookup"><span data-stu-id="0a588-119">Relationships</span></span>
<span data-ttu-id="0a588-120">Нет</span><span class="sxs-lookup"><span data-stu-id="0a588-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0a588-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0a588-121">JSON Representation</span></span>
<span data-ttu-id="0a588-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0a588-122">Here is a JSON representation of the resource.</span></span>
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









