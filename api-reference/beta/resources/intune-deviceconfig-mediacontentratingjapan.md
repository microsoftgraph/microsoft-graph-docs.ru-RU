---
title: Тип ресурса mediaContentRatingJapan
description: Н/Д
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1c129fb2853025758fc71aff381efe500d38ec8f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394840"
---
# <a name="mediacontentratingjapan-resource-type"></a><span data-ttu-id="56cad-103">Тип ресурса mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="56cad-103">mediaContentRatingJapan resource type</span></span>

> <span data-ttu-id="56cad-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="56cad-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="56cad-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="56cad-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="56cad-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="56cad-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="56cad-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="56cad-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="56cad-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="56cad-108">Properties</span></span>
|<span data-ttu-id="56cad-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="56cad-109">Property</span></span>|<span data-ttu-id="56cad-110">Тип</span><span class="sxs-lookup"><span data-stu-id="56cad-110">Type</span></span>|<span data-ttu-id="56cad-111">Описание</span><span class="sxs-lookup"><span data-stu-id="56cad-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56cad-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="56cad-112">movieRating</span></span>|[<span data-ttu-id="56cad-113">ratingJapanMoviesType</span><span class="sxs-lookup"><span data-stu-id="56cad-113">ratingJapanMoviesType</span></span>](../resources/intune-deviceconfig-ratingjapanmoviestype.md)|<span data-ttu-id="56cad-114">Оценка выбранных для Японии фильмы.</span><span class="sxs-lookup"><span data-stu-id="56cad-114">Movies rating selected for Japan.</span></span> <span data-ttu-id="56cad-115">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="56cad-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="56cad-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="56cad-116">tvRating</span></span>|[<span data-ttu-id="56cad-117">ratingJapanTelevisionType</span><span class="sxs-lookup"><span data-stu-id="56cad-117">ratingJapanTelevisionType</span></span>](../resources/intune-deviceconfig-ratingjapantelevisiontype.md)|<span data-ttu-id="56cad-118">Оценка TV, выбранной для Японии.</span><span class="sxs-lookup"><span data-stu-id="56cad-118">TV rating selected for Japan.</span></span> <span data-ttu-id="56cad-119">Возможные значения: `allAllowed`, `allBlocked`, `explicitAllowed`.</span><span class="sxs-lookup"><span data-stu-id="56cad-119">Possible values are: `allAllowed`, `allBlocked`, `explicitAllowed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="56cad-120">Связи</span><span class="sxs-lookup"><span data-stu-id="56cad-120">Relationships</span></span>
<span data-ttu-id="56cad-121">Нет</span><span class="sxs-lookup"><span data-stu-id="56cad-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="56cad-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="56cad-122">JSON Representation</span></span>
<span data-ttu-id="56cad-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="56cad-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingJapan"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingJapan",
  "movieRating": "String",
  "tvRating": "String"
}
```




