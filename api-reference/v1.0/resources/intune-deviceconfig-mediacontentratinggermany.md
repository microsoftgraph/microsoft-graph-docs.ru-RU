---
title: Тип ресурса mediaContentRatingGermany
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1a08891428edd5fec07308e2ff7e44da49eaea93
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530633"
---
# <a name="mediacontentratinggermany-resource-type"></a><span data-ttu-id="19197-103">Тип ресурса mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="19197-103">mediaContentRatingGermany resource type</span></span>

<span data-ttu-id="19197-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="19197-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="19197-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="19197-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="19197-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="19197-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="19197-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="19197-107">Properties</span></span>
|<span data-ttu-id="19197-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="19197-108">Property</span></span>|<span data-ttu-id="19197-109">Тип</span><span class="sxs-lookup"><span data-stu-id="19197-109">Type</span></span>|<span data-ttu-id="19197-110">Описание</span><span class="sxs-lookup"><span data-stu-id="19197-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19197-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="19197-111">movieRating</span></span>|[<span data-ttu-id="19197-112">ратингжерманимовиестипе</span><span class="sxs-lookup"><span data-stu-id="19197-112">ratingGermanyMoviesType</span></span>](../resources/intune-deviceconfig-ratinggermanymoviestype.md)|<span data-ttu-id="19197-113">Оценка фильмов выбрана для Германии.</span><span class="sxs-lookup"><span data-stu-id="19197-113">Movies rating selected for Germany.</span></span> <span data-ttu-id="19197-114">Возможные значения: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="19197-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="19197-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="19197-115">tvRating</span></span>|[<span data-ttu-id="19197-116">ратингжерманителевисионтипе</span><span class="sxs-lookup"><span data-stu-id="19197-116">ratingGermanyTelevisionType</span></span>](../resources/intune-deviceconfig-ratinggermanytelevisiontype.md)|<span data-ttu-id="19197-117">Рейтинг для телевизора выбран в Германии.</span><span class="sxs-lookup"><span data-stu-id="19197-117">TV rating selected for Germany.</span></span> <span data-ttu-id="19197-118">Возможные значения: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="19197-118">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="19197-119">Связи</span><span class="sxs-lookup"><span data-stu-id="19197-119">Relationships</span></span>
<span data-ttu-id="19197-120">Нет</span><span class="sxs-lookup"><span data-stu-id="19197-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="19197-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="19197-121">JSON Representation</span></span>
<span data-ttu-id="19197-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="19197-122">Here is a JSON representation of the resource.</span></span>
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




