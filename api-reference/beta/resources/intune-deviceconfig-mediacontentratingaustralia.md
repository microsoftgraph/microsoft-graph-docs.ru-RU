---
title: Тип ресурса mediaContentRatingAustralia
description: Н/Д
ms.openlocfilehash: ff8cb3e6bc389e7a99b84e9aa248871b5830a7e9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080415"
---
# <a name="mediacontentratingaustralia-resource-type"></a><span data-ttu-id="aed08-103">Тип ресурса mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="aed08-103">mediaContentRatingAustralia resource type</span></span>

> <span data-ttu-id="aed08-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="aed08-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aed08-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aed08-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="aed08-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="aed08-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="aed08-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="aed08-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="aed08-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="aed08-108">Properties</span></span>
|<span data-ttu-id="aed08-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="aed08-109">Property</span></span>|<span data-ttu-id="aed08-110">Тип</span><span class="sxs-lookup"><span data-stu-id="aed08-110">Type</span></span>|<span data-ttu-id="aed08-111">Описание</span><span class="sxs-lookup"><span data-stu-id="aed08-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aed08-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="aed08-112">movieRating</span></span>|[<span data-ttu-id="aed08-113">ratingAustraliaMoviesType</span><span class="sxs-lookup"><span data-stu-id="aed08-113">ratingAustraliaMoviesType</span></span>](../resources/intune-deviceconfig-ratingaustraliamoviestype.md)|<span data-ttu-id="aed08-114">Оценка выбранных для Австралии фильмы.</span><span class="sxs-lookup"><span data-stu-id="aed08-114">Movies rating selected for Australia.</span></span> <span data-ttu-id="aed08-115">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="aed08-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="aed08-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="aed08-116">tvRating</span></span>|[<span data-ttu-id="aed08-117">ratingAustraliaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="aed08-117">ratingAustraliaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingaustraliatelevisiontype.md)|<span data-ttu-id="aed08-118">Оценка TV, выбранной для Австралии.</span><span class="sxs-lookup"><span data-stu-id="aed08-118">TV rating selected for Australia.</span></span> <span data-ttu-id="aed08-119">Возможные значения: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span><span class="sxs-lookup"><span data-stu-id="aed08-119">Possible values are: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aed08-120">Связи</span><span class="sxs-lookup"><span data-stu-id="aed08-120">Relationships</span></span>
<span data-ttu-id="aed08-121">Нет</span><span class="sxs-lookup"><span data-stu-id="aed08-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="aed08-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="aed08-122">JSON Representation</span></span>
<span data-ttu-id="aed08-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aed08-123">Here is a JSON representation of the resource.</span></span>
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





