---
title: Тип ресурса mediaContentRatingFrance
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 724fe7a511616b457d29cd804c19d69705bfb42b
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52757775"
---
# <a name="mediacontentratingfrance-resource-type"></a><span data-ttu-id="295d9-103">Тип ресурса mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="295d9-103">mediaContentRatingFrance resource type</span></span>

<span data-ttu-id="295d9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="295d9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="295d9-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="295d9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="295d9-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="295d9-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="295d9-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="295d9-107">Properties</span></span>
|<span data-ttu-id="295d9-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="295d9-108">Property</span></span>|<span data-ttu-id="295d9-109">Тип</span><span class="sxs-lookup"><span data-stu-id="295d9-109">Type</span></span>|<span data-ttu-id="295d9-110">Описание</span><span class="sxs-lookup"><span data-stu-id="295d9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="295d9-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="295d9-111">movieRating</span></span>|[<span data-ttu-id="295d9-112">ratingFranceMoviesType</span><span class="sxs-lookup"><span data-stu-id="295d9-112">ratingFranceMoviesType</span></span>](../resources/intune-deviceconfig-ratingfrancemoviestype.md)|<span data-ttu-id="295d9-113">Рейтинг фильмов, выбранный для Франции.</span><span class="sxs-lookup"><span data-stu-id="295d9-113">Movies rating selected for France.</span></span> <span data-ttu-id="295d9-114">Возможные значения: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="295d9-114">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|
|<span data-ttu-id="295d9-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="295d9-115">tvRating</span></span>|[<span data-ttu-id="295d9-116">ratingFranceTelevisionType</span><span class="sxs-lookup"><span data-stu-id="295d9-116">ratingFranceTelevisionType</span></span>](../resources/intune-deviceconfig-ratingfrancetelevisiontype.md)|<span data-ttu-id="295d9-117">Телевизионный рейтинг, выбранный для Франции.</span><span class="sxs-lookup"><span data-stu-id="295d9-117">TV rating selected for France.</span></span> <span data-ttu-id="295d9-118">Возможные значения: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="295d9-118">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="295d9-119">Отношения</span><span class="sxs-lookup"><span data-stu-id="295d9-119">Relationships</span></span>
<span data-ttu-id="295d9-120">Нет</span><span class="sxs-lookup"><span data-stu-id="295d9-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="295d9-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="295d9-121">JSON Representation</span></span>
<span data-ttu-id="295d9-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="295d9-122">Here is a JSON representation of the resource.</span></span>
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




