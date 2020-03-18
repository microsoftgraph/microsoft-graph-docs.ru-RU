---
title: Тип ресурса mediaContentRatingAustralia
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: af27f6f4cfc49e90186aed4ed266b62c9b1a0343
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42788606"
---
# <a name="mediacontentratingaustralia-resource-type"></a><span data-ttu-id="b1fd7-103">Тип ресурса mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="b1fd7-103">mediaContentRatingAustralia resource type</span></span>

> <span data-ttu-id="b1fd7-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1fd7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b1fd7-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b1fd7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1fd7-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="b1fd7-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="b1fd7-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="b1fd7-107">Properties</span></span>
|<span data-ttu-id="b1fd7-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="b1fd7-108">Property</span></span>|<span data-ttu-id="b1fd7-109">Тип</span><span class="sxs-lookup"><span data-stu-id="b1fd7-109">Type</span></span>|<span data-ttu-id="b1fd7-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b1fd7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1fd7-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="b1fd7-111">movieRating</span></span>|[<span data-ttu-id="b1fd7-112">ратингаустралиамовиестипе</span><span class="sxs-lookup"><span data-stu-id="b1fd7-112">ratingAustraliaMoviesType</span></span>](../resources/intune-deviceconfig-ratingaustraliamoviestype.md)|<span data-ttu-id="b1fd7-113">Оценка фильмов выбрана для Австралии.</span><span class="sxs-lookup"><span data-stu-id="b1fd7-113">Movies rating selected for Australia.</span></span> <span data-ttu-id="b1fd7-114">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="b1fd7-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="b1fd7-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="b1fd7-115">tvRating</span></span>|[<span data-ttu-id="b1fd7-116">ратингаустралиателевисионтипе</span><span class="sxs-lookup"><span data-stu-id="b1fd7-116">ratingAustraliaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingaustraliatelevisiontype.md)|<span data-ttu-id="b1fd7-117">Рейтинг для телевизора выбран для Австралии.</span><span class="sxs-lookup"><span data-stu-id="b1fd7-117">TV rating selected for Australia.</span></span> <span data-ttu-id="b1fd7-118">Возможные значения: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span><span class="sxs-lookup"><span data-stu-id="b1fd7-118">Possible values are: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b1fd7-119">Связи</span><span class="sxs-lookup"><span data-stu-id="b1fd7-119">Relationships</span></span>
<span data-ttu-id="b1fd7-120">Нет</span><span class="sxs-lookup"><span data-stu-id="b1fd7-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b1fd7-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b1fd7-121">JSON Representation</span></span>
<span data-ttu-id="b1fd7-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b1fd7-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingAustralia"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingAustralia",
  "movieRating": "String",
  "tvRating": "String"
}
```



