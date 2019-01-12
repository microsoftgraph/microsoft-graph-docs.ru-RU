---
title: Тип ресурса mediaContentRatingAustralia
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5147cc307c39187b2daab4cd4031bf449f7cc4e5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962991"
---
# <a name="mediacontentratingaustralia-resource-type"></a><span data-ttu-id="4004e-103">Тип ресурса mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="4004e-103">mediaContentRatingAustralia resource type</span></span>

> <span data-ttu-id="4004e-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4004e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4004e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4004e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4004e-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4004e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4004e-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="4004e-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="4004e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="4004e-108">Properties</span></span>
|<span data-ttu-id="4004e-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="4004e-109">Property</span></span>|<span data-ttu-id="4004e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="4004e-110">Type</span></span>|<span data-ttu-id="4004e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="4004e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4004e-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="4004e-112">movieRating</span></span>|[<span data-ttu-id="4004e-113">ratingAustraliaMoviesType</span><span class="sxs-lookup"><span data-stu-id="4004e-113">ratingAustraliaMoviesType</span></span>](../resources/intune-deviceconfig-ratingaustraliamoviestype.md)|<span data-ttu-id="4004e-114">Оценка выбранных для Австралии фильмы.</span><span class="sxs-lookup"><span data-stu-id="4004e-114">Movies rating selected for Australia.</span></span> <span data-ttu-id="4004e-115">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="4004e-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="4004e-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="4004e-116">tvRating</span></span>|[<span data-ttu-id="4004e-117">ratingAustraliaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="4004e-117">ratingAustraliaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingaustraliatelevisiontype.md)|<span data-ttu-id="4004e-118">Оценка TV, выбранной для Австралии.</span><span class="sxs-lookup"><span data-stu-id="4004e-118">TV rating selected for Australia.</span></span> <span data-ttu-id="4004e-119">Возможные значения: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span><span class="sxs-lookup"><span data-stu-id="4004e-119">Possible values are: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4004e-120">Связи</span><span class="sxs-lookup"><span data-stu-id="4004e-120">Relationships</span></span>
<span data-ttu-id="4004e-121">Нет</span><span class="sxs-lookup"><span data-stu-id="4004e-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4004e-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4004e-122">JSON Representation</span></span>
<span data-ttu-id="4004e-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4004e-123">Here is a JSON representation of the resource.</span></span>
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





