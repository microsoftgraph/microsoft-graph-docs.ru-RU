---
title: Тип ресурса mediaContentRatingJapan
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 202b778fefe1236577f61058025714ea0f337826
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27943020"
---
# <a name="mediacontentratingjapan-resource-type"></a><span data-ttu-id="bf069-103">Тип ресурса mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="bf069-103">mediaContentRatingJapan resource type</span></span>

> <span data-ttu-id="bf069-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="bf069-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bf069-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bf069-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bf069-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="bf069-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bf069-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="bf069-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="bf069-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="bf069-108">Properties</span></span>
|<span data-ttu-id="bf069-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="bf069-109">Property</span></span>|<span data-ttu-id="bf069-110">Тип</span><span class="sxs-lookup"><span data-stu-id="bf069-110">Type</span></span>|<span data-ttu-id="bf069-111">Описание</span><span class="sxs-lookup"><span data-stu-id="bf069-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf069-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="bf069-112">movieRating</span></span>|[<span data-ttu-id="bf069-113">ratingJapanMoviesType</span><span class="sxs-lookup"><span data-stu-id="bf069-113">ratingJapanMoviesType</span></span>](../resources/intune-deviceconfig-ratingjapanmoviestype.md)|<span data-ttu-id="bf069-114">Оценка выбранных для Японии фильмы.</span><span class="sxs-lookup"><span data-stu-id="bf069-114">Movies rating selected for Japan.</span></span> <span data-ttu-id="bf069-115">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="bf069-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="bf069-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="bf069-116">tvRating</span></span>|[<span data-ttu-id="bf069-117">ratingJapanTelevisionType</span><span class="sxs-lookup"><span data-stu-id="bf069-117">ratingJapanTelevisionType</span></span>](../resources/intune-deviceconfig-ratingjapantelevisiontype.md)|<span data-ttu-id="bf069-118">Оценка TV, выбранной для Японии.</span><span class="sxs-lookup"><span data-stu-id="bf069-118">TV rating selected for Japan.</span></span> <span data-ttu-id="bf069-119">Возможные значения: `allAllowed`, `allBlocked`, `explicitAllowed`.</span><span class="sxs-lookup"><span data-stu-id="bf069-119">Possible values are: `allAllowed`, `allBlocked`, `explicitAllowed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bf069-120">Связи</span><span class="sxs-lookup"><span data-stu-id="bf069-120">Relationships</span></span>
<span data-ttu-id="bf069-121">Нет</span><span class="sxs-lookup"><span data-stu-id="bf069-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="bf069-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bf069-122">JSON Representation</span></span>
<span data-ttu-id="bf069-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bf069-123">Here is a JSON representation of the resource.</span></span>
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





