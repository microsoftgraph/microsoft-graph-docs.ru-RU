---
title: Тип ресурса mediaContentRatingAustralia
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 38a72d9fdc77eea40b02c43464c7e8934885831e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48003201"
---
# <a name="mediacontentratingaustralia-resource-type"></a><span data-ttu-id="9995a-103">Тип ресурса mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="9995a-103">mediaContentRatingAustralia resource type</span></span>

<span data-ttu-id="9995a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9995a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9995a-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9995a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9995a-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="9995a-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="9995a-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="9995a-107">Properties</span></span>
|<span data-ttu-id="9995a-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="9995a-108">Property</span></span>|<span data-ttu-id="9995a-109">Тип</span><span class="sxs-lookup"><span data-stu-id="9995a-109">Type</span></span>|<span data-ttu-id="9995a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="9995a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9995a-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="9995a-111">movieRating</span></span>|[<span data-ttu-id="9995a-112">ратингаустралиамовиестипе</span><span class="sxs-lookup"><span data-stu-id="9995a-112">ratingAustraliaMoviesType</span></span>](../resources/intune-deviceconfig-ratingaustraliamoviestype.md)|<span data-ttu-id="9995a-113">Оценка фильмов выбрана для Австралии.</span><span class="sxs-lookup"><span data-stu-id="9995a-113">Movies rating selected for Australia.</span></span> <span data-ttu-id="9995a-114">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="9995a-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="9995a-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="9995a-115">tvRating</span></span>|[<span data-ttu-id="9995a-116">ратингаустралиателевисионтипе</span><span class="sxs-lookup"><span data-stu-id="9995a-116">ratingAustraliaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingaustraliatelevisiontype.md)|<span data-ttu-id="9995a-117">Рейтинг для телевизора выбран для Австралии.</span><span class="sxs-lookup"><span data-stu-id="9995a-117">TV rating selected for Australia.</span></span> <span data-ttu-id="9995a-118">Возможные значения: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span><span class="sxs-lookup"><span data-stu-id="9995a-118">Possible values are: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9995a-119">Связи</span><span class="sxs-lookup"><span data-stu-id="9995a-119">Relationships</span></span>
<span data-ttu-id="9995a-120">Нет</span><span class="sxs-lookup"><span data-stu-id="9995a-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9995a-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9995a-121">JSON Representation</span></span>
<span data-ttu-id="9995a-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9995a-122">Here is a JSON representation of the resource.</span></span>
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









