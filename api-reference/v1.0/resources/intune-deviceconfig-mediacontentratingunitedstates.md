---
title: Тип ресурса mediaContentRatingUnitedStates
description: Пока не задокументировано.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: baa5d98f0fcb1d267221c95c0b27be988d3a197f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32572320"
---
# <a name="mediacontentratingunitedstates-resource-type"></a><span data-ttu-id="07967-103">Тип ресурса mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="07967-103">mediaContentRatingUnitedStates resource type</span></span>

> <span data-ttu-id="07967-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="07967-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07967-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="07967-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="07967-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="07967-106">Properties</span></span>
|<span data-ttu-id="07967-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="07967-107">Property</span></span>|<span data-ttu-id="07967-108">Тип</span><span class="sxs-lookup"><span data-stu-id="07967-108">Type</span></span>|<span data-ttu-id="07967-109">Описание</span><span class="sxs-lookup"><span data-stu-id="07967-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07967-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="07967-110">movieRating</span></span>|[<span data-ttu-id="07967-111">Ратингунитедстатесмовиестипе</span><span class="sxs-lookup"><span data-stu-id="07967-111">ratingUnitedStatesMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedstatesmoviestype.md)|<span data-ttu-id="07967-112">Оценка фильмов, выбранных для США.</span><span class="sxs-lookup"><span data-stu-id="07967-112">Movies rating selected for United States.</span></span> <span data-ttu-id="07967-113">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="07967-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span></span>|
|<span data-ttu-id="07967-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="07967-114">tvRating</span></span>|[<span data-ttu-id="07967-115">Ратингунитедстатестелевисионтипе</span><span class="sxs-lookup"><span data-stu-id="07967-115">ratingUnitedStatesTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedstatestelevisiontype.md)|<span data-ttu-id="07967-116">Рейтинг для телевизора выбран для США.</span><span class="sxs-lookup"><span data-stu-id="07967-116">TV rating selected for United States.</span></span> <span data-ttu-id="07967-117">Возможные значения: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="07967-117">Possible values are: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="07967-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="07967-118">Relationships</span></span>
<span data-ttu-id="07967-119">Нет</span><span class="sxs-lookup"><span data-stu-id="07967-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="07967-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="07967-120">JSON Representation</span></span>
<span data-ttu-id="07967-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="07967-121">Here is a JSON representation of the resource.</span></span>
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



