---
title: Тип ресурса mediaContentRatingFrance
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7aa3c16df6b32f5c5c50f53959aaccc767b39bbd
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27928145"
---
# <a name="mediacontentratingfrance-resource-type"></a><span data-ttu-id="f27ca-103">Тип ресурса mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="f27ca-103">mediaContentRatingFrance resource type</span></span>

> <span data-ttu-id="f27ca-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f27ca-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f27ca-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f27ca-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f27ca-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f27ca-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f27ca-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="f27ca-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="f27ca-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="f27ca-108">Properties</span></span>
|<span data-ttu-id="f27ca-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="f27ca-109">Property</span></span>|<span data-ttu-id="f27ca-110">Тип</span><span class="sxs-lookup"><span data-stu-id="f27ca-110">Type</span></span>|<span data-ttu-id="f27ca-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f27ca-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f27ca-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="f27ca-112">movieRating</span></span>|[<span data-ttu-id="f27ca-113">ratingFranceMoviesType</span><span class="sxs-lookup"><span data-stu-id="f27ca-113">ratingFranceMoviesType</span></span>](../resources/intune-deviceconfig-ratingfrancemoviestype.md)|<span data-ttu-id="f27ca-114">Оценка выбранных для Франции фильмы.</span><span class="sxs-lookup"><span data-stu-id="f27ca-114">Movies rating selected for France.</span></span> <span data-ttu-id="f27ca-115">Возможные значения: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="f27ca-115">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|
|<span data-ttu-id="f27ca-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="f27ca-116">tvRating</span></span>|[<span data-ttu-id="f27ca-117">ratingFranceTelevisionType</span><span class="sxs-lookup"><span data-stu-id="f27ca-117">ratingFranceTelevisionType</span></span>](../resources/intune-deviceconfig-ratingfrancetelevisiontype.md)|<span data-ttu-id="f27ca-118">Оценка TV, выбранной для Франции.</span><span class="sxs-lookup"><span data-stu-id="f27ca-118">TV rating selected for France.</span></span> <span data-ttu-id="f27ca-119">Возможные значения: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="f27ca-119">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f27ca-120">Связи</span><span class="sxs-lookup"><span data-stu-id="f27ca-120">Relationships</span></span>
<span data-ttu-id="f27ca-121">Нет</span><span class="sxs-lookup"><span data-stu-id="f27ca-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f27ca-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f27ca-122">JSON Representation</span></span>
<span data-ttu-id="f27ca-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f27ca-123">Here is a JSON representation of the resource.</span></span>
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





