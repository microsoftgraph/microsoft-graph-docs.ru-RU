---
title: Тип ресурса mediaContentRatingUnitedStates
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3e37a707b7ad190ddc1f3206f149d0dcc3c1aad3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27959226"
---
# <a name="mediacontentratingunitedstates-resource-type"></a><span data-ttu-id="ebb53-103">Тип ресурса mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="ebb53-103">mediaContentRatingUnitedStates resource type</span></span>

> <span data-ttu-id="ebb53-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ebb53-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ebb53-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="ebb53-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="ebb53-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="ebb53-106">Properties</span></span>
|<span data-ttu-id="ebb53-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="ebb53-107">Property</span></span>|<span data-ttu-id="ebb53-108">Тип</span><span class="sxs-lookup"><span data-stu-id="ebb53-108">Type</span></span>|<span data-ttu-id="ebb53-109">Описание</span><span class="sxs-lookup"><span data-stu-id="ebb53-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ebb53-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="ebb53-110">movieRating</span></span>|[<span data-ttu-id="ebb53-111">ratingUnitedStatesMoviesType</span><span class="sxs-lookup"><span data-stu-id="ebb53-111">ratingUnitedStatesMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedstatesmoviestype.md)|<span data-ttu-id="ebb53-112">Фильмы рейтинг выбранных для США.</span><span class="sxs-lookup"><span data-stu-id="ebb53-112">Movies rating selected for United States.</span></span> <span data-ttu-id="ebb53-113">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="ebb53-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span></span>|
|<span data-ttu-id="ebb53-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="ebb53-114">tvRating</span></span>|[<span data-ttu-id="ebb53-115">ratingUnitedStatesTelevisionType</span><span class="sxs-lookup"><span data-stu-id="ebb53-115">ratingUnitedStatesTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedstatestelevisiontype.md)|<span data-ttu-id="ebb53-116">Оценка TV, выбранной для США.</span><span class="sxs-lookup"><span data-stu-id="ebb53-116">TV rating selected for United States.</span></span> <span data-ttu-id="ebb53-117">Возможные значения: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="ebb53-117">Possible values are: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ebb53-118">Связи</span><span class="sxs-lookup"><span data-stu-id="ebb53-118">Relationships</span></span>
<span data-ttu-id="ebb53-119">Нет</span><span class="sxs-lookup"><span data-stu-id="ebb53-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ebb53-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ebb53-120">JSON Representation</span></span>
<span data-ttu-id="ebb53-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ebb53-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingUnitedStates"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingUnitedStates",
  "movieRating": "String",
  "tvRating": "String"
}
```



