---
title: Тип ресурса mediaContentRatingCanada
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 08673417c883c2aa2a8082010a0eaa001ca02004
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43410081"
---
# <a name="mediacontentratingcanada-resource-type"></a><span data-ttu-id="186eb-103">Тип ресурса mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="186eb-103">mediaContentRatingCanada resource type</span></span>

<span data-ttu-id="186eb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="186eb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="186eb-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="186eb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="186eb-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="186eb-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="186eb-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="186eb-107">Properties</span></span>
|<span data-ttu-id="186eb-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="186eb-108">Property</span></span>|<span data-ttu-id="186eb-109">Тип</span><span class="sxs-lookup"><span data-stu-id="186eb-109">Type</span></span>|<span data-ttu-id="186eb-110">Описание</span><span class="sxs-lookup"><span data-stu-id="186eb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="186eb-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="186eb-111">movieRating</span></span>|[<span data-ttu-id="186eb-112">ратингканадамовиестипе</span><span class="sxs-lookup"><span data-stu-id="186eb-112">ratingCanadaMoviesType</span></span>](../resources/intune-deviceconfig-ratingcanadamoviestype.md)|<span data-ttu-id="186eb-113">Оценка фильмов выбрана для Канады.</span><span class="sxs-lookup"><span data-stu-id="186eb-113">Movies rating selected for Canada.</span></span> <span data-ttu-id="186eb-114">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span><span class="sxs-lookup"><span data-stu-id="186eb-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span></span>|
|<span data-ttu-id="186eb-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="186eb-115">tvRating</span></span>|[<span data-ttu-id="186eb-116">ратингканадателевисионтипе</span><span class="sxs-lookup"><span data-stu-id="186eb-116">ratingCanadaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingcanadatelevisiontype.md)|<span data-ttu-id="186eb-117">Рейтинг для телевизора выбран для Канады.</span><span class="sxs-lookup"><span data-stu-id="186eb-117">TV rating selected for Canada.</span></span> <span data-ttu-id="186eb-118">Возможные значения: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="186eb-118">Possible values are: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="186eb-119">Связи</span><span class="sxs-lookup"><span data-stu-id="186eb-119">Relationships</span></span>
<span data-ttu-id="186eb-120">Нет</span><span class="sxs-lookup"><span data-stu-id="186eb-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="186eb-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="186eb-121">JSON Representation</span></span>
<span data-ttu-id="186eb-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="186eb-122">Here is a JSON representation of the resource.</span></span>
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







