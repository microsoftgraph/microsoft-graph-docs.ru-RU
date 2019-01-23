---
title: Тип ресурса mediaContentRatingCanada
description: Н/Д
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 292dc926a626a2aca96312133eb6c9a850db39af
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398053"
---
# <a name="mediacontentratingcanada-resource-type"></a><span data-ttu-id="44b65-103">Тип ресурса mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="44b65-103">mediaContentRatingCanada resource type</span></span>

> <span data-ttu-id="44b65-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="44b65-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="44b65-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44b65-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="44b65-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="44b65-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="44b65-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="44b65-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="44b65-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="44b65-108">Properties</span></span>
|<span data-ttu-id="44b65-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="44b65-109">Property</span></span>|<span data-ttu-id="44b65-110">Тип</span><span class="sxs-lookup"><span data-stu-id="44b65-110">Type</span></span>|<span data-ttu-id="44b65-111">Описание</span><span class="sxs-lookup"><span data-stu-id="44b65-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44b65-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="44b65-112">movieRating</span></span>|[<span data-ttu-id="44b65-113">ratingCanadaMoviesType</span><span class="sxs-lookup"><span data-stu-id="44b65-113">ratingCanadaMoviesType</span></span>](../resources/intune-deviceconfig-ratingcanadamoviestype.md)|<span data-ttu-id="44b65-114">Оценка выбранных для Канады фильмы.</span><span class="sxs-lookup"><span data-stu-id="44b65-114">Movies rating selected for Canada.</span></span> <span data-ttu-id="44b65-115">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span><span class="sxs-lookup"><span data-stu-id="44b65-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span></span>|
|<span data-ttu-id="44b65-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="44b65-116">tvRating</span></span>|[<span data-ttu-id="44b65-117">ratingCanadaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="44b65-117">ratingCanadaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingcanadatelevisiontype.md)|<span data-ttu-id="44b65-118">Оценка TV, выбранной для Канады.</span><span class="sxs-lookup"><span data-stu-id="44b65-118">TV rating selected for Canada.</span></span> <span data-ttu-id="44b65-119">Возможные значения: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="44b65-119">Possible values are: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="44b65-120">Связи</span><span class="sxs-lookup"><span data-stu-id="44b65-120">Relationships</span></span>
<span data-ttu-id="44b65-121">Нет</span><span class="sxs-lookup"><span data-stu-id="44b65-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="44b65-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="44b65-122">JSON Representation</span></span>
<span data-ttu-id="44b65-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="44b65-123">Here is a JSON representation of the resource.</span></span>
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




