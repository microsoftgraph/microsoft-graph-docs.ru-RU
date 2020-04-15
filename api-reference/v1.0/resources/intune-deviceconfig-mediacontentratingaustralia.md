---
title: Тип ресурса mediaContentRatingAustralia
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b25b309e011645c376a23c08b8673a7579ae69ad
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43410136"
---
# <a name="mediacontentratingaustralia-resource-type"></a><span data-ttu-id="c5b72-103">Тип ресурса mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="c5b72-103">mediaContentRatingAustralia resource type</span></span>

<span data-ttu-id="c5b72-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c5b72-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c5b72-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c5b72-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5b72-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="c5b72-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="c5b72-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="c5b72-107">Properties</span></span>
|<span data-ttu-id="c5b72-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="c5b72-108">Property</span></span>|<span data-ttu-id="c5b72-109">Тип</span><span class="sxs-lookup"><span data-stu-id="c5b72-109">Type</span></span>|<span data-ttu-id="c5b72-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c5b72-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5b72-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="c5b72-111">movieRating</span></span>|[<span data-ttu-id="c5b72-112">ратингаустралиамовиестипе</span><span class="sxs-lookup"><span data-stu-id="c5b72-112">ratingAustraliaMoviesType</span></span>](../resources/intune-deviceconfig-ratingaustraliamoviestype.md)|<span data-ttu-id="c5b72-113">Оценка фильмов выбрана для Австралии.</span><span class="sxs-lookup"><span data-stu-id="c5b72-113">Movies rating selected for Australia.</span></span> <span data-ttu-id="c5b72-114">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="c5b72-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="c5b72-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="c5b72-115">tvRating</span></span>|[<span data-ttu-id="c5b72-116">ратингаустралиателевисионтипе</span><span class="sxs-lookup"><span data-stu-id="c5b72-116">ratingAustraliaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingaustraliatelevisiontype.md)|<span data-ttu-id="c5b72-117">Рейтинг для телевизора выбран для Австралии.</span><span class="sxs-lookup"><span data-stu-id="c5b72-117">TV rating selected for Australia.</span></span> <span data-ttu-id="c5b72-118">Возможные значения: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span><span class="sxs-lookup"><span data-stu-id="c5b72-118">Possible values are: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c5b72-119">Отношения</span><span class="sxs-lookup"><span data-stu-id="c5b72-119">Relationships</span></span>
<span data-ttu-id="c5b72-120">Нет</span><span class="sxs-lookup"><span data-stu-id="c5b72-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c5b72-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c5b72-121">JSON Representation</span></span>
<span data-ttu-id="c5b72-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c5b72-122">Here is a JSON representation of the resource.</span></span>
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







