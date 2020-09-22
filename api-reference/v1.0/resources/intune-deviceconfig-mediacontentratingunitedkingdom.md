---
title: Тип ресурса mediaContentRatingUnitedKingdom
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5e9fd03ebd0834ff63c129216833673255715f76
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48003089"
---
# <a name="mediacontentratingunitedkingdom-resource-type"></a><span data-ttu-id="f3251-103">Тип ресурса mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="f3251-103">mediaContentRatingUnitedKingdom resource type</span></span>

<span data-ttu-id="f3251-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f3251-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f3251-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f3251-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3251-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="f3251-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="f3251-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="f3251-107">Properties</span></span>
|<span data-ttu-id="f3251-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="f3251-108">Property</span></span>|<span data-ttu-id="f3251-109">Тип</span><span class="sxs-lookup"><span data-stu-id="f3251-109">Type</span></span>|<span data-ttu-id="f3251-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f3251-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3251-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="f3251-111">movieRating</span></span>|[<span data-ttu-id="f3251-112">ратингунитедкингдоммовиестипе</span><span class="sxs-lookup"><span data-stu-id="f3251-112">ratingUnitedKingdomMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdommoviestype.md)|<span data-ttu-id="f3251-113">Оценка фильмов выбрана для Великобритании.</span><span class="sxs-lookup"><span data-stu-id="f3251-113">Movies rating selected for United Kingdom.</span></span> <span data-ttu-id="f3251-114">Возможные значения: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="f3251-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span></span>|
|<span data-ttu-id="f3251-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="f3251-115">tvRating</span></span>|[<span data-ttu-id="f3251-116">ратингунитедкингдомтелевисионтипе</span><span class="sxs-lookup"><span data-stu-id="f3251-116">ratingUnitedKingdomTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdomtelevisiontype.md)|<span data-ttu-id="f3251-117">Рейтинг для телевизора выбран для Великобритании.</span><span class="sxs-lookup"><span data-stu-id="f3251-117">TV rating selected for United Kingdom.</span></span> <span data-ttu-id="f3251-118">Возможные значения: `allAllowed`, `allBlocked`, `caution`.</span><span class="sxs-lookup"><span data-stu-id="f3251-118">Possible values are: `allAllowed`, `allBlocked`, `caution`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f3251-119">Связи</span><span class="sxs-lookup"><span data-stu-id="f3251-119">Relationships</span></span>
<span data-ttu-id="f3251-120">Нет</span><span class="sxs-lookup"><span data-stu-id="f3251-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f3251-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f3251-121">JSON Representation</span></span>
<span data-ttu-id="f3251-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f3251-122">Here is a JSON representation of the resource.</span></span>
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









