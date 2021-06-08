---
title: Тип ресурса mediaContentRatingJapan
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 691b723f2140bbdda370bbf5b46330579ca0a871
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758836"
---
# <a name="mediacontentratingjapan-resource-type"></a><span data-ttu-id="c2021-103">Тип ресурса mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="c2021-103">mediaContentRatingJapan resource type</span></span>

<span data-ttu-id="c2021-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c2021-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c2021-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c2021-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c2021-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="c2021-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="c2021-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="c2021-107">Properties</span></span>
|<span data-ttu-id="c2021-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="c2021-108">Property</span></span>|<span data-ttu-id="c2021-109">Тип</span><span class="sxs-lookup"><span data-stu-id="c2021-109">Type</span></span>|<span data-ttu-id="c2021-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c2021-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2021-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="c2021-111">movieRating</span></span>|[<span data-ttu-id="c2021-112">ratingJapanMoviesType</span><span class="sxs-lookup"><span data-stu-id="c2021-112">ratingJapanMoviesType</span></span>](../resources/intune-deviceconfig-ratingjapanmoviestype.md)|<span data-ttu-id="c2021-113">Рейтинг фильмов, выбранный для Японии.</span><span class="sxs-lookup"><span data-stu-id="c2021-113">Movies rating selected for Japan.</span></span> <span data-ttu-id="c2021-114">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="c2021-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="c2021-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="c2021-115">tvRating</span></span>|[<span data-ttu-id="c2021-116">ratingJapanTelevisionType</span><span class="sxs-lookup"><span data-stu-id="c2021-116">ratingJapanTelevisionType</span></span>](../resources/intune-deviceconfig-ratingjapantelevisiontype.md)|<span data-ttu-id="c2021-117">Телевизионный рейтинг, выбранный для Японии.</span><span class="sxs-lookup"><span data-stu-id="c2021-117">TV rating selected for Japan.</span></span> <span data-ttu-id="c2021-118">Возможные значения: `allAllowed`, `allBlocked`, `explicitAllowed`.</span><span class="sxs-lookup"><span data-stu-id="c2021-118">Possible values are: `allAllowed`, `allBlocked`, `explicitAllowed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c2021-119">Связи</span><span class="sxs-lookup"><span data-stu-id="c2021-119">Relationships</span></span>
<span data-ttu-id="c2021-120">Нет</span><span class="sxs-lookup"><span data-stu-id="c2021-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c2021-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c2021-121">JSON Representation</span></span>
<span data-ttu-id="c2021-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c2021-122">Here is a JSON representation of the resource.</span></span>
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




