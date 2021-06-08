---
title: Тип ресурса mediaContentRatingGermany
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 06cad29f595ecc1124344d2ad72bed50a71b4314
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52757768"
---
# <a name="mediacontentratinggermany-resource-type"></a><span data-ttu-id="d9888-103">Тип ресурса mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="d9888-103">mediaContentRatingGermany resource type</span></span>

<span data-ttu-id="d9888-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d9888-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d9888-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d9888-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d9888-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="d9888-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="d9888-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="d9888-107">Properties</span></span>
|<span data-ttu-id="d9888-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="d9888-108">Property</span></span>|<span data-ttu-id="d9888-109">Тип</span><span class="sxs-lookup"><span data-stu-id="d9888-109">Type</span></span>|<span data-ttu-id="d9888-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d9888-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9888-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="d9888-111">movieRating</span></span>|[<span data-ttu-id="d9888-112">ratingGermanyMoviesType</span><span class="sxs-lookup"><span data-stu-id="d9888-112">ratingGermanyMoviesType</span></span>](../resources/intune-deviceconfig-ratinggermanymoviestype.md)|<span data-ttu-id="d9888-113">Рейтинг фильмов, выбранный для Германии.</span><span class="sxs-lookup"><span data-stu-id="d9888-113">Movies rating selected for Germany.</span></span> <span data-ttu-id="d9888-114">Возможные значения: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="d9888-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="d9888-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="d9888-115">tvRating</span></span>|[<span data-ttu-id="d9888-116">ratingGermanyTelevisionType</span><span class="sxs-lookup"><span data-stu-id="d9888-116">ratingGermanyTelevisionType</span></span>](../resources/intune-deviceconfig-ratinggermanytelevisiontype.md)|<span data-ttu-id="d9888-117">Телевизионный рейтинг, выбранный для Германии.</span><span class="sxs-lookup"><span data-stu-id="d9888-117">TV rating selected for Germany.</span></span> <span data-ttu-id="d9888-118">Возможные значения: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="d9888-118">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d9888-119">Отношения</span><span class="sxs-lookup"><span data-stu-id="d9888-119">Relationships</span></span>
<span data-ttu-id="d9888-120">Нет</span><span class="sxs-lookup"><span data-stu-id="d9888-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d9888-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d9888-121">JSON Representation</span></span>
<span data-ttu-id="d9888-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d9888-122">Here is a JSON representation of the resource.</span></span>
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




