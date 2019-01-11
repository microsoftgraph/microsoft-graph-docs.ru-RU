---
title: Тип ресурса mediaContentRatingAustralia
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 916257d83e28f3877773a6fcc7d7aefadab41af8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884226"
---
# <a name="mediacontentratingaustralia-resource-type"></a><span data-ttu-id="9213a-103">Тип ресурса mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="9213a-103">mediaContentRatingAustralia resource type</span></span>

> <span data-ttu-id="9213a-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9213a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9213a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9213a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9213a-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="9213a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9213a-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="9213a-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="9213a-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="9213a-108">Properties</span></span>
|<span data-ttu-id="9213a-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="9213a-109">Property</span></span>|<span data-ttu-id="9213a-110">Тип</span><span class="sxs-lookup"><span data-stu-id="9213a-110">Type</span></span>|<span data-ttu-id="9213a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="9213a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9213a-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="9213a-112">movieRating</span></span>|[<span data-ttu-id="9213a-113">ratingAustraliaMoviesType</span><span class="sxs-lookup"><span data-stu-id="9213a-113">ratingAustraliaMoviesType</span></span>](../resources/intune-deviceconfig-ratingaustraliamoviestype.md)|<span data-ttu-id="9213a-114">Оценка выбранных для Австралии фильмы.</span><span class="sxs-lookup"><span data-stu-id="9213a-114">Movies rating selected for Australia.</span></span> <span data-ttu-id="9213a-115">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="9213a-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="9213a-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="9213a-116">tvRating</span></span>|[<span data-ttu-id="9213a-117">ratingAustraliaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="9213a-117">ratingAustraliaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingaustraliatelevisiontype.md)|<span data-ttu-id="9213a-118">Оценка TV, выбранной для Австралии.</span><span class="sxs-lookup"><span data-stu-id="9213a-118">TV rating selected for Australia.</span></span> <span data-ttu-id="9213a-119">Возможные значения: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span><span class="sxs-lookup"><span data-stu-id="9213a-119">Possible values are: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9213a-120">Связи</span><span class="sxs-lookup"><span data-stu-id="9213a-120">Relationships</span></span>
<span data-ttu-id="9213a-121">Нет</span><span class="sxs-lookup"><span data-stu-id="9213a-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9213a-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9213a-122">JSON Representation</span></span>
<span data-ttu-id="9213a-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9213a-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingAustralia"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingAustralia",
  "movieRating": "String",
  "tvRating": "String"
}
```





