---
title: Тип ресурса mediaContentRatingUnitedKingdom
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e4ab6731bc486918815efe0d3f4c7f6f2638329d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27953303"
---
# <a name="mediacontentratingunitedkingdom-resource-type"></a><span data-ttu-id="bbd41-103">Тип ресурса mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="bbd41-103">mediaContentRatingUnitedKingdom resource type</span></span>

> <span data-ttu-id="bbd41-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="bbd41-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bbd41-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bbd41-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bbd41-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="bbd41-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bbd41-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="bbd41-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="bbd41-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="bbd41-108">Properties</span></span>
|<span data-ttu-id="bbd41-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="bbd41-109">Property</span></span>|<span data-ttu-id="bbd41-110">Тип</span><span class="sxs-lookup"><span data-stu-id="bbd41-110">Type</span></span>|<span data-ttu-id="bbd41-111">Описание</span><span class="sxs-lookup"><span data-stu-id="bbd41-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bbd41-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="bbd41-112">movieRating</span></span>|[<span data-ttu-id="bbd41-113">ratingUnitedKingdomMoviesType</span><span class="sxs-lookup"><span data-stu-id="bbd41-113">ratingUnitedKingdomMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdommoviestype.md)|<span data-ttu-id="bbd41-114">Оценка выбранных для Великобритании фильмы.</span><span class="sxs-lookup"><span data-stu-id="bbd41-114">Movies rating selected for United Kingdom.</span></span> <span data-ttu-id="bbd41-115">Возможные значения: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="bbd41-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span></span>|
|<span data-ttu-id="bbd41-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="bbd41-116">tvRating</span></span>|[<span data-ttu-id="bbd41-117">ratingUnitedKingdomTelevisionType</span><span class="sxs-lookup"><span data-stu-id="bbd41-117">ratingUnitedKingdomTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdomtelevisiontype.md)|<span data-ttu-id="bbd41-118">Оценка TV, выбранные для Великобритании.</span><span class="sxs-lookup"><span data-stu-id="bbd41-118">TV rating selected for United Kingdom.</span></span> <span data-ttu-id="bbd41-119">Возможные значения: `allAllowed`, `allBlocked`, `caution`.</span><span class="sxs-lookup"><span data-stu-id="bbd41-119">Possible values are: `allAllowed`, `allBlocked`, `caution`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bbd41-120">Связи</span><span class="sxs-lookup"><span data-stu-id="bbd41-120">Relationships</span></span>
<span data-ttu-id="bbd41-121">Нет</span><span class="sxs-lookup"><span data-stu-id="bbd41-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="bbd41-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bbd41-122">JSON Representation</span></span>
<span data-ttu-id="bbd41-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bbd41-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingUnitedKingdom"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingUnitedKingdom",
  "movieRating": "String",
  "tvRating": "String"
}
```





