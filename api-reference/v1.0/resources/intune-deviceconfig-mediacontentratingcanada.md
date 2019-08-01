---
title: Тип ресурса mediaContentRatingCanada
description: Пока не задокументировано.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9735497f3f2f71f28b8fe9847d2664bd4e65e959
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028114"
---
# <a name="mediacontentratingcanada-resource-type"></a><span data-ttu-id="b4951-103">Тип ресурса mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="b4951-103">mediaContentRatingCanada resource type</span></span>

> <span data-ttu-id="b4951-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b4951-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b4951-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="b4951-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="b4951-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="b4951-106">Properties</span></span>
|<span data-ttu-id="b4951-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="b4951-107">Property</span></span>|<span data-ttu-id="b4951-108">Тип</span><span class="sxs-lookup"><span data-stu-id="b4951-108">Type</span></span>|<span data-ttu-id="b4951-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b4951-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4951-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="b4951-110">movieRating</span></span>|[<span data-ttu-id="b4951-111">Ратингканадамовиестипе</span><span class="sxs-lookup"><span data-stu-id="b4951-111">ratingCanadaMoviesType</span></span>](../resources/intune-deviceconfig-ratingcanadamoviestype.md)|<span data-ttu-id="b4951-112">Оценка фильмов выбрана для Канады.</span><span class="sxs-lookup"><span data-stu-id="b4951-112">Movies rating selected for Canada.</span></span> <span data-ttu-id="b4951-113">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span><span class="sxs-lookup"><span data-stu-id="b4951-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span></span>|
|<span data-ttu-id="b4951-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="b4951-114">tvRating</span></span>|[<span data-ttu-id="b4951-115">Ратингканадателевисионтипе</span><span class="sxs-lookup"><span data-stu-id="b4951-115">ratingCanadaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingcanadatelevisiontype.md)|<span data-ttu-id="b4951-116">Рейтинг для телевизора выбран для Канады.</span><span class="sxs-lookup"><span data-stu-id="b4951-116">TV rating selected for Canada.</span></span> <span data-ttu-id="b4951-117">Возможные значения: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="b4951-117">Possible values are: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b4951-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="b4951-118">Relationships</span></span>
<span data-ttu-id="b4951-119">Нет</span><span class="sxs-lookup"><span data-stu-id="b4951-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b4951-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b4951-120">JSON Representation</span></span>
<span data-ttu-id="b4951-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b4951-121">Here is a JSON representation of the resource.</span></span>
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



