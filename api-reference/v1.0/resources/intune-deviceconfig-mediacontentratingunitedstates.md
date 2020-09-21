---
title: Тип ресурса mediaContentRatingUnitedStates
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 30e41727b84e7f10b82917f4dc1dd23f296cc19f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48003061"
---
# <a name="mediacontentratingunitedstates-resource-type"></a><span data-ttu-id="9b13e-103">Тип ресурса mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="9b13e-103">mediaContentRatingUnitedStates resource type</span></span>

<span data-ttu-id="9b13e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9b13e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9b13e-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9b13e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9b13e-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="9b13e-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="9b13e-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="9b13e-107">Properties</span></span>
|<span data-ttu-id="9b13e-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="9b13e-108">Property</span></span>|<span data-ttu-id="9b13e-109">Тип</span><span class="sxs-lookup"><span data-stu-id="9b13e-109">Type</span></span>|<span data-ttu-id="9b13e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="9b13e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b13e-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="9b13e-111">movieRating</span></span>|[<span data-ttu-id="9b13e-112">ратингунитедстатесмовиестипе</span><span class="sxs-lookup"><span data-stu-id="9b13e-112">ratingUnitedStatesMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedstatesmoviestype.md)|<span data-ttu-id="9b13e-113">Оценка фильмов, выбранных для США.</span><span class="sxs-lookup"><span data-stu-id="9b13e-113">Movies rating selected for United States.</span></span> <span data-ttu-id="9b13e-114">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="9b13e-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span></span>|
|<span data-ttu-id="9b13e-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="9b13e-115">tvRating</span></span>|[<span data-ttu-id="9b13e-116">ратингунитедстатестелевисионтипе</span><span class="sxs-lookup"><span data-stu-id="9b13e-116">ratingUnitedStatesTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedstatestelevisiontype.md)|<span data-ttu-id="9b13e-117">Рейтинг для телевизора выбран для США.</span><span class="sxs-lookup"><span data-stu-id="9b13e-117">TV rating selected for United States.</span></span> <span data-ttu-id="9b13e-118">Возможные значения: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="9b13e-118">Possible values are: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9b13e-119">Связи</span><span class="sxs-lookup"><span data-stu-id="9b13e-119">Relationships</span></span>
<span data-ttu-id="9b13e-120">Нет</span><span class="sxs-lookup"><span data-stu-id="9b13e-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9b13e-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9b13e-121">JSON Representation</span></span>
<span data-ttu-id="9b13e-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9b13e-122">Here is a JSON representation of the resource.</span></span>
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









