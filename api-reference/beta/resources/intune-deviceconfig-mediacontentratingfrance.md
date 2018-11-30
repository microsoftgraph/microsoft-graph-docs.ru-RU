---
title: Тип ресурса mediaContentRatingFrance
description: Н/Д
ms.openlocfilehash: dabadb4d03181d3cd66db582005c4ec58f28aa9d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076733"
---
# <a name="mediacontentratingfrance-resource-type"></a><span data-ttu-id="ab0bb-103">Тип ресурса mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="ab0bb-103">mediaContentRatingFrance resource type</span></span>

> <span data-ttu-id="ab0bb-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ab0bb-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ab0bb-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab0bb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ab0bb-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ab0bb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ab0bb-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="ab0bb-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="ab0bb-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="ab0bb-108">Properties</span></span>
|<span data-ttu-id="ab0bb-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="ab0bb-109">Property</span></span>|<span data-ttu-id="ab0bb-110">Тип</span><span class="sxs-lookup"><span data-stu-id="ab0bb-110">Type</span></span>|<span data-ttu-id="ab0bb-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ab0bb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab0bb-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="ab0bb-112">movieRating</span></span>|[<span data-ttu-id="ab0bb-113">ratingFranceMoviesType</span><span class="sxs-lookup"><span data-stu-id="ab0bb-113">ratingFranceMoviesType</span></span>](../resources/intune-deviceconfig-ratingfrancemoviestype.md)|<span data-ttu-id="ab0bb-114">Оценка выбранных для Франции фильмы.</span><span class="sxs-lookup"><span data-stu-id="ab0bb-114">Movies rating selected for France.</span></span> <span data-ttu-id="ab0bb-115">Возможные значения: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="ab0bb-115">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|
|<span data-ttu-id="ab0bb-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="ab0bb-116">tvRating</span></span>|[<span data-ttu-id="ab0bb-117">ratingFranceTelevisionType</span><span class="sxs-lookup"><span data-stu-id="ab0bb-117">ratingFranceTelevisionType</span></span>](../resources/intune-deviceconfig-ratingfrancetelevisiontype.md)|<span data-ttu-id="ab0bb-118">Оценка TV, выбранной для Франции.</span><span class="sxs-lookup"><span data-stu-id="ab0bb-118">TV rating selected for France.</span></span> <span data-ttu-id="ab0bb-119">Возможные значения: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="ab0bb-119">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ab0bb-120">Связи</span><span class="sxs-lookup"><span data-stu-id="ab0bb-120">Relationships</span></span>
<span data-ttu-id="ab0bb-121">Нет</span><span class="sxs-lookup"><span data-stu-id="ab0bb-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ab0bb-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ab0bb-122">JSON Representation</span></span>
<span data-ttu-id="ab0bb-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ab0bb-123">Here is a JSON representation of the resource.</span></span>
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





