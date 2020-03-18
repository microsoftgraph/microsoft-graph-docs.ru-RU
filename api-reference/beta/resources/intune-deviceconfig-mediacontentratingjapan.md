---
title: Тип ресурса mediaContentRatingJapan
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8c659cfc0fb4528c7ed94025c0b1927a3bd67e4b
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42788571"
---
# <a name="mediacontentratingjapan-resource-type"></a><span data-ttu-id="cf7b3-103">Тип ресурса mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="cf7b3-103">mediaContentRatingJapan resource type</span></span>

> <span data-ttu-id="cf7b3-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cf7b3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cf7b3-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cf7b3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cf7b3-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="cf7b3-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="cf7b3-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="cf7b3-107">Properties</span></span>
|<span data-ttu-id="cf7b3-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="cf7b3-108">Property</span></span>|<span data-ttu-id="cf7b3-109">Тип</span><span class="sxs-lookup"><span data-stu-id="cf7b3-109">Type</span></span>|<span data-ttu-id="cf7b3-110">Описание</span><span class="sxs-lookup"><span data-stu-id="cf7b3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf7b3-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="cf7b3-111">movieRating</span></span>|[<span data-ttu-id="cf7b3-112">ратингжапанмовиестипе</span><span class="sxs-lookup"><span data-stu-id="cf7b3-112">ratingJapanMoviesType</span></span>](../resources/intune-deviceconfig-ratingjapanmoviestype.md)|<span data-ttu-id="cf7b3-113">Оценка фильмов выбрана для Японии.</span><span class="sxs-lookup"><span data-stu-id="cf7b3-113">Movies rating selected for Japan.</span></span> <span data-ttu-id="cf7b3-114">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="cf7b3-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="cf7b3-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="cf7b3-115">tvRating</span></span>|[<span data-ttu-id="cf7b3-116">ратингжапантелевисионтипе</span><span class="sxs-lookup"><span data-stu-id="cf7b3-116">ratingJapanTelevisionType</span></span>](../resources/intune-deviceconfig-ratingjapantelevisiontype.md)|<span data-ttu-id="cf7b3-117">Рейтинг для телевизора выбран для Японии.</span><span class="sxs-lookup"><span data-stu-id="cf7b3-117">TV rating selected for Japan.</span></span> <span data-ttu-id="cf7b3-118">Возможные значения: `allAllowed`, `allBlocked`, `explicitAllowed`.</span><span class="sxs-lookup"><span data-stu-id="cf7b3-118">Possible values are: `allAllowed`, `allBlocked`, `explicitAllowed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cf7b3-119">Связи</span><span class="sxs-lookup"><span data-stu-id="cf7b3-119">Relationships</span></span>
<span data-ttu-id="cf7b3-120">Нет</span><span class="sxs-lookup"><span data-stu-id="cf7b3-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cf7b3-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cf7b3-121">JSON Representation</span></span>
<span data-ttu-id="cf7b3-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cf7b3-122">Here is a JSON representation of the resource.</span></span>
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



