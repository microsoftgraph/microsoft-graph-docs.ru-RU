---
title: Тип ресурса mediaContentRatingCanada
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 38f3bac4e8410a3c63bd07319888ab0a5fc7df19
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30146349"
---
# <a name="mediacontentratingcanada-resource-type"></a><span data-ttu-id="6bd1f-103">Тип ресурса mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="6bd1f-103">mediaContentRatingCanada resource type</span></span>

> <span data-ttu-id="6bd1f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6bd1f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6bd1f-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6bd1f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6bd1f-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="6bd1f-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="6bd1f-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="6bd1f-107">Properties</span></span>
|<span data-ttu-id="6bd1f-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="6bd1f-108">Property</span></span>|<span data-ttu-id="6bd1f-109">Тип</span><span class="sxs-lookup"><span data-stu-id="6bd1f-109">Type</span></span>|<span data-ttu-id="6bd1f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6bd1f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6bd1f-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="6bd1f-111">movieRating</span></span>|[<span data-ttu-id="6bd1f-112">Ратингканадамовиестипе</span><span class="sxs-lookup"><span data-stu-id="6bd1f-112">ratingCanadaMoviesType</span></span>](../resources/intune-deviceconfig-ratingcanadamoviestype.md)|<span data-ttu-id="6bd1f-113">Оценка фильмов выбрана для Канады.</span><span class="sxs-lookup"><span data-stu-id="6bd1f-113">Movies rating selected for Canada.</span></span> <span data-ttu-id="6bd1f-114">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span><span class="sxs-lookup"><span data-stu-id="6bd1f-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span></span>|
|<span data-ttu-id="6bd1f-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="6bd1f-115">tvRating</span></span>|[<span data-ttu-id="6bd1f-116">Ратингканадателевисионтипе</span><span class="sxs-lookup"><span data-stu-id="6bd1f-116">ratingCanadaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingcanadatelevisiontype.md)|<span data-ttu-id="6bd1f-117">Рейтинг для телевизора выбран для Канады.</span><span class="sxs-lookup"><span data-stu-id="6bd1f-117">TV rating selected for Canada.</span></span> <span data-ttu-id="6bd1f-118">Возможные значения: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="6bd1f-118">Possible values are: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6bd1f-119">Связи</span><span class="sxs-lookup"><span data-stu-id="6bd1f-119">Relationships</span></span>
<span data-ttu-id="6bd1f-120">Нет</span><span class="sxs-lookup"><span data-stu-id="6bd1f-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6bd1f-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6bd1f-121">JSON Representation</span></span>
<span data-ttu-id="6bd1f-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6bd1f-122">Here is a JSON representation of the resource.</span></span>
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




