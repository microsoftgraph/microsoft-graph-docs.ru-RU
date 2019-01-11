---
title: Тип ресурса mediaContentRatingNewZealand
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 31d3dcf84b6343bcb03430fa27f901ca02580044
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837964"
---
# <a name="mediacontentratingnewzealand-resource-type"></a><span data-ttu-id="fa4d7-103">Тип ресурса mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="fa4d7-103">mediaContentRatingNewZealand resource type</span></span>

> <span data-ttu-id="fa4d7-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fa4d7-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fa4d7-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa4d7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fa4d7-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="fa4d7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fa4d7-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="fa4d7-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="fa4d7-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="fa4d7-108">Properties</span></span>
|<span data-ttu-id="fa4d7-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="fa4d7-109">Property</span></span>|<span data-ttu-id="fa4d7-110">Тип</span><span class="sxs-lookup"><span data-stu-id="fa4d7-110">Type</span></span>|<span data-ttu-id="fa4d7-111">Описание</span><span class="sxs-lookup"><span data-stu-id="fa4d7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa4d7-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="fa4d7-112">movieRating</span></span>|[<span data-ttu-id="fa4d7-113">ratingNewZealandMoviesType</span><span class="sxs-lookup"><span data-stu-id="fa4d7-113">ratingNewZealandMoviesType</span></span>](../resources/intune-deviceconfig-ratingnewzealandmoviestype.md)|<span data-ttu-id="fa4d7-114">Оценка выбранных для новой Зеландии фильмы.</span><span class="sxs-lookup"><span data-stu-id="fa4d7-114">Movies rating selected for New Zealand.</span></span> <span data-ttu-id="fa4d7-115">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span><span class="sxs-lookup"><span data-stu-id="fa4d7-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span></span>|
|<span data-ttu-id="fa4d7-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="fa4d7-116">tvRating</span></span>|[<span data-ttu-id="fa4d7-117">ratingNewZealandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="fa4d7-117">ratingNewZealandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingnewzealandtelevisiontype.md)|<span data-ttu-id="fa4d7-118">Оценка TV, выбранной для новой Зеландии.</span><span class="sxs-lookup"><span data-stu-id="fa4d7-118">TV rating selected for New Zealand.</span></span> <span data-ttu-id="fa4d7-119">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="fa4d7-119">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fa4d7-120">Связи</span><span class="sxs-lookup"><span data-stu-id="fa4d7-120">Relationships</span></span>
<span data-ttu-id="fa4d7-121">Нет</span><span class="sxs-lookup"><span data-stu-id="fa4d7-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="fa4d7-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fa4d7-122">JSON Representation</span></span>
<span data-ttu-id="fa4d7-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fa4d7-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingNewZealand"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingNewZealand",
  "movieRating": "String",
  "tvRating": "String"
}
```





