---
title: Тип ресурса mediaContentRatingUnitedStates
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c5ed2470ff226a5c593dfed892bafb7b0fc3431d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532431"
---
# <a name="mediacontentratingunitedstates-resource-type"></a><span data-ttu-id="9d582-103">Тип ресурса mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="9d582-103">mediaContentRatingUnitedStates resource type</span></span>

<span data-ttu-id="9d582-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9d582-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9d582-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9d582-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9d582-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="9d582-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="9d582-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="9d582-107">Properties</span></span>
|<span data-ttu-id="9d582-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="9d582-108">Property</span></span>|<span data-ttu-id="9d582-109">Тип</span><span class="sxs-lookup"><span data-stu-id="9d582-109">Type</span></span>|<span data-ttu-id="9d582-110">Описание</span><span class="sxs-lookup"><span data-stu-id="9d582-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d582-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="9d582-111">movieRating</span></span>|[<span data-ttu-id="9d582-112">ратингунитедстатесмовиестипе</span><span class="sxs-lookup"><span data-stu-id="9d582-112">ratingUnitedStatesMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedstatesmoviestype.md)|<span data-ttu-id="9d582-113">Оценка фильмов, выбранных для США.</span><span class="sxs-lookup"><span data-stu-id="9d582-113">Movies rating selected for United States.</span></span> <span data-ttu-id="9d582-114">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="9d582-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span></span>|
|<span data-ttu-id="9d582-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="9d582-115">tvRating</span></span>|[<span data-ttu-id="9d582-116">ратингунитедстатестелевисионтипе</span><span class="sxs-lookup"><span data-stu-id="9d582-116">ratingUnitedStatesTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedstatestelevisiontype.md)|<span data-ttu-id="9d582-117">Рейтинг для телевизора выбран для США.</span><span class="sxs-lookup"><span data-stu-id="9d582-117">TV rating selected for United States.</span></span> <span data-ttu-id="9d582-118">Возможные значения: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="9d582-118">Possible values are: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9d582-119">Связи</span><span class="sxs-lookup"><span data-stu-id="9d582-119">Relationships</span></span>
<span data-ttu-id="9d582-120">Нет</span><span class="sxs-lookup"><span data-stu-id="9d582-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9d582-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9d582-121">JSON Representation</span></span>
<span data-ttu-id="9d582-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9d582-122">Here is a JSON representation of the resource.</span></span>
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




