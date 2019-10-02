---
title: Тип ресурса mediaContentRatingCanada
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 84f54697d5c6a05f03c28b70e7d6250fa5dd0e46
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37360022"
---
# <a name="mediacontentratingcanada-resource-type"></a><span data-ttu-id="ababf-103">Тип ресурса mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="ababf-103">mediaContentRatingCanada resource type</span></span>

> <span data-ttu-id="ababf-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ababf-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ababf-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="ababf-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="ababf-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="ababf-106">Properties</span></span>
|<span data-ttu-id="ababf-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="ababf-107">Property</span></span>|<span data-ttu-id="ababf-108">Тип</span><span class="sxs-lookup"><span data-stu-id="ababf-108">Type</span></span>|<span data-ttu-id="ababf-109">Описание</span><span class="sxs-lookup"><span data-stu-id="ababf-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ababf-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="ababf-110">movieRating</span></span>|[<span data-ttu-id="ababf-111">ратингканадамовиестипе</span><span class="sxs-lookup"><span data-stu-id="ababf-111">ratingCanadaMoviesType</span></span>](../resources/intune-deviceconfig-ratingcanadamoviestype.md)|<span data-ttu-id="ababf-112">Оценка фильмов выбрана для Канады.</span><span class="sxs-lookup"><span data-stu-id="ababf-112">Movies rating selected for Canada.</span></span> <span data-ttu-id="ababf-113">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span><span class="sxs-lookup"><span data-stu-id="ababf-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span></span>|
|<span data-ttu-id="ababf-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="ababf-114">tvRating</span></span>|[<span data-ttu-id="ababf-115">ратингканадателевисионтипе</span><span class="sxs-lookup"><span data-stu-id="ababf-115">ratingCanadaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingcanadatelevisiontype.md)|<span data-ttu-id="ababf-116">Рейтинг для телевизора выбран для Канады.</span><span class="sxs-lookup"><span data-stu-id="ababf-116">TV rating selected for Canada.</span></span> <span data-ttu-id="ababf-117">Возможные значения: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="ababf-117">Possible values are: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ababf-118">Связи</span><span class="sxs-lookup"><span data-stu-id="ababf-118">Relationships</span></span>
<span data-ttu-id="ababf-119">Нет</span><span class="sxs-lookup"><span data-stu-id="ababf-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ababf-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ababf-120">JSON Representation</span></span>
<span data-ttu-id="ababf-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ababf-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingCanada"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingCanada",
  "movieRating": "String",
  "tvRating": "String"
}
```




