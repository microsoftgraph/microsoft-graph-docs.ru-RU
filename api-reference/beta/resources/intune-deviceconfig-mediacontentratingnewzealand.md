---
title: Тип ресурса mediaContentRatingNewZealand
description: Н/Д
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: adfc34cf65104f0bf370a4e1ba22cfcb78bf250b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403450"
---
# <a name="mediacontentratingnewzealand-resource-type"></a><span data-ttu-id="78a45-103">Тип ресурса mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="78a45-103">mediaContentRatingNewZealand resource type</span></span>

> <span data-ttu-id="78a45-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="78a45-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="78a45-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="78a45-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="78a45-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="78a45-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="78a45-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="78a45-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="78a45-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="78a45-108">Properties</span></span>
|<span data-ttu-id="78a45-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="78a45-109">Property</span></span>|<span data-ttu-id="78a45-110">Тип</span><span class="sxs-lookup"><span data-stu-id="78a45-110">Type</span></span>|<span data-ttu-id="78a45-111">Описание</span><span class="sxs-lookup"><span data-stu-id="78a45-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="78a45-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="78a45-112">movieRating</span></span>|[<span data-ttu-id="78a45-113">ratingNewZealandMoviesType</span><span class="sxs-lookup"><span data-stu-id="78a45-113">ratingNewZealandMoviesType</span></span>](../resources/intune-deviceconfig-ratingnewzealandmoviestype.md)|<span data-ttu-id="78a45-114">Оценка выбранных для новой Зеландии фильмы.</span><span class="sxs-lookup"><span data-stu-id="78a45-114">Movies rating selected for New Zealand.</span></span> <span data-ttu-id="78a45-115">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span><span class="sxs-lookup"><span data-stu-id="78a45-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span></span>|
|<span data-ttu-id="78a45-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="78a45-116">tvRating</span></span>|[<span data-ttu-id="78a45-117">ratingNewZealandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="78a45-117">ratingNewZealandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingnewzealandtelevisiontype.md)|<span data-ttu-id="78a45-118">Оценка TV, выбранной для новой Зеландии.</span><span class="sxs-lookup"><span data-stu-id="78a45-118">TV rating selected for New Zealand.</span></span> <span data-ttu-id="78a45-119">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="78a45-119">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="78a45-120">Отношения</span><span class="sxs-lookup"><span data-stu-id="78a45-120">Relationships</span></span>
<span data-ttu-id="78a45-121">Нет</span><span class="sxs-lookup"><span data-stu-id="78a45-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="78a45-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="78a45-122">JSON Representation</span></span>
<span data-ttu-id="78a45-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="78a45-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingNewZealand"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingNewZealand",
  "movieRating": "String",
  "tvRating": "String"
}
```




