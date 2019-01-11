---
title: Тип ресурса mediaContentRatingJapan
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 8877e1b5f2c6031725c07a02b387da4ce5bc9136
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27856532"
---
# <a name="mediacontentratingjapan-resource-type"></a><span data-ttu-id="0f513-103">Тип ресурса mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="0f513-103">mediaContentRatingJapan resource type</span></span>

> <span data-ttu-id="0f513-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0f513-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0f513-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0f513-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0f513-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="0f513-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0f513-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="0f513-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="0f513-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="0f513-108">Properties</span></span>
|<span data-ttu-id="0f513-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="0f513-109">Property</span></span>|<span data-ttu-id="0f513-110">Тип</span><span class="sxs-lookup"><span data-stu-id="0f513-110">Type</span></span>|<span data-ttu-id="0f513-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0f513-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f513-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="0f513-112">movieRating</span></span>|[<span data-ttu-id="0f513-113">ratingJapanMoviesType</span><span class="sxs-lookup"><span data-stu-id="0f513-113">ratingJapanMoviesType</span></span>](../resources/intune-deviceconfig-ratingjapanmoviestype.md)|<span data-ttu-id="0f513-114">Оценка выбранных для Японии фильмы.</span><span class="sxs-lookup"><span data-stu-id="0f513-114">Movies rating selected for Japan.</span></span> <span data-ttu-id="0f513-115">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="0f513-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="0f513-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="0f513-116">tvRating</span></span>|[<span data-ttu-id="0f513-117">ratingJapanTelevisionType</span><span class="sxs-lookup"><span data-stu-id="0f513-117">ratingJapanTelevisionType</span></span>](../resources/intune-deviceconfig-ratingjapantelevisiontype.md)|<span data-ttu-id="0f513-118">Оценка TV, выбранной для Японии.</span><span class="sxs-lookup"><span data-stu-id="0f513-118">TV rating selected for Japan.</span></span> <span data-ttu-id="0f513-119">Возможные значения: `allAllowed`, `allBlocked`, `explicitAllowed`.</span><span class="sxs-lookup"><span data-stu-id="0f513-119">Possible values are: `allAllowed`, `allBlocked`, `explicitAllowed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0f513-120">Связи</span><span class="sxs-lookup"><span data-stu-id="0f513-120">Relationships</span></span>
<span data-ttu-id="0f513-121">Нет</span><span class="sxs-lookup"><span data-stu-id="0f513-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0f513-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0f513-122">JSON Representation</span></span>
<span data-ttu-id="0f513-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0f513-123">Here is a JSON representation of the resource.</span></span>
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





