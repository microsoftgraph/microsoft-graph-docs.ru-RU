---
title: Тип ресурса mediaContentRatingGermany
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3adb081f2b18bbf38327cd56adf90f29333ec146
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43439451"
---
# <a name="mediacontentratinggermany-resource-type"></a><span data-ttu-id="7a331-103">Тип ресурса mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="7a331-103">mediaContentRatingGermany resource type</span></span>

<span data-ttu-id="7a331-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7a331-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7a331-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7a331-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7a331-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="7a331-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="7a331-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="7a331-107">Properties</span></span>
|<span data-ttu-id="7a331-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="7a331-108">Property</span></span>|<span data-ttu-id="7a331-109">Тип</span><span class="sxs-lookup"><span data-stu-id="7a331-109">Type</span></span>|<span data-ttu-id="7a331-110">Описание</span><span class="sxs-lookup"><span data-stu-id="7a331-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a331-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="7a331-111">movieRating</span></span>|[<span data-ttu-id="7a331-112">ратингжерманимовиестипе</span><span class="sxs-lookup"><span data-stu-id="7a331-112">ratingGermanyMoviesType</span></span>](../resources/intune-deviceconfig-ratinggermanymoviestype.md)|<span data-ttu-id="7a331-113">Оценка фильмов выбрана для Германии.</span><span class="sxs-lookup"><span data-stu-id="7a331-113">Movies rating selected for Germany.</span></span> <span data-ttu-id="7a331-114">Возможные значения: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="7a331-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="7a331-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="7a331-115">tvRating</span></span>|[<span data-ttu-id="7a331-116">ратингжерманителевисионтипе</span><span class="sxs-lookup"><span data-stu-id="7a331-116">ratingGermanyTelevisionType</span></span>](../resources/intune-deviceconfig-ratinggermanytelevisiontype.md)|<span data-ttu-id="7a331-117">Рейтинг для телевизора выбран в Германии.</span><span class="sxs-lookup"><span data-stu-id="7a331-117">TV rating selected for Germany.</span></span> <span data-ttu-id="7a331-118">Возможные значения: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="7a331-118">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7a331-119">Связи</span><span class="sxs-lookup"><span data-stu-id="7a331-119">Relationships</span></span>
<span data-ttu-id="7a331-120">Нет</span><span class="sxs-lookup"><span data-stu-id="7a331-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7a331-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7a331-121">JSON Representation</span></span>
<span data-ttu-id="7a331-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7a331-122">Here is a JSON representation of the resource.</span></span>
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







