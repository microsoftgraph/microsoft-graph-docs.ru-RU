---
title: Тип ресурса mediaContentRatingAustralia
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ae1cb934af017c751ae2bcf05cd992668a452ed6
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30166768"
---
# <a name="mediacontentratingaustralia-resource-type"></a><span data-ttu-id="f3435-103">Тип ресурса mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="f3435-103">mediaContentRatingAustralia resource type</span></span>

> <span data-ttu-id="f3435-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3435-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f3435-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f3435-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3435-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="f3435-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="f3435-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="f3435-107">Properties</span></span>
|<span data-ttu-id="f3435-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="f3435-108">Property</span></span>|<span data-ttu-id="f3435-109">Тип</span><span class="sxs-lookup"><span data-stu-id="f3435-109">Type</span></span>|<span data-ttu-id="f3435-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f3435-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3435-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="f3435-111">movieRating</span></span>|[<span data-ttu-id="f3435-112">Ратингаустралиамовиестипе</span><span class="sxs-lookup"><span data-stu-id="f3435-112">ratingAustraliaMoviesType</span></span>](../resources/intune-deviceconfig-ratingaustraliamoviestype.md)|<span data-ttu-id="f3435-113">Оценка фильмов выбрана для Австралии.</span><span class="sxs-lookup"><span data-stu-id="f3435-113">Movies rating selected for Australia.</span></span> <span data-ttu-id="f3435-114">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="f3435-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="f3435-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="f3435-115">tvRating</span></span>|[<span data-ttu-id="f3435-116">Ратингаустралиателевисионтипе</span><span class="sxs-lookup"><span data-stu-id="f3435-116">ratingAustraliaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingaustraliatelevisiontype.md)|<span data-ttu-id="f3435-117">Рейтинг для телевизора выбран для Австралии.</span><span class="sxs-lookup"><span data-stu-id="f3435-117">TV rating selected for Australia.</span></span> <span data-ttu-id="f3435-118">Возможные значения: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span><span class="sxs-lookup"><span data-stu-id="f3435-118">Possible values are: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f3435-119">Отношения</span><span class="sxs-lookup"><span data-stu-id="f3435-119">Relationships</span></span>
<span data-ttu-id="f3435-120">Нет</span><span class="sxs-lookup"><span data-stu-id="f3435-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f3435-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f3435-121">JSON Representation</span></span>
<span data-ttu-id="f3435-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f3435-122">Here is a JSON representation of the resource.</span></span>
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




