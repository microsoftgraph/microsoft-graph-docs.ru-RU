---
title: Тип ресурса mediaContentRatingUnitedStates
description: Пока не задокументировано.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c6c6df674fc4cef174892d4cdb27303c3933fcdd
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031376"
---
# <a name="mediacontentratingunitedstates-resource-type"></a><span data-ttu-id="99aae-103">Тип ресурса mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="99aae-103">mediaContentRatingUnitedStates resource type</span></span>

> <span data-ttu-id="99aae-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="99aae-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="99aae-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="99aae-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="99aae-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="99aae-106">Properties</span></span>
|<span data-ttu-id="99aae-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="99aae-107">Property</span></span>|<span data-ttu-id="99aae-108">Тип</span><span class="sxs-lookup"><span data-stu-id="99aae-108">Type</span></span>|<span data-ttu-id="99aae-109">Описание</span><span class="sxs-lookup"><span data-stu-id="99aae-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99aae-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="99aae-110">movieRating</span></span>|[<span data-ttu-id="99aae-111">Ратингунитедстатесмовиестипе</span><span class="sxs-lookup"><span data-stu-id="99aae-111">ratingUnitedStatesMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedstatesmoviestype.md)|<span data-ttu-id="99aae-112">Оценка фильмов, выбранных для США.</span><span class="sxs-lookup"><span data-stu-id="99aae-112">Movies rating selected for United States.</span></span> <span data-ttu-id="99aae-113">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="99aae-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span></span>|
|<span data-ttu-id="99aae-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="99aae-114">tvRating</span></span>|[<span data-ttu-id="99aae-115">Ратингунитедстатестелевисионтипе</span><span class="sxs-lookup"><span data-stu-id="99aae-115">ratingUnitedStatesTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedstatestelevisiontype.md)|<span data-ttu-id="99aae-116">Рейтинг для телевизора выбран для США.</span><span class="sxs-lookup"><span data-stu-id="99aae-116">TV rating selected for United States.</span></span> <span data-ttu-id="99aae-117">Возможные значения: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="99aae-117">Possible values are: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="99aae-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="99aae-118">Relationships</span></span>
<span data-ttu-id="99aae-119">Нет</span><span class="sxs-lookup"><span data-stu-id="99aae-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="99aae-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="99aae-120">JSON Representation</span></span>
<span data-ttu-id="99aae-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="99aae-121">Here is a JSON representation of the resource.</span></span>
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



