---
title: Тип ресурса mediaContentRatingAustralia
description: Н/Д
author: tfitzmac
ms.openlocfilehash: 29501d5e52b922baabd777a8838896230a502631
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27317166"
---
# <a name="mediacontentratingaustralia-resource-type"></a><span data-ttu-id="b8ab6-103">Тип ресурса mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="b8ab6-103">mediaContentRatingAustralia resource type</span></span>

> <span data-ttu-id="b8ab6-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b8ab6-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b8ab6-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b8ab6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b8ab6-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b8ab6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b8ab6-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="b8ab6-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="b8ab6-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="b8ab6-108">Properties</span></span>
|<span data-ttu-id="b8ab6-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="b8ab6-109">Property</span></span>|<span data-ttu-id="b8ab6-110">Тип</span><span class="sxs-lookup"><span data-stu-id="b8ab6-110">Type</span></span>|<span data-ttu-id="b8ab6-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b8ab6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8ab6-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="b8ab6-112">movieRating</span></span>|[<span data-ttu-id="b8ab6-113">ratingAustraliaMoviesType</span><span class="sxs-lookup"><span data-stu-id="b8ab6-113">ratingAustraliaMoviesType</span></span>](../resources/intune-deviceconfig-ratingaustraliamoviestype.md)|<span data-ttu-id="b8ab6-114">Оценка выбранных для Австралии фильмы.</span><span class="sxs-lookup"><span data-stu-id="b8ab6-114">Movies rating selected for Australia.</span></span> <span data-ttu-id="b8ab6-115">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="b8ab6-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="b8ab6-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="b8ab6-116">tvRating</span></span>|[<span data-ttu-id="b8ab6-117">ratingAustraliaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="b8ab6-117">ratingAustraliaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingaustraliatelevisiontype.md)|<span data-ttu-id="b8ab6-118">Оценка TV, выбранной для Австралии.</span><span class="sxs-lookup"><span data-stu-id="b8ab6-118">TV rating selected for Australia.</span></span> <span data-ttu-id="b8ab6-119">Возможные значения: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span><span class="sxs-lookup"><span data-stu-id="b8ab6-119">Possible values are: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b8ab6-120">Связи</span><span class="sxs-lookup"><span data-stu-id="b8ab6-120">Relationships</span></span>
<span data-ttu-id="b8ab6-121">Нет</span><span class="sxs-lookup"><span data-stu-id="b8ab6-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b8ab6-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b8ab6-122">JSON Representation</span></span>
<span data-ttu-id="b8ab6-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b8ab6-123">Here is a JSON representation of the resource.</span></span>
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





