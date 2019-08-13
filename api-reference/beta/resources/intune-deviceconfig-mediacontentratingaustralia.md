---
title: Тип ресурса mediaContentRatingAustralia
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f2d3c6808b6fa350ea1ca5965eb7c123c0e70287
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36368795"
---
# <a name="mediacontentratingaustralia-resource-type"></a><span data-ttu-id="43782-103">Тип ресурса mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="43782-103">mediaContentRatingAustralia resource type</span></span>

> <span data-ttu-id="43782-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="43782-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="43782-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="43782-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="43782-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="43782-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="43782-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="43782-107">Properties</span></span>
|<span data-ttu-id="43782-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="43782-108">Property</span></span>|<span data-ttu-id="43782-109">Тип</span><span class="sxs-lookup"><span data-stu-id="43782-109">Type</span></span>|<span data-ttu-id="43782-110">Описание</span><span class="sxs-lookup"><span data-stu-id="43782-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43782-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="43782-111">movieRating</span></span>|[<span data-ttu-id="43782-112">ратингаустралиамовиестипе</span><span class="sxs-lookup"><span data-stu-id="43782-112">ratingAustraliaMoviesType</span></span>](../resources/intune-deviceconfig-ratingaustraliamoviestype.md)|<span data-ttu-id="43782-113">Оценка фильмов выбрана для Австралии.</span><span class="sxs-lookup"><span data-stu-id="43782-113">Movies rating selected for Australia.</span></span> <span data-ttu-id="43782-114">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="43782-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="43782-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="43782-115">tvRating</span></span>|[<span data-ttu-id="43782-116">ратингаустралиателевисионтипе</span><span class="sxs-lookup"><span data-stu-id="43782-116">ratingAustraliaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingaustraliatelevisiontype.md)|<span data-ttu-id="43782-117">Рейтинг для телевизора выбран для Австралии.</span><span class="sxs-lookup"><span data-stu-id="43782-117">TV rating selected for Australia.</span></span> <span data-ttu-id="43782-118">Возможные значения: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span><span class="sxs-lookup"><span data-stu-id="43782-118">Possible values are: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="43782-119">Отношения</span><span class="sxs-lookup"><span data-stu-id="43782-119">Relationships</span></span>
<span data-ttu-id="43782-120">Нет</span><span class="sxs-lookup"><span data-stu-id="43782-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="43782-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="43782-121">JSON Representation</span></span>
<span data-ttu-id="43782-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="43782-122">Here is a JSON representation of the resource.</span></span>
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



