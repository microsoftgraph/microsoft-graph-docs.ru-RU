---
title: Тип ресурса mediaContentRatingGermany
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e146adc4b2d2e550701a6f152efcdefb41758644
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43437217"
---
# <a name="mediacontentratinggermany-resource-type"></a><span data-ttu-id="304b2-103">Тип ресурса mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="304b2-103">mediaContentRatingGermany resource type</span></span>

<span data-ttu-id="304b2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="304b2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="304b2-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="304b2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="304b2-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="304b2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="304b2-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="304b2-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="304b2-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="304b2-108">Properties</span></span>
|<span data-ttu-id="304b2-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="304b2-109">Property</span></span>|<span data-ttu-id="304b2-110">Тип</span><span class="sxs-lookup"><span data-stu-id="304b2-110">Type</span></span>|<span data-ttu-id="304b2-111">Описание</span><span class="sxs-lookup"><span data-stu-id="304b2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="304b2-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="304b2-112">movieRating</span></span>|[<span data-ttu-id="304b2-113">ратингжерманимовиестипе</span><span class="sxs-lookup"><span data-stu-id="304b2-113">ratingGermanyMoviesType</span></span>](../resources/intune-deviceconfig-ratinggermanymoviestype.md)|<span data-ttu-id="304b2-114">Оценка фильмов выбрана для Германии.</span><span class="sxs-lookup"><span data-stu-id="304b2-114">Movies rating selected for Germany.</span></span> <span data-ttu-id="304b2-115">Возможные значения: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="304b2-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="304b2-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="304b2-116">tvRating</span></span>|[<span data-ttu-id="304b2-117">ратингжерманителевисионтипе</span><span class="sxs-lookup"><span data-stu-id="304b2-117">ratingGermanyTelevisionType</span></span>](../resources/intune-deviceconfig-ratinggermanytelevisiontype.md)|<span data-ttu-id="304b2-118">Рейтинг для телевизора выбран в Германии.</span><span class="sxs-lookup"><span data-stu-id="304b2-118">TV rating selected for Germany.</span></span> <span data-ttu-id="304b2-119">Возможные значения: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="304b2-119">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="304b2-120">Связи</span><span class="sxs-lookup"><span data-stu-id="304b2-120">Relationships</span></span>
<span data-ttu-id="304b2-121">Нет</span><span class="sxs-lookup"><span data-stu-id="304b2-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="304b2-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="304b2-122">JSON Representation</span></span>
<span data-ttu-id="304b2-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="304b2-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingGermany"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingGermany",
  "movieRating": "String",
  "tvRating": "String"
}
```



