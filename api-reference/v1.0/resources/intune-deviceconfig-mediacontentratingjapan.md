---
title: Тип ресурса mediaContentRatingJapan
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b31ca971ea15470853a4ec9d6e1cf89a76fa3b9b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43473155"
---
# <a name="mediacontentratingjapan-resource-type"></a><span data-ttu-id="14474-103">Тип ресурса mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="14474-103">mediaContentRatingJapan resource type</span></span>

<span data-ttu-id="14474-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="14474-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="14474-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="14474-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="14474-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="14474-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="14474-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="14474-107">Properties</span></span>
|<span data-ttu-id="14474-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="14474-108">Property</span></span>|<span data-ttu-id="14474-109">Тип</span><span class="sxs-lookup"><span data-stu-id="14474-109">Type</span></span>|<span data-ttu-id="14474-110">Описание</span><span class="sxs-lookup"><span data-stu-id="14474-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14474-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="14474-111">movieRating</span></span>|[<span data-ttu-id="14474-112">ратингжапанмовиестипе</span><span class="sxs-lookup"><span data-stu-id="14474-112">ratingJapanMoviesType</span></span>](../resources/intune-deviceconfig-ratingjapanmoviestype.md)|<span data-ttu-id="14474-113">Оценка фильмов выбрана для Японии.</span><span class="sxs-lookup"><span data-stu-id="14474-113">Movies rating selected for Japan.</span></span> <span data-ttu-id="14474-114">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="14474-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="14474-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="14474-115">tvRating</span></span>|[<span data-ttu-id="14474-116">ратингжапантелевисионтипе</span><span class="sxs-lookup"><span data-stu-id="14474-116">ratingJapanTelevisionType</span></span>](../resources/intune-deviceconfig-ratingjapantelevisiontype.md)|<span data-ttu-id="14474-117">Рейтинг для телевизора выбран для Японии.</span><span class="sxs-lookup"><span data-stu-id="14474-117">TV rating selected for Japan.</span></span> <span data-ttu-id="14474-118">Возможные значения: `allAllowed`, `allBlocked`, `explicitAllowed`.</span><span class="sxs-lookup"><span data-stu-id="14474-118">Possible values are: `allAllowed`, `allBlocked`, `explicitAllowed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="14474-119">Отношения</span><span class="sxs-lookup"><span data-stu-id="14474-119">Relationships</span></span>
<span data-ttu-id="14474-120">Нет</span><span class="sxs-lookup"><span data-stu-id="14474-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="14474-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="14474-121">JSON Representation</span></span>
<span data-ttu-id="14474-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="14474-122">Here is a JSON representation of the resource.</span></span>
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







