---
title: Тип ресурса mediaContentRatingJapan
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8b1c79e68a530d176445b0395fdb7c4d50996485
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33950888"
---
# <a name="mediacontentratingjapan-resource-type"></a><span data-ttu-id="83180-103">Тип ресурса mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="83180-103">mediaContentRatingJapan resource type</span></span>

> <span data-ttu-id="83180-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="83180-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="83180-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="83180-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="83180-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="83180-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="83180-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="83180-107">Properties</span></span>
|<span data-ttu-id="83180-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="83180-108">Property</span></span>|<span data-ttu-id="83180-109">Тип</span><span class="sxs-lookup"><span data-stu-id="83180-109">Type</span></span>|<span data-ttu-id="83180-110">Описание</span><span class="sxs-lookup"><span data-stu-id="83180-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83180-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="83180-111">movieRating</span></span>|[<span data-ttu-id="83180-112">Ратингжапанмовиестипе</span><span class="sxs-lookup"><span data-stu-id="83180-112">ratingJapanMoviesType</span></span>](../resources/intune-deviceconfig-ratingjapanmoviestype.md)|<span data-ttu-id="83180-113">Оценка фильмов выбрана для Японии.</span><span class="sxs-lookup"><span data-stu-id="83180-113">Movies rating selected for Japan.</span></span> <span data-ttu-id="83180-114">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="83180-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="83180-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="83180-115">tvRating</span></span>|[<span data-ttu-id="83180-116">Ратингжапантелевисионтипе</span><span class="sxs-lookup"><span data-stu-id="83180-116">ratingJapanTelevisionType</span></span>](../resources/intune-deviceconfig-ratingjapantelevisiontype.md)|<span data-ttu-id="83180-117">Рейтинг для телевизора выбран для Японии.</span><span class="sxs-lookup"><span data-stu-id="83180-117">TV rating selected for Japan.</span></span> <span data-ttu-id="83180-118">Возможные значения: `allAllowed`, `allBlocked`, `explicitAllowed`.</span><span class="sxs-lookup"><span data-stu-id="83180-118">Possible values are: `allAllowed`, `allBlocked`, `explicitAllowed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="83180-119">Связи</span><span class="sxs-lookup"><span data-stu-id="83180-119">Relationships</span></span>
<span data-ttu-id="83180-120">Нет</span><span class="sxs-lookup"><span data-stu-id="83180-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="83180-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="83180-121">JSON Representation</span></span>
<span data-ttu-id="83180-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="83180-122">Here is a JSON representation of the resource.</span></span>
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




