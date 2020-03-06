---
title: Тип ресурса mediaContentRatingJapan
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d7b4efd96b766eef9104baaa694d166eb22df340
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530619"
---
# <a name="mediacontentratingjapan-resource-type"></a><span data-ttu-id="e0032-103">Тип ресурса mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="e0032-103">mediaContentRatingJapan resource type</span></span>

<span data-ttu-id="e0032-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e0032-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e0032-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e0032-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e0032-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="e0032-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="e0032-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="e0032-107">Properties</span></span>
|<span data-ttu-id="e0032-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="e0032-108">Property</span></span>|<span data-ttu-id="e0032-109">Тип</span><span class="sxs-lookup"><span data-stu-id="e0032-109">Type</span></span>|<span data-ttu-id="e0032-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e0032-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0032-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="e0032-111">movieRating</span></span>|[<span data-ttu-id="e0032-112">ратингжапанмовиестипе</span><span class="sxs-lookup"><span data-stu-id="e0032-112">ratingJapanMoviesType</span></span>](../resources/intune-deviceconfig-ratingjapanmoviestype.md)|<span data-ttu-id="e0032-113">Оценка фильмов выбрана для Японии.</span><span class="sxs-lookup"><span data-stu-id="e0032-113">Movies rating selected for Japan.</span></span> <span data-ttu-id="e0032-114">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="e0032-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="e0032-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="e0032-115">tvRating</span></span>|[<span data-ttu-id="e0032-116">ратингжапантелевисионтипе</span><span class="sxs-lookup"><span data-stu-id="e0032-116">ratingJapanTelevisionType</span></span>](../resources/intune-deviceconfig-ratingjapantelevisiontype.md)|<span data-ttu-id="e0032-117">Рейтинг для телевизора выбран для Японии.</span><span class="sxs-lookup"><span data-stu-id="e0032-117">TV rating selected for Japan.</span></span> <span data-ttu-id="e0032-118">Возможные значения: `allAllowed`, `allBlocked`, `explicitAllowed`.</span><span class="sxs-lookup"><span data-stu-id="e0032-118">Possible values are: `allAllowed`, `allBlocked`, `explicitAllowed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e0032-119">Связи</span><span class="sxs-lookup"><span data-stu-id="e0032-119">Relationships</span></span>
<span data-ttu-id="e0032-120">Нет</span><span class="sxs-lookup"><span data-stu-id="e0032-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e0032-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e0032-121">JSON Representation</span></span>
<span data-ttu-id="e0032-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e0032-122">Here is a JSON representation of the resource.</span></span>
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




