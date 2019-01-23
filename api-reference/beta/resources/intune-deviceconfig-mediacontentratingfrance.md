---
title: Тип ресурса mediaContentRatingFrance
description: Н/Д
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: bb199abfc350a8b88913e353d377745714368c95
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412368"
---
# <a name="mediacontentratingfrance-resource-type"></a><span data-ttu-id="f3bdd-103">Тип ресурса mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="f3bdd-103">mediaContentRatingFrance resource type</span></span>

> <span data-ttu-id="f3bdd-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f3bdd-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f3bdd-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3bdd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f3bdd-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f3bdd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3bdd-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="f3bdd-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="f3bdd-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="f3bdd-108">Properties</span></span>
|<span data-ttu-id="f3bdd-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="f3bdd-109">Property</span></span>|<span data-ttu-id="f3bdd-110">Тип</span><span class="sxs-lookup"><span data-stu-id="f3bdd-110">Type</span></span>|<span data-ttu-id="f3bdd-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f3bdd-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3bdd-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="f3bdd-112">movieRating</span></span>|[<span data-ttu-id="f3bdd-113">ratingFranceMoviesType</span><span class="sxs-lookup"><span data-stu-id="f3bdd-113">ratingFranceMoviesType</span></span>](../resources/intune-deviceconfig-ratingfrancemoviestype.md)|<span data-ttu-id="f3bdd-114">Оценка выбранных для Франции фильмы.</span><span class="sxs-lookup"><span data-stu-id="f3bdd-114">Movies rating selected for France.</span></span> <span data-ttu-id="f3bdd-115">Возможные значения: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="f3bdd-115">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|
|<span data-ttu-id="f3bdd-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="f3bdd-116">tvRating</span></span>|[<span data-ttu-id="f3bdd-117">ratingFranceTelevisionType</span><span class="sxs-lookup"><span data-stu-id="f3bdd-117">ratingFranceTelevisionType</span></span>](../resources/intune-deviceconfig-ratingfrancetelevisiontype.md)|<span data-ttu-id="f3bdd-118">Оценка TV, выбранной для Франции.</span><span class="sxs-lookup"><span data-stu-id="f3bdd-118">TV rating selected for France.</span></span> <span data-ttu-id="f3bdd-119">Возможные значения: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="f3bdd-119">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f3bdd-120">Отношения</span><span class="sxs-lookup"><span data-stu-id="f3bdd-120">Relationships</span></span>
<span data-ttu-id="f3bdd-121">Нет</span><span class="sxs-lookup"><span data-stu-id="f3bdd-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f3bdd-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f3bdd-122">JSON Representation</span></span>
<span data-ttu-id="f3bdd-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f3bdd-123">Here is a JSON representation of the resource.</span></span>
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




