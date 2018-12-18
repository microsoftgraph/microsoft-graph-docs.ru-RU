---
title: Тип ресурса mediaContentRatingUnitedStates
description: Н/Д
author: tfitzmac
ms.openlocfilehash: b69e09684097ffbd85cf8117e4dd17779cbc5c67
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27319455"
---
# <a name="mediacontentratingunitedstates-resource-type"></a><span data-ttu-id="af0ec-103">Тип ресурса mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="af0ec-103">mediaContentRatingUnitedStates resource type</span></span>

> <span data-ttu-id="af0ec-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="af0ec-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="af0ec-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="af0ec-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="af0ec-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="af0ec-106">Properties</span></span>
|<span data-ttu-id="af0ec-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="af0ec-107">Property</span></span>|<span data-ttu-id="af0ec-108">Тип</span><span class="sxs-lookup"><span data-stu-id="af0ec-108">Type</span></span>|<span data-ttu-id="af0ec-109">Описание</span><span class="sxs-lookup"><span data-stu-id="af0ec-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af0ec-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="af0ec-110">movieRating</span></span>|[<span data-ttu-id="af0ec-111">ratingUnitedStatesMoviesType</span><span class="sxs-lookup"><span data-stu-id="af0ec-111">ratingUnitedStatesMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedstatesmoviestype.md)|<span data-ttu-id="af0ec-112">Фильмы рейтинг выбранных для США.</span><span class="sxs-lookup"><span data-stu-id="af0ec-112">Movies rating selected for United States.</span></span> <span data-ttu-id="af0ec-113">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="af0ec-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span></span>|
|<span data-ttu-id="af0ec-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="af0ec-114">tvRating</span></span>|[<span data-ttu-id="af0ec-115">ratingUnitedStatesTelevisionType</span><span class="sxs-lookup"><span data-stu-id="af0ec-115">ratingUnitedStatesTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedstatestelevisiontype.md)|<span data-ttu-id="af0ec-116">Оценка TV, выбранной для США.</span><span class="sxs-lookup"><span data-stu-id="af0ec-116">TV rating selected for United States.</span></span> <span data-ttu-id="af0ec-117">Возможные значения: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="af0ec-117">Possible values are: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="af0ec-118">Связи</span><span class="sxs-lookup"><span data-stu-id="af0ec-118">Relationships</span></span>
<span data-ttu-id="af0ec-119">Нет</span><span class="sxs-lookup"><span data-stu-id="af0ec-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="af0ec-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="af0ec-120">JSON Representation</span></span>
<span data-ttu-id="af0ec-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="af0ec-121">Here is a JSON representation of the resource.</span></span>
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



