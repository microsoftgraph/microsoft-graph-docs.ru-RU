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
# <a name="mediacontentratingaustralia-resource-type"></a><span data-ttu-id="9a112-103">Тип ресурса mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="9a112-103">mediaContentRatingAustralia resource type</span></span>

<span data-ttu-id="9a112-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9a112-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9a112-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9a112-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9a112-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="9a112-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="9a112-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="9a112-107">Properties</span></span>
|<span data-ttu-id="9a112-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="9a112-108">Property</span></span>|<span data-ttu-id="9a112-109">Тип</span><span class="sxs-lookup"><span data-stu-id="9a112-109">Type</span></span>|<span data-ttu-id="9a112-110">Описание</span><span class="sxs-lookup"><span data-stu-id="9a112-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9a112-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="9a112-111">movieRating</span></span>|[<span data-ttu-id="9a112-112">ратингаустралиамовиестипе</span><span class="sxs-lookup"><span data-stu-id="9a112-112">ratingAustraliaMoviesType</span></span>](../resources/intune-deviceconfig-ratingaustraliamoviestype.md)|<span data-ttu-id="9a112-113">Оценка фильмов выбрана для Австралии.</span><span class="sxs-lookup"><span data-stu-id="9a112-113">Movies rating selected for Australia.</span></span> <span data-ttu-id="9a112-114">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="9a112-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="9a112-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="9a112-115">tvRating</span></span>|[<span data-ttu-id="9a112-116">ратингаустралиателевисионтипе</span><span class="sxs-lookup"><span data-stu-id="9a112-116">ratingAustraliaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingaustraliatelevisiontype.md)|<span data-ttu-id="9a112-117">Рейтинг для телевизора выбран для Австралии.</span><span class="sxs-lookup"><span data-stu-id="9a112-117">TV rating selected for Australia.</span></span> <span data-ttu-id="9a112-118">Возможные значения: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span><span class="sxs-lookup"><span data-stu-id="9a112-118">Possible values are: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9a112-119">Связи</span><span class="sxs-lookup"><span data-stu-id="9a112-119">Relationships</span></span>
<span data-ttu-id="9a112-120">Нет</span><span class="sxs-lookup"><span data-stu-id="9a112-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9a112-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9a112-121">JSON Representation</span></span>
<span data-ttu-id="9a112-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9a112-122">Here is a JSON representation of the resource.</span></span>
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







