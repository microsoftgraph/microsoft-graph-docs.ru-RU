---
title: Тип ресурса mediaContentRatingCanada
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9b4151b810fcfbc56c652492fff9fa1f3f841189
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27932184"
---
# <a name="mediacontentratingcanada-resource-type"></a><span data-ttu-id="98b69-103">Тип ресурса mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="98b69-103">mediaContentRatingCanada resource type</span></span>

> <span data-ttu-id="98b69-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="98b69-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="98b69-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="98b69-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="98b69-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="98b69-106">Properties</span></span>
|<span data-ttu-id="98b69-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="98b69-107">Property</span></span>|<span data-ttu-id="98b69-108">Тип</span><span class="sxs-lookup"><span data-stu-id="98b69-108">Type</span></span>|<span data-ttu-id="98b69-109">Описание</span><span class="sxs-lookup"><span data-stu-id="98b69-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98b69-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="98b69-110">movieRating</span></span>|[<span data-ttu-id="98b69-111">ratingCanadaMoviesType</span><span class="sxs-lookup"><span data-stu-id="98b69-111">ratingCanadaMoviesType</span></span>](../resources/intune-deviceconfig-ratingcanadamoviestype.md)|<span data-ttu-id="98b69-112">Оценка выбранных для Канады фильмы.</span><span class="sxs-lookup"><span data-stu-id="98b69-112">Movies rating selected for Canada.</span></span> <span data-ttu-id="98b69-113">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span><span class="sxs-lookup"><span data-stu-id="98b69-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span></span>|
|<span data-ttu-id="98b69-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="98b69-114">tvRating</span></span>|[<span data-ttu-id="98b69-115">ratingCanadaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="98b69-115">ratingCanadaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingcanadatelevisiontype.md)|<span data-ttu-id="98b69-116">Оценка TV, выбранной для Канады.</span><span class="sxs-lookup"><span data-stu-id="98b69-116">TV rating selected for Canada.</span></span> <span data-ttu-id="98b69-117">Возможные значения: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="98b69-117">Possible values are: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="98b69-118">Связи</span><span class="sxs-lookup"><span data-stu-id="98b69-118">Relationships</span></span>
<span data-ttu-id="98b69-119">Нет</span><span class="sxs-lookup"><span data-stu-id="98b69-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="98b69-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="98b69-120">JSON Representation</span></span>
<span data-ttu-id="98b69-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="98b69-121">Here is a JSON representation of the resource.</span></span>
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



