---
title: Тип ресурса mediaContentRatingUnitedKingdom
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d298120444078a9b45d17e6237607b7a382fdfb7
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43473101"
---
# <a name="mediacontentratingunitedkingdom-resource-type"></a><span data-ttu-id="9d97c-103">Тип ресурса mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="9d97c-103">mediaContentRatingUnitedKingdom resource type</span></span>

<span data-ttu-id="9d97c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9d97c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9d97c-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9d97c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9d97c-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="9d97c-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="9d97c-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="9d97c-107">Properties</span></span>
|<span data-ttu-id="9d97c-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="9d97c-108">Property</span></span>|<span data-ttu-id="9d97c-109">Тип</span><span class="sxs-lookup"><span data-stu-id="9d97c-109">Type</span></span>|<span data-ttu-id="9d97c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="9d97c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d97c-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="9d97c-111">movieRating</span></span>|[<span data-ttu-id="9d97c-112">ратингунитедкингдоммовиестипе</span><span class="sxs-lookup"><span data-stu-id="9d97c-112">ratingUnitedKingdomMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdommoviestype.md)|<span data-ttu-id="9d97c-113">Оценка фильмов выбрана для Великобритании.</span><span class="sxs-lookup"><span data-stu-id="9d97c-113">Movies rating selected for United Kingdom.</span></span> <span data-ttu-id="9d97c-114">Возможные значения: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="9d97c-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span></span>|
|<span data-ttu-id="9d97c-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="9d97c-115">tvRating</span></span>|[<span data-ttu-id="9d97c-116">ратингунитедкингдомтелевисионтипе</span><span class="sxs-lookup"><span data-stu-id="9d97c-116">ratingUnitedKingdomTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdomtelevisiontype.md)|<span data-ttu-id="9d97c-117">Рейтинг для телевизора выбран для Великобритании.</span><span class="sxs-lookup"><span data-stu-id="9d97c-117">TV rating selected for United Kingdom.</span></span> <span data-ttu-id="9d97c-118">Возможные значения: `allAllowed`, `allBlocked`, `caution`.</span><span class="sxs-lookup"><span data-stu-id="9d97c-118">Possible values are: `allAllowed`, `allBlocked`, `caution`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9d97c-119">Связи</span><span class="sxs-lookup"><span data-stu-id="9d97c-119">Relationships</span></span>
<span data-ttu-id="9d97c-120">Нет</span><span class="sxs-lookup"><span data-stu-id="9d97c-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9d97c-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9d97c-121">JSON Representation</span></span>
<span data-ttu-id="9d97c-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9d97c-122">Here is a JSON representation of the resource.</span></span>
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







