---
title: Тип ресурса mediaContentRatingUnitedKingdom
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5dc8a19664e0d1b9d80451af88686be59b179780
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47993785"
---
# <a name="mediacontentratingunitedkingdom-resource-type"></a><span data-ttu-id="b8829-103">Тип ресурса mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="b8829-103">mediaContentRatingUnitedKingdom resource type</span></span>

<span data-ttu-id="b8829-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b8829-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b8829-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b8829-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b8829-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b8829-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b8829-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="b8829-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="b8829-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="b8829-108">Properties</span></span>
|<span data-ttu-id="b8829-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="b8829-109">Property</span></span>|<span data-ttu-id="b8829-110">Тип</span><span class="sxs-lookup"><span data-stu-id="b8829-110">Type</span></span>|<span data-ttu-id="b8829-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b8829-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8829-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="b8829-112">movieRating</span></span>|[<span data-ttu-id="b8829-113">ратингунитедкингдоммовиестипе</span><span class="sxs-lookup"><span data-stu-id="b8829-113">ratingUnitedKingdomMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdommoviestype.md)|<span data-ttu-id="b8829-114">Оценка фильмов выбрана для Великобритании.</span><span class="sxs-lookup"><span data-stu-id="b8829-114">Movies rating selected for United Kingdom.</span></span> <span data-ttu-id="b8829-115">Возможные значения: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="b8829-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span></span>|
|<span data-ttu-id="b8829-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="b8829-116">tvRating</span></span>|[<span data-ttu-id="b8829-117">ратингунитедкингдомтелевисионтипе</span><span class="sxs-lookup"><span data-stu-id="b8829-117">ratingUnitedKingdomTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdomtelevisiontype.md)|<span data-ttu-id="b8829-118">Рейтинг для телевизора выбран для Великобритании.</span><span class="sxs-lookup"><span data-stu-id="b8829-118">TV rating selected for United Kingdom.</span></span> <span data-ttu-id="b8829-119">Возможные значения: `allAllowed`, `allBlocked`, `caution`.</span><span class="sxs-lookup"><span data-stu-id="b8829-119">Possible values are: `allAllowed`, `allBlocked`, `caution`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b8829-120">Связи</span><span class="sxs-lookup"><span data-stu-id="b8829-120">Relationships</span></span>
<span data-ttu-id="b8829-121">Нет</span><span class="sxs-lookup"><span data-stu-id="b8829-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b8829-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b8829-122">JSON Representation</span></span>
<span data-ttu-id="b8829-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b8829-123">Here is a JSON representation of the resource.</span></span>
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






