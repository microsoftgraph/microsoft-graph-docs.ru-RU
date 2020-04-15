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
# <a name="mediacontentratinggermany-resource-type"></a><span data-ttu-id="cfcdd-103">Тип ресурса mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="cfcdd-103">mediaContentRatingGermany resource type</span></span>

<span data-ttu-id="cfcdd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cfcdd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cfcdd-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cfcdd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cfcdd-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="cfcdd-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="cfcdd-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="cfcdd-107">Properties</span></span>
|<span data-ttu-id="cfcdd-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="cfcdd-108">Property</span></span>|<span data-ttu-id="cfcdd-109">Тип</span><span class="sxs-lookup"><span data-stu-id="cfcdd-109">Type</span></span>|<span data-ttu-id="cfcdd-110">Описание</span><span class="sxs-lookup"><span data-stu-id="cfcdd-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cfcdd-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="cfcdd-111">movieRating</span></span>|[<span data-ttu-id="cfcdd-112">ратингжерманимовиестипе</span><span class="sxs-lookup"><span data-stu-id="cfcdd-112">ratingGermanyMoviesType</span></span>](../resources/intune-deviceconfig-ratinggermanymoviestype.md)|<span data-ttu-id="cfcdd-113">Оценка фильмов выбрана для Германии.</span><span class="sxs-lookup"><span data-stu-id="cfcdd-113">Movies rating selected for Germany.</span></span> <span data-ttu-id="cfcdd-114">Возможные значения: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="cfcdd-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="cfcdd-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="cfcdd-115">tvRating</span></span>|[<span data-ttu-id="cfcdd-116">ратингжерманителевисионтипе</span><span class="sxs-lookup"><span data-stu-id="cfcdd-116">ratingGermanyTelevisionType</span></span>](../resources/intune-deviceconfig-ratinggermanytelevisiontype.md)|<span data-ttu-id="cfcdd-117">Рейтинг для телевизора выбран в Германии.</span><span class="sxs-lookup"><span data-stu-id="cfcdd-117">TV rating selected for Germany.</span></span> <span data-ttu-id="cfcdd-118">Возможные значения: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="cfcdd-118">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cfcdd-119">Отношения</span><span class="sxs-lookup"><span data-stu-id="cfcdd-119">Relationships</span></span>
<span data-ttu-id="cfcdd-120">Нет</span><span class="sxs-lookup"><span data-stu-id="cfcdd-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cfcdd-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cfcdd-121">JSON Representation</span></span>
<span data-ttu-id="cfcdd-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cfcdd-122">Here is a JSON representation of the resource.</span></span>
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







