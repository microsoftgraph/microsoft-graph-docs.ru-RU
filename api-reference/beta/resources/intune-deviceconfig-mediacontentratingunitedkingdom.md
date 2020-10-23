---
title: Тип ресурса mediaContentRatingUnitedKingdom
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6f4810e8fa69e391b48c1048595a8da3c9766f4c
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48707152"
---
# <a name="mediacontentratingunitedkingdom-resource-type"></a><span data-ttu-id="bd163-103">Тип ресурса mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="bd163-103">mediaContentRatingUnitedKingdom resource type</span></span>

<span data-ttu-id="bd163-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bd163-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bd163-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd163-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bd163-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bd163-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bd163-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="bd163-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="bd163-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="bd163-108">Properties</span></span>
|<span data-ttu-id="bd163-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="bd163-109">Property</span></span>|<span data-ttu-id="bd163-110">Тип</span><span class="sxs-lookup"><span data-stu-id="bd163-110">Type</span></span>|<span data-ttu-id="bd163-111">Описание</span><span class="sxs-lookup"><span data-stu-id="bd163-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bd163-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="bd163-112">movieRating</span></span>|[<span data-ttu-id="bd163-113">ратингунитедкингдоммовиестипе</span><span class="sxs-lookup"><span data-stu-id="bd163-113">ratingUnitedKingdomMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdommoviestype.md)|<span data-ttu-id="bd163-114">Оценка фильмов выбрана для Великобритании.</span><span class="sxs-lookup"><span data-stu-id="bd163-114">Movies rating selected for United Kingdom.</span></span> <span data-ttu-id="bd163-115">Возможные значения: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="bd163-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span></span>|
|<span data-ttu-id="bd163-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="bd163-116">tvRating</span></span>|[<span data-ttu-id="bd163-117">ратингунитедкингдомтелевисионтипе</span><span class="sxs-lookup"><span data-stu-id="bd163-117">ratingUnitedKingdomTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdomtelevisiontype.md)|<span data-ttu-id="bd163-118">Рейтинг для телевизора выбран для Великобритании.</span><span class="sxs-lookup"><span data-stu-id="bd163-118">TV rating selected for United Kingdom.</span></span> <span data-ttu-id="bd163-119">Возможные значения: `allAllowed`, `allBlocked`, `caution`.</span><span class="sxs-lookup"><span data-stu-id="bd163-119">Possible values are: `allAllowed`, `allBlocked`, `caution`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bd163-120">Связи</span><span class="sxs-lookup"><span data-stu-id="bd163-120">Relationships</span></span>
<span data-ttu-id="bd163-121">Нет</span><span class="sxs-lookup"><span data-stu-id="bd163-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bd163-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bd163-122">JSON Representation</span></span>
<span data-ttu-id="bd163-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bd163-123">Here is a JSON representation of the resource.</span></span>
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





