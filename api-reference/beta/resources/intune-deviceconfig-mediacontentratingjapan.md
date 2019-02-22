---
title: Тип ресурса mediaContentRatingJapan
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3b10d498edd03850a52aa09ba29e352a143a77c5
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30163443"
---
# <a name="mediacontentratingjapan-resource-type"></a><span data-ttu-id="5df64-103">Тип ресурса mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="5df64-103">mediaContentRatingJapan resource type</span></span>

> <span data-ttu-id="5df64-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5df64-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5df64-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5df64-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5df64-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="5df64-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="5df64-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="5df64-107">Properties</span></span>
|<span data-ttu-id="5df64-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="5df64-108">Property</span></span>|<span data-ttu-id="5df64-109">Тип</span><span class="sxs-lookup"><span data-stu-id="5df64-109">Type</span></span>|<span data-ttu-id="5df64-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5df64-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5df64-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="5df64-111">movieRating</span></span>|[<span data-ttu-id="5df64-112">Ратингжапанмовиестипе</span><span class="sxs-lookup"><span data-stu-id="5df64-112">ratingJapanMoviesType</span></span>](../resources/intune-deviceconfig-ratingjapanmoviestype.md)|<span data-ttu-id="5df64-113">Оценка фильмов выбрана для Японии.</span><span class="sxs-lookup"><span data-stu-id="5df64-113">Movies rating selected for Japan.</span></span> <span data-ttu-id="5df64-114">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="5df64-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="5df64-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="5df64-115">tvRating</span></span>|[<span data-ttu-id="5df64-116">Ратингжапантелевисионтипе</span><span class="sxs-lookup"><span data-stu-id="5df64-116">ratingJapanTelevisionType</span></span>](../resources/intune-deviceconfig-ratingjapantelevisiontype.md)|<span data-ttu-id="5df64-117">Рейтинг для телевизора выбран для Японии.</span><span class="sxs-lookup"><span data-stu-id="5df64-117">TV rating selected for Japan.</span></span> <span data-ttu-id="5df64-118">Возможные значения: `allAllowed`, `allBlocked`, `explicitAllowed`.</span><span class="sxs-lookup"><span data-stu-id="5df64-118">Possible values are: `allAllowed`, `allBlocked`, `explicitAllowed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5df64-119">Связи</span><span class="sxs-lookup"><span data-stu-id="5df64-119">Relationships</span></span>
<span data-ttu-id="5df64-120">Нет</span><span class="sxs-lookup"><span data-stu-id="5df64-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5df64-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5df64-121">JSON Representation</span></span>
<span data-ttu-id="5df64-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5df64-122">Here is a JSON representation of the resource.</span></span>
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




