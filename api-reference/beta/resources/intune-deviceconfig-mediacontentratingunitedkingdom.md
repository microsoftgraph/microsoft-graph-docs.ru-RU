---
title: Тип ресурса mediaContentRatingUnitedKingdom
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: bc6be04b245e07d9dea11dae750ff5e56b68a5e0
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42788557"
---
# <a name="mediacontentratingunitedkingdom-resource-type"></a><span data-ttu-id="f856d-103">Тип ресурса mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="f856d-103">mediaContentRatingUnitedKingdom resource type</span></span>

> <span data-ttu-id="f856d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f856d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f856d-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f856d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f856d-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="f856d-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="f856d-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="f856d-107">Properties</span></span>
|<span data-ttu-id="f856d-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="f856d-108">Property</span></span>|<span data-ttu-id="f856d-109">Тип</span><span class="sxs-lookup"><span data-stu-id="f856d-109">Type</span></span>|<span data-ttu-id="f856d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f856d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f856d-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="f856d-111">movieRating</span></span>|[<span data-ttu-id="f856d-112">ратингунитедкингдоммовиестипе</span><span class="sxs-lookup"><span data-stu-id="f856d-112">ratingUnitedKingdomMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdommoviestype.md)|<span data-ttu-id="f856d-113">Оценка фильмов выбрана для Великобритании.</span><span class="sxs-lookup"><span data-stu-id="f856d-113">Movies rating selected for United Kingdom.</span></span> <span data-ttu-id="f856d-114">Возможные значения: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="f856d-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span></span>|
|<span data-ttu-id="f856d-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="f856d-115">tvRating</span></span>|[<span data-ttu-id="f856d-116">ратингунитедкингдомтелевисионтипе</span><span class="sxs-lookup"><span data-stu-id="f856d-116">ratingUnitedKingdomTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdomtelevisiontype.md)|<span data-ttu-id="f856d-117">Рейтинг для телевизора выбран для Великобритании.</span><span class="sxs-lookup"><span data-stu-id="f856d-117">TV rating selected for United Kingdom.</span></span> <span data-ttu-id="f856d-118">Возможные значения: `allAllowed`, `allBlocked`, `caution`.</span><span class="sxs-lookup"><span data-stu-id="f856d-118">Possible values are: `allAllowed`, `allBlocked`, `caution`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f856d-119">Связи</span><span class="sxs-lookup"><span data-stu-id="f856d-119">Relationships</span></span>
<span data-ttu-id="f856d-120">Нет</span><span class="sxs-lookup"><span data-stu-id="f856d-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f856d-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f856d-121">JSON Representation</span></span>
<span data-ttu-id="f856d-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f856d-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingUnitedKingdom"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingUnitedKingdom",
  "movieRating": "String",
  "tvRating": "String"
}
```



