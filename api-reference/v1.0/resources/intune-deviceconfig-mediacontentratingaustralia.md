---
title: Тип ресурса mediaContentRatingAustralia
description: Пока не задокументировано.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0a9e3035585794216440522233f23a8061ddafee
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031432"
---
# <a name="mediacontentratingaustralia-resource-type"></a><span data-ttu-id="5b384-103">Тип ресурса mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="5b384-103">mediaContentRatingAustralia resource type</span></span>

> <span data-ttu-id="5b384-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5b384-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5b384-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="5b384-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="5b384-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="5b384-106">Properties</span></span>
|<span data-ttu-id="5b384-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="5b384-107">Property</span></span>|<span data-ttu-id="5b384-108">Тип</span><span class="sxs-lookup"><span data-stu-id="5b384-108">Type</span></span>|<span data-ttu-id="5b384-109">Описание</span><span class="sxs-lookup"><span data-stu-id="5b384-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b384-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="5b384-110">movieRating</span></span>|[<span data-ttu-id="5b384-111">Ратингаустралиамовиестипе</span><span class="sxs-lookup"><span data-stu-id="5b384-111">ratingAustraliaMoviesType</span></span>](../resources/intune-deviceconfig-ratingaustraliamoviestype.md)|<span data-ttu-id="5b384-112">Оценка фильмов выбрана для Австралии.</span><span class="sxs-lookup"><span data-stu-id="5b384-112">Movies rating selected for Australia.</span></span> <span data-ttu-id="5b384-113">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="5b384-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="5b384-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="5b384-114">tvRating</span></span>|[<span data-ttu-id="5b384-115">Ратингаустралиателевисионтипе</span><span class="sxs-lookup"><span data-stu-id="5b384-115">ratingAustraliaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingaustraliatelevisiontype.md)|<span data-ttu-id="5b384-116">Рейтинг для телевизора выбран для Австралии.</span><span class="sxs-lookup"><span data-stu-id="5b384-116">TV rating selected for Australia.</span></span> <span data-ttu-id="5b384-117">Возможные значения: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span><span class="sxs-lookup"><span data-stu-id="5b384-117">Possible values are: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5b384-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="5b384-118">Relationships</span></span>
<span data-ttu-id="5b384-119">Нет</span><span class="sxs-lookup"><span data-stu-id="5b384-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5b384-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5b384-120">JSON Representation</span></span>
<span data-ttu-id="5b384-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5b384-121">Here is a JSON representation of the resource.</span></span>
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



