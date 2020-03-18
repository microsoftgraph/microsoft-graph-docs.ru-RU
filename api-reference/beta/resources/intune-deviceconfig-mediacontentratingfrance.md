---
title: Тип ресурса mediaContentRatingFrance
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ccfa69711a4bd9790cce28e41fc0585fe34b6dfb
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42788592"
---
# <a name="mediacontentratingfrance-resource-type"></a><span data-ttu-id="a7f46-103">Тип ресурса mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="a7f46-103">mediaContentRatingFrance resource type</span></span>

> <span data-ttu-id="a7f46-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7f46-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a7f46-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a7f46-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a7f46-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="a7f46-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="a7f46-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="a7f46-107">Properties</span></span>
|<span data-ttu-id="a7f46-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="a7f46-108">Property</span></span>|<span data-ttu-id="a7f46-109">Тип</span><span class="sxs-lookup"><span data-stu-id="a7f46-109">Type</span></span>|<span data-ttu-id="a7f46-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a7f46-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7f46-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="a7f46-111">movieRating</span></span>|[<span data-ttu-id="a7f46-112">ратингфранцемовиестипе</span><span class="sxs-lookup"><span data-stu-id="a7f46-112">ratingFranceMoviesType</span></span>](../resources/intune-deviceconfig-ratingfrancemoviestype.md)|<span data-ttu-id="a7f46-113">Оценка фильмов выбрана для Франции.</span><span class="sxs-lookup"><span data-stu-id="a7f46-113">Movies rating selected for France.</span></span> <span data-ttu-id="a7f46-114">Возможные значения: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="a7f46-114">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|
|<span data-ttu-id="a7f46-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="a7f46-115">tvRating</span></span>|[<span data-ttu-id="a7f46-116">ратингфранцетелевисионтипе</span><span class="sxs-lookup"><span data-stu-id="a7f46-116">ratingFranceTelevisionType</span></span>](../resources/intune-deviceconfig-ratingfrancetelevisiontype.md)|<span data-ttu-id="a7f46-117">Рейтинг телевизора выбран для Франции.</span><span class="sxs-lookup"><span data-stu-id="a7f46-117">TV rating selected for France.</span></span> <span data-ttu-id="a7f46-118">Возможные значения: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="a7f46-118">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a7f46-119">Связи</span><span class="sxs-lookup"><span data-stu-id="a7f46-119">Relationships</span></span>
<span data-ttu-id="a7f46-120">Нет</span><span class="sxs-lookup"><span data-stu-id="a7f46-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a7f46-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a7f46-121">JSON Representation</span></span>
<span data-ttu-id="a7f46-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a7f46-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingFrance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingFrance",
  "movieRating": "String",
  "tvRating": "String"
}
```



