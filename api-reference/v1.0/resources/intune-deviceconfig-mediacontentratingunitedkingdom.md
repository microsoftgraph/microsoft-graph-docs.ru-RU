---
title: Тип ресурса mediaContentRatingUnitedKingdom
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f4ee57f4cbc1621fbbdbf7962a5d89719e7e02e9
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760017"
---
# <a name="mediacontentratingunitedkingdom-resource-type"></a><span data-ttu-id="9fa95-103">Тип ресурса mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="9fa95-103">mediaContentRatingUnitedKingdom resource type</span></span>

<span data-ttu-id="9fa95-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9fa95-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9fa95-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9fa95-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9fa95-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="9fa95-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="9fa95-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="9fa95-107">Properties</span></span>
|<span data-ttu-id="9fa95-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="9fa95-108">Property</span></span>|<span data-ttu-id="9fa95-109">Тип</span><span class="sxs-lookup"><span data-stu-id="9fa95-109">Type</span></span>|<span data-ttu-id="9fa95-110">Описание</span><span class="sxs-lookup"><span data-stu-id="9fa95-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9fa95-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="9fa95-111">movieRating</span></span>|[<span data-ttu-id="9fa95-112">ratingUnitedKingdomMoviesType</span><span class="sxs-lookup"><span data-stu-id="9fa95-112">ratingUnitedKingdomMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdommoviestype.md)|<span data-ttu-id="9fa95-113">Рейтинг фильмов, выбранный для Великобритании.</span><span class="sxs-lookup"><span data-stu-id="9fa95-113">Movies rating selected for United Kingdom.</span></span> <span data-ttu-id="9fa95-114">Возможные значения: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="9fa95-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span></span>|
|<span data-ttu-id="9fa95-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="9fa95-115">tvRating</span></span>|[<span data-ttu-id="9fa95-116">ratingUnitedKingdomTelevisionType</span><span class="sxs-lookup"><span data-stu-id="9fa95-116">ratingUnitedKingdomTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdomtelevisiontype.md)|<span data-ttu-id="9fa95-117">Телевизионный рейтинг, выбранный для Соединенного Королевства.</span><span class="sxs-lookup"><span data-stu-id="9fa95-117">TV rating selected for United Kingdom.</span></span> <span data-ttu-id="9fa95-118">Возможные значения: `allAllowed`, `allBlocked`, `caution`.</span><span class="sxs-lookup"><span data-stu-id="9fa95-118">Possible values are: `allAllowed`, `allBlocked`, `caution`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9fa95-119">Связи</span><span class="sxs-lookup"><span data-stu-id="9fa95-119">Relationships</span></span>
<span data-ttu-id="9fa95-120">Нет</span><span class="sxs-lookup"><span data-stu-id="9fa95-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9fa95-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9fa95-121">JSON Representation</span></span>
<span data-ttu-id="9fa95-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9fa95-122">Here is a JSON representation of the resource.</span></span>
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




