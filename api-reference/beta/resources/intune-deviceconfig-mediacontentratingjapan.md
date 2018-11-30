---
title: Тип ресурса mediaContentRatingJapan
description: Н/Д
ms.openlocfilehash: 2fdf6ea6115f066df697a778e44e0476feac7d96
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076513"
---
# <a name="mediacontentratingjapan-resource-type"></a><span data-ttu-id="dc3f1-103">Тип ресурса mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="dc3f1-103">mediaContentRatingJapan resource type</span></span>

> <span data-ttu-id="dc3f1-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="dc3f1-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dc3f1-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc3f1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dc3f1-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="dc3f1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dc3f1-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="dc3f1-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="dc3f1-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="dc3f1-108">Properties</span></span>
|<span data-ttu-id="dc3f1-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="dc3f1-109">Property</span></span>|<span data-ttu-id="dc3f1-110">Тип</span><span class="sxs-lookup"><span data-stu-id="dc3f1-110">Type</span></span>|<span data-ttu-id="dc3f1-111">Описание</span><span class="sxs-lookup"><span data-stu-id="dc3f1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc3f1-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="dc3f1-112">movieRating</span></span>|[<span data-ttu-id="dc3f1-113">ratingJapanMoviesType</span><span class="sxs-lookup"><span data-stu-id="dc3f1-113">ratingJapanMoviesType</span></span>](../resources/intune-deviceconfig-ratingjapanmoviestype.md)|<span data-ttu-id="dc3f1-114">Оценка выбранных для Японии фильмы.</span><span class="sxs-lookup"><span data-stu-id="dc3f1-114">Movies rating selected for Japan.</span></span> <span data-ttu-id="dc3f1-115">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="dc3f1-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="dc3f1-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="dc3f1-116">tvRating</span></span>|[<span data-ttu-id="dc3f1-117">ratingJapanTelevisionType</span><span class="sxs-lookup"><span data-stu-id="dc3f1-117">ratingJapanTelevisionType</span></span>](../resources/intune-deviceconfig-ratingjapantelevisiontype.md)|<span data-ttu-id="dc3f1-118">Оценка TV, выбранной для Японии.</span><span class="sxs-lookup"><span data-stu-id="dc3f1-118">TV rating selected for Japan.</span></span> <span data-ttu-id="dc3f1-119">Возможные значения: `allAllowed`, `allBlocked`, `explicitAllowed`.</span><span class="sxs-lookup"><span data-stu-id="dc3f1-119">Possible values are: `allAllowed`, `allBlocked`, `explicitAllowed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dc3f1-120">Связи</span><span class="sxs-lookup"><span data-stu-id="dc3f1-120">Relationships</span></span>
<span data-ttu-id="dc3f1-121">Нет</span><span class="sxs-lookup"><span data-stu-id="dc3f1-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="dc3f1-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dc3f1-122">JSON Representation</span></span>
<span data-ttu-id="dc3f1-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dc3f1-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingJapan"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingJapan",
  "movieRating": "String",
  "tvRating": "String"
}
```





