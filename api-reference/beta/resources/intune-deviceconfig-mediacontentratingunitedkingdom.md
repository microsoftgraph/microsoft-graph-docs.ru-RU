---
title: Тип ресурса mediaContentRatingUnitedKingdom
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2f35198006e08ca1ecd4e0ccd2200366c0607214
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35970103"
---
# <a name="mediacontentratingunitedkingdom-resource-type"></a><span data-ttu-id="2a53a-103">Тип ресурса mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="2a53a-103">mediaContentRatingUnitedKingdom resource type</span></span>

> <span data-ttu-id="2a53a-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a53a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2a53a-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2a53a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2a53a-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="2a53a-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="2a53a-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="2a53a-107">Properties</span></span>
|<span data-ttu-id="2a53a-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="2a53a-108">Property</span></span>|<span data-ttu-id="2a53a-109">Тип</span><span class="sxs-lookup"><span data-stu-id="2a53a-109">Type</span></span>|<span data-ttu-id="2a53a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2a53a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a53a-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="2a53a-111">movieRating</span></span>|[<span data-ttu-id="2a53a-112">Ратингунитедкингдоммовиестипе</span><span class="sxs-lookup"><span data-stu-id="2a53a-112">ratingUnitedKingdomMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdommoviestype.md)|<span data-ttu-id="2a53a-113">Оценка фильмов выбрана для Великобритании.</span><span class="sxs-lookup"><span data-stu-id="2a53a-113">Movies rating selected for United Kingdom.</span></span> <span data-ttu-id="2a53a-114">Возможные значения: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="2a53a-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span></span>|
|<span data-ttu-id="2a53a-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="2a53a-115">tvRating</span></span>|[<span data-ttu-id="2a53a-116">Ратингунитедкингдомтелевисионтипе</span><span class="sxs-lookup"><span data-stu-id="2a53a-116">ratingUnitedKingdomTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdomtelevisiontype.md)|<span data-ttu-id="2a53a-117">Рейтинг для телевизора выбран для Великобритании.</span><span class="sxs-lookup"><span data-stu-id="2a53a-117">TV rating selected for United Kingdom.</span></span> <span data-ttu-id="2a53a-118">Возможные значения: `allAllowed`, `allBlocked`, `caution`.</span><span class="sxs-lookup"><span data-stu-id="2a53a-118">Possible values are: `allAllowed`, `allBlocked`, `caution`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2a53a-119">Отношения</span><span class="sxs-lookup"><span data-stu-id="2a53a-119">Relationships</span></span>
<span data-ttu-id="2a53a-120">Нет</span><span class="sxs-lookup"><span data-stu-id="2a53a-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2a53a-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2a53a-121">JSON Representation</span></span>
<span data-ttu-id="2a53a-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2a53a-122">Here is a JSON representation of the resource.</span></span>
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





