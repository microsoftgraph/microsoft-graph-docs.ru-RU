---
title: Тип ресурса mediaContentRatingUnitedStates
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4d9887ee7d2375a9b954a7f62f84701b997d9b7a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43473094"
---
# <a name="mediacontentratingunitedstates-resource-type"></a><span data-ttu-id="6a3e7-103">Тип ресурса mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="6a3e7-103">mediaContentRatingUnitedStates resource type</span></span>

<span data-ttu-id="6a3e7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6a3e7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6a3e7-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6a3e7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a3e7-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="6a3e7-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="6a3e7-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="6a3e7-107">Properties</span></span>
|<span data-ttu-id="6a3e7-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="6a3e7-108">Property</span></span>|<span data-ttu-id="6a3e7-109">Тип</span><span class="sxs-lookup"><span data-stu-id="6a3e7-109">Type</span></span>|<span data-ttu-id="6a3e7-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6a3e7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a3e7-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="6a3e7-111">movieRating</span></span>|[<span data-ttu-id="6a3e7-112">ратингунитедстатесмовиестипе</span><span class="sxs-lookup"><span data-stu-id="6a3e7-112">ratingUnitedStatesMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedstatesmoviestype.md)|<span data-ttu-id="6a3e7-113">Оценка фильмов, выбранных для США.</span><span class="sxs-lookup"><span data-stu-id="6a3e7-113">Movies rating selected for United States.</span></span> <span data-ttu-id="6a3e7-114">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="6a3e7-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span></span>|
|<span data-ttu-id="6a3e7-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="6a3e7-115">tvRating</span></span>|[<span data-ttu-id="6a3e7-116">ратингунитедстатестелевисионтипе</span><span class="sxs-lookup"><span data-stu-id="6a3e7-116">ratingUnitedStatesTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedstatestelevisiontype.md)|<span data-ttu-id="6a3e7-117">Рейтинг для телевизора выбран для США.</span><span class="sxs-lookup"><span data-stu-id="6a3e7-117">TV rating selected for United States.</span></span> <span data-ttu-id="6a3e7-118">Возможные значения: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="6a3e7-118">Possible values are: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6a3e7-119">Связи</span><span class="sxs-lookup"><span data-stu-id="6a3e7-119">Relationships</span></span>
<span data-ttu-id="6a3e7-120">Нет</span><span class="sxs-lookup"><span data-stu-id="6a3e7-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6a3e7-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6a3e7-121">JSON Representation</span></span>
<span data-ttu-id="6a3e7-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6a3e7-122">Here is a JSON representation of the resource.</span></span>
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







