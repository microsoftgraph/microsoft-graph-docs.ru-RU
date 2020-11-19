---
title: Тип ресурса mediaContentRatingUnitedKingdom
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d9173aec94ce24056fd8d6c7efffcf144509c5ef
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49273447"
---
# <a name="mediacontentratingunitedkingdom-resource-type"></a><span data-ttu-id="252c6-103">Тип ресурса mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="252c6-103">mediaContentRatingUnitedKingdom resource type</span></span>

<span data-ttu-id="252c6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="252c6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="252c6-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="252c6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="252c6-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="252c6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="252c6-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="252c6-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="252c6-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="252c6-108">Properties</span></span>
|<span data-ttu-id="252c6-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="252c6-109">Property</span></span>|<span data-ttu-id="252c6-110">Тип</span><span class="sxs-lookup"><span data-stu-id="252c6-110">Type</span></span>|<span data-ttu-id="252c6-111">Описание</span><span class="sxs-lookup"><span data-stu-id="252c6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="252c6-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="252c6-112">movieRating</span></span>|[<span data-ttu-id="252c6-113">ратингунитедкингдоммовиестипе</span><span class="sxs-lookup"><span data-stu-id="252c6-113">ratingUnitedKingdomMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdommoviestype.md)|<span data-ttu-id="252c6-114">Оценка фильмов выбрана для Великобритании.</span><span class="sxs-lookup"><span data-stu-id="252c6-114">Movies rating selected for United Kingdom.</span></span> <span data-ttu-id="252c6-115">Возможные значения: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="252c6-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span></span>|
|<span data-ttu-id="252c6-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="252c6-116">tvRating</span></span>|[<span data-ttu-id="252c6-117">ратингунитедкингдомтелевисионтипе</span><span class="sxs-lookup"><span data-stu-id="252c6-117">ratingUnitedKingdomTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdomtelevisiontype.md)|<span data-ttu-id="252c6-118">Рейтинг для телевизора выбран для Великобритании.</span><span class="sxs-lookup"><span data-stu-id="252c6-118">TV rating selected for United Kingdom.</span></span> <span data-ttu-id="252c6-119">Возможные значения: `allAllowed`, `allBlocked`, `caution`.</span><span class="sxs-lookup"><span data-stu-id="252c6-119">Possible values are: `allAllowed`, `allBlocked`, `caution`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="252c6-120">Связи</span><span class="sxs-lookup"><span data-stu-id="252c6-120">Relationships</span></span>
<span data-ttu-id="252c6-121">Нет</span><span class="sxs-lookup"><span data-stu-id="252c6-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="252c6-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="252c6-122">JSON Representation</span></span>
<span data-ttu-id="252c6-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="252c6-123">Here is a JSON representation of the resource.</span></span>
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




