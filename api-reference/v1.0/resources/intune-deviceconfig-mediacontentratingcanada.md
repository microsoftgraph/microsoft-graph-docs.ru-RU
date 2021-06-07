---
title: Тип ресурса mediaContentRatingCanada
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: eff3a957e242dfad4840ad5d616cec54f9a3c344
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755044"
---
# <a name="mediacontentratingcanada-resource-type"></a><span data-ttu-id="1261d-103">Тип ресурса mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="1261d-103">mediaContentRatingCanada resource type</span></span>

<span data-ttu-id="1261d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1261d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1261d-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1261d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1261d-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="1261d-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="1261d-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="1261d-107">Properties</span></span>
|<span data-ttu-id="1261d-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="1261d-108">Property</span></span>|<span data-ttu-id="1261d-109">Тип</span><span class="sxs-lookup"><span data-stu-id="1261d-109">Type</span></span>|<span data-ttu-id="1261d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="1261d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1261d-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="1261d-111">movieRating</span></span>|[<span data-ttu-id="1261d-112">ratingCanadaMoviesType</span><span class="sxs-lookup"><span data-stu-id="1261d-112">ratingCanadaMoviesType</span></span>](../resources/intune-deviceconfig-ratingcanadamoviestype.md)|<span data-ttu-id="1261d-113">Рейтинг фильмов, выбранный для Канады.</span><span class="sxs-lookup"><span data-stu-id="1261d-113">Movies rating selected for Canada.</span></span> <span data-ttu-id="1261d-114">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span><span class="sxs-lookup"><span data-stu-id="1261d-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span></span>|
|<span data-ttu-id="1261d-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="1261d-115">tvRating</span></span>|[<span data-ttu-id="1261d-116">ratingCanadaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="1261d-116">ratingCanadaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingcanadatelevisiontype.md)|<span data-ttu-id="1261d-117">Телевизионный рейтинг, выбранный для Канады.</span><span class="sxs-lookup"><span data-stu-id="1261d-117">TV rating selected for Canada.</span></span> <span data-ttu-id="1261d-118">Возможные значения: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="1261d-118">Possible values are: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1261d-119">Отношения</span><span class="sxs-lookup"><span data-stu-id="1261d-119">Relationships</span></span>
<span data-ttu-id="1261d-120">Нет</span><span class="sxs-lookup"><span data-stu-id="1261d-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1261d-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1261d-121">JSON Representation</span></span>
<span data-ttu-id="1261d-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1261d-122">Here is a JSON representation of the resource.</span></span>
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




