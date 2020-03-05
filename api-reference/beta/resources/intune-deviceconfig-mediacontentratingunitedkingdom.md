---
title: Тип ресурса mediaContentRatingUnitedKingdom
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 485213d59e42793301acfe637554c08d9325b7ad
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526022"
---
# <a name="mediacontentratingunitedkingdom-resource-type"></a><span data-ttu-id="ddd15-103">Тип ресурса mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="ddd15-103">mediaContentRatingUnitedKingdom resource type</span></span>

<span data-ttu-id="ddd15-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ddd15-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ddd15-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ddd15-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ddd15-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ddd15-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ddd15-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="ddd15-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="ddd15-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="ddd15-108">Properties</span></span>
|<span data-ttu-id="ddd15-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="ddd15-109">Property</span></span>|<span data-ttu-id="ddd15-110">Тип</span><span class="sxs-lookup"><span data-stu-id="ddd15-110">Type</span></span>|<span data-ttu-id="ddd15-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ddd15-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ddd15-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="ddd15-112">movieRating</span></span>|[<span data-ttu-id="ddd15-113">ратингунитедкингдоммовиестипе</span><span class="sxs-lookup"><span data-stu-id="ddd15-113">ratingUnitedKingdomMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdommoviestype.md)|<span data-ttu-id="ddd15-114">Оценка фильмов выбрана для Великобритании.</span><span class="sxs-lookup"><span data-stu-id="ddd15-114">Movies rating selected for United Kingdom.</span></span> <span data-ttu-id="ddd15-115">Возможные значения: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="ddd15-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span></span>|
|<span data-ttu-id="ddd15-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="ddd15-116">tvRating</span></span>|[<span data-ttu-id="ddd15-117">ратингунитедкингдомтелевисионтипе</span><span class="sxs-lookup"><span data-stu-id="ddd15-117">ratingUnitedKingdomTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdomtelevisiontype.md)|<span data-ttu-id="ddd15-118">Рейтинг для телевизора выбран для Великобритании.</span><span class="sxs-lookup"><span data-stu-id="ddd15-118">TV rating selected for United Kingdom.</span></span> <span data-ttu-id="ddd15-119">Возможные значения: `allAllowed`, `allBlocked`, `caution`.</span><span class="sxs-lookup"><span data-stu-id="ddd15-119">Possible values are: `allAllowed`, `allBlocked`, `caution`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ddd15-120">Связи</span><span class="sxs-lookup"><span data-stu-id="ddd15-120">Relationships</span></span>
<span data-ttu-id="ddd15-121">Нет</span><span class="sxs-lookup"><span data-stu-id="ddd15-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ddd15-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ddd15-122">JSON Representation</span></span>
<span data-ttu-id="ddd15-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ddd15-123">Here is a JSON representation of the resource.</span></span>
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



