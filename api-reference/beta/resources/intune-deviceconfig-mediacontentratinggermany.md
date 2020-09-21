---
title: Тип ресурса mediaContentRatingGermany
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 568f88dd3d595e3fafdf1ac8d201752d19235a8d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47968432"
---
# <a name="mediacontentratinggermany-resource-type"></a><span data-ttu-id="5075a-103">Тип ресурса mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="5075a-103">mediaContentRatingGermany resource type</span></span>

<span data-ttu-id="5075a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5075a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5075a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5075a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5075a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5075a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5075a-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="5075a-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="5075a-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="5075a-108">Properties</span></span>
|<span data-ttu-id="5075a-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="5075a-109">Property</span></span>|<span data-ttu-id="5075a-110">Тип</span><span class="sxs-lookup"><span data-stu-id="5075a-110">Type</span></span>|<span data-ttu-id="5075a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="5075a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5075a-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="5075a-112">movieRating</span></span>|[<span data-ttu-id="5075a-113">ратингжерманимовиестипе</span><span class="sxs-lookup"><span data-stu-id="5075a-113">ratingGermanyMoviesType</span></span>](../resources/intune-deviceconfig-ratinggermanymoviestype.md)|<span data-ttu-id="5075a-114">Оценка фильмов выбрана для Германии.</span><span class="sxs-lookup"><span data-stu-id="5075a-114">Movies rating selected for Germany.</span></span> <span data-ttu-id="5075a-115">Возможные значения: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="5075a-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="5075a-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="5075a-116">tvRating</span></span>|[<span data-ttu-id="5075a-117">ратингжерманителевисионтипе</span><span class="sxs-lookup"><span data-stu-id="5075a-117">ratingGermanyTelevisionType</span></span>](../resources/intune-deviceconfig-ratinggermanytelevisiontype.md)|<span data-ttu-id="5075a-118">Рейтинг для телевизора выбран в Германии.</span><span class="sxs-lookup"><span data-stu-id="5075a-118">TV rating selected for Germany.</span></span> <span data-ttu-id="5075a-119">Возможные значения: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="5075a-119">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5075a-120">Связи</span><span class="sxs-lookup"><span data-stu-id="5075a-120">Relationships</span></span>
<span data-ttu-id="5075a-121">Нет</span><span class="sxs-lookup"><span data-stu-id="5075a-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5075a-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5075a-122">JSON Representation</span></span>
<span data-ttu-id="5075a-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5075a-123">Here is a JSON representation of the resource.</span></span>
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






