---
title: Тип ресурса mediaContentRatingAustralia
description: Н/Д
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 259860387e005f7fe5bfd2d402be5c03ef21149f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396639"
---
# <a name="mediacontentratingaustralia-resource-type"></a><span data-ttu-id="37edf-103">Тип ресурса mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="37edf-103">mediaContentRatingAustralia resource type</span></span>

> <span data-ttu-id="37edf-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="37edf-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="37edf-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="37edf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="37edf-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="37edf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="37edf-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="37edf-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="37edf-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="37edf-108">Properties</span></span>
|<span data-ttu-id="37edf-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="37edf-109">Property</span></span>|<span data-ttu-id="37edf-110">Тип</span><span class="sxs-lookup"><span data-stu-id="37edf-110">Type</span></span>|<span data-ttu-id="37edf-111">Описание</span><span class="sxs-lookup"><span data-stu-id="37edf-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37edf-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="37edf-112">movieRating</span></span>|[<span data-ttu-id="37edf-113">ratingAustraliaMoviesType</span><span class="sxs-lookup"><span data-stu-id="37edf-113">ratingAustraliaMoviesType</span></span>](../resources/intune-deviceconfig-ratingaustraliamoviestype.md)|<span data-ttu-id="37edf-114">Оценка выбранных для Австралии фильмы.</span><span class="sxs-lookup"><span data-stu-id="37edf-114">Movies rating selected for Australia.</span></span> <span data-ttu-id="37edf-115">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="37edf-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="37edf-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="37edf-116">tvRating</span></span>|[<span data-ttu-id="37edf-117">ratingAustraliaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="37edf-117">ratingAustraliaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingaustraliatelevisiontype.md)|<span data-ttu-id="37edf-118">Оценка TV, выбранной для Австралии.</span><span class="sxs-lookup"><span data-stu-id="37edf-118">TV rating selected for Australia.</span></span> <span data-ttu-id="37edf-119">Возможные значения: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span><span class="sxs-lookup"><span data-stu-id="37edf-119">Possible values are: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="37edf-120">Отношения</span><span class="sxs-lookup"><span data-stu-id="37edf-120">Relationships</span></span>
<span data-ttu-id="37edf-121">Нет</span><span class="sxs-lookup"><span data-stu-id="37edf-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="37edf-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="37edf-122">JSON Representation</span></span>
<span data-ttu-id="37edf-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="37edf-123">Here is a JSON representation of the resource.</span></span>
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




