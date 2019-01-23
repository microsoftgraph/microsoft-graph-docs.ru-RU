---
title: Тип ресурса mediaContentRatingUnitedStates
description: Н/Д
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 60f673e31014eb4da027a58ea29099d9d8aa18e3
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425836"
---
# <a name="mediacontentratingunitedstates-resource-type"></a><span data-ttu-id="3e35e-103">Тип ресурса mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="3e35e-103">mediaContentRatingUnitedStates resource type</span></span>

> <span data-ttu-id="3e35e-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3e35e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3e35e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e35e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3e35e-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3e35e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3e35e-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="3e35e-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="3e35e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="3e35e-108">Properties</span></span>
|<span data-ttu-id="3e35e-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="3e35e-109">Property</span></span>|<span data-ttu-id="3e35e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="3e35e-110">Type</span></span>|<span data-ttu-id="3e35e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="3e35e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e35e-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="3e35e-112">movieRating</span></span>|[<span data-ttu-id="3e35e-113">ratingUnitedStatesMoviesType</span><span class="sxs-lookup"><span data-stu-id="3e35e-113">ratingUnitedStatesMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedstatesmoviestype.md)|<span data-ttu-id="3e35e-114">Фильмы рейтинг выбранных для США.</span><span class="sxs-lookup"><span data-stu-id="3e35e-114">Movies rating selected for United States.</span></span> <span data-ttu-id="3e35e-115">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="3e35e-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span></span>|
|<span data-ttu-id="3e35e-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="3e35e-116">tvRating</span></span>|[<span data-ttu-id="3e35e-117">ratingUnitedStatesTelevisionType</span><span class="sxs-lookup"><span data-stu-id="3e35e-117">ratingUnitedStatesTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedstatestelevisiontype.md)|<span data-ttu-id="3e35e-118">Оценка TV, выбранной для США.</span><span class="sxs-lookup"><span data-stu-id="3e35e-118">TV rating selected for United States.</span></span> <span data-ttu-id="3e35e-119">Возможные значения: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="3e35e-119">Possible values are: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3e35e-120">Связи</span><span class="sxs-lookup"><span data-stu-id="3e35e-120">Relationships</span></span>
<span data-ttu-id="3e35e-121">Нет</span><span class="sxs-lookup"><span data-stu-id="3e35e-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3e35e-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3e35e-122">JSON Representation</span></span>
<span data-ttu-id="3e35e-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3e35e-123">Here is a JSON representation of the resource.</span></span>
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




