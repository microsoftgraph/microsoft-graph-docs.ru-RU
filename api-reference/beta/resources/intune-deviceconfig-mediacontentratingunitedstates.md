---
title: Тип ресурса mediaContentRatingUnitedStates
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 130b74fa3cf0a5424f7ad816107b80101b9cee49
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30161903"
---
# <a name="mediacontentratingunitedstates-resource-type"></a><span data-ttu-id="23efb-103">Тип ресурса mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="23efb-103">mediaContentRatingUnitedStates resource type</span></span>

> <span data-ttu-id="23efb-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="23efb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="23efb-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="23efb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="23efb-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="23efb-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="23efb-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="23efb-107">Properties</span></span>
|<span data-ttu-id="23efb-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="23efb-108">Property</span></span>|<span data-ttu-id="23efb-109">Тип</span><span class="sxs-lookup"><span data-stu-id="23efb-109">Type</span></span>|<span data-ttu-id="23efb-110">Описание</span><span class="sxs-lookup"><span data-stu-id="23efb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23efb-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="23efb-111">movieRating</span></span>|[<span data-ttu-id="23efb-112">Ратингунитедстатесмовиестипе</span><span class="sxs-lookup"><span data-stu-id="23efb-112">ratingUnitedStatesMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedstatesmoviestype.md)|<span data-ttu-id="23efb-113">Оценка фильмов, выбранных для США.</span><span class="sxs-lookup"><span data-stu-id="23efb-113">Movies rating selected for United States.</span></span> <span data-ttu-id="23efb-114">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="23efb-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span></span>|
|<span data-ttu-id="23efb-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="23efb-115">tvRating</span></span>|[<span data-ttu-id="23efb-116">Ратингунитедстатестелевисионтипе</span><span class="sxs-lookup"><span data-stu-id="23efb-116">ratingUnitedStatesTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedstatestelevisiontype.md)|<span data-ttu-id="23efb-117">Рейтинг для телевизора выбран для США.</span><span class="sxs-lookup"><span data-stu-id="23efb-117">TV rating selected for United States.</span></span> <span data-ttu-id="23efb-118">Возможные значения: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="23efb-118">Possible values are: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="23efb-119">Связи</span><span class="sxs-lookup"><span data-stu-id="23efb-119">Relationships</span></span>
<span data-ttu-id="23efb-120">Нет</span><span class="sxs-lookup"><span data-stu-id="23efb-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="23efb-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="23efb-121">JSON Representation</span></span>
<span data-ttu-id="23efb-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="23efb-122">Here is a JSON representation of the resource.</span></span>
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




