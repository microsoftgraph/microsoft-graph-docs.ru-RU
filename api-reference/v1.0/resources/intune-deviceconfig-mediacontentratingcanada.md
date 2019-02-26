---
title: Тип ресурса mediaContentRatingCanada
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 88975975b07eb2805ee5f73cc416e3803d5fe24f
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30253318"
---
# <a name="mediacontentratingcanada-resource-type"></a><span data-ttu-id="2fcc4-103">Тип ресурса mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="2fcc4-103">mediaContentRatingCanada resource type</span></span>

> <span data-ttu-id="2fcc4-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2fcc4-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2fcc4-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="2fcc4-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="2fcc4-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="2fcc4-106">Properties</span></span>
|<span data-ttu-id="2fcc4-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="2fcc4-107">Property</span></span>|<span data-ttu-id="2fcc4-108">Тип</span><span class="sxs-lookup"><span data-stu-id="2fcc4-108">Type</span></span>|<span data-ttu-id="2fcc4-109">Описание</span><span class="sxs-lookup"><span data-stu-id="2fcc4-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2fcc4-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="2fcc4-110">movieRating</span></span>|[<span data-ttu-id="2fcc4-111">Ратингканадамовиестипе</span><span class="sxs-lookup"><span data-stu-id="2fcc4-111">ratingCanadaMoviesType</span></span>](../resources/intune-deviceconfig-ratingcanadamoviestype.md)|<span data-ttu-id="2fcc4-112">Оценка фильмов выбрана для Канады.</span><span class="sxs-lookup"><span data-stu-id="2fcc4-112">Movies rating selected for Canada.</span></span> <span data-ttu-id="2fcc4-113">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span><span class="sxs-lookup"><span data-stu-id="2fcc4-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span></span>|
|<span data-ttu-id="2fcc4-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="2fcc4-114">tvRating</span></span>|[<span data-ttu-id="2fcc4-115">Ратингканадателевисионтипе</span><span class="sxs-lookup"><span data-stu-id="2fcc4-115">ratingCanadaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingcanadatelevisiontype.md)|<span data-ttu-id="2fcc4-116">Рейтинг для телевизора выбран для Канады.</span><span class="sxs-lookup"><span data-stu-id="2fcc4-116">TV rating selected for Canada.</span></span> <span data-ttu-id="2fcc4-117">Возможные значения: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="2fcc4-117">Possible values are: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2fcc4-118">Связи</span><span class="sxs-lookup"><span data-stu-id="2fcc4-118">Relationships</span></span>
<span data-ttu-id="2fcc4-119">Нет</span><span class="sxs-lookup"><span data-stu-id="2fcc4-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2fcc4-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2fcc4-120">JSON Representation</span></span>
<span data-ttu-id="2fcc4-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2fcc4-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingCanada"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingCanada",
  "movieRating": "String",
  "tvRating": "String"
}
```



