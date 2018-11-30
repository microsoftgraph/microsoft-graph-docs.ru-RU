---
title: Тип ресурса mediaContentRatingCanada
description: Н/Д
ms.openlocfilehash: 764bea688c5c7d86f675caafdc47fa42d4a7d37a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027393"
---
# <a name="mediacontentratingcanada-resource-type"></a><span data-ttu-id="86db8-103">Тип ресурса mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="86db8-103">mediaContentRatingCanada resource type</span></span>

> <span data-ttu-id="86db8-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="86db8-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="86db8-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="86db8-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="86db8-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="86db8-106">Properties</span></span>
|<span data-ttu-id="86db8-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="86db8-107">Property</span></span>|<span data-ttu-id="86db8-108">Тип</span><span class="sxs-lookup"><span data-stu-id="86db8-108">Type</span></span>|<span data-ttu-id="86db8-109">Описание</span><span class="sxs-lookup"><span data-stu-id="86db8-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86db8-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="86db8-110">movieRating</span></span>|[<span data-ttu-id="86db8-111">ratingCanadaMoviesType</span><span class="sxs-lookup"><span data-stu-id="86db8-111">ratingCanadaMoviesType</span></span>](../resources/intune-deviceconfig-ratingcanadamoviestype.md)|<span data-ttu-id="86db8-112">Оценка выбранных для Канады фильмы.</span><span class="sxs-lookup"><span data-stu-id="86db8-112">Movies rating selected for Canada.</span></span> <span data-ttu-id="86db8-113">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span><span class="sxs-lookup"><span data-stu-id="86db8-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span></span>|
|<span data-ttu-id="86db8-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="86db8-114">tvRating</span></span>|[<span data-ttu-id="86db8-115">ratingCanadaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="86db8-115">ratingCanadaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingcanadatelevisiontype.md)|<span data-ttu-id="86db8-116">Оценка TV, выбранной для Канады.</span><span class="sxs-lookup"><span data-stu-id="86db8-116">TV rating selected for Canada.</span></span> <span data-ttu-id="86db8-117">Возможные значения: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="86db8-117">Possible values are: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="86db8-118">Связи</span><span class="sxs-lookup"><span data-stu-id="86db8-118">Relationships</span></span>
<span data-ttu-id="86db8-119">Нет</span><span class="sxs-lookup"><span data-stu-id="86db8-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="86db8-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="86db8-120">JSON Representation</span></span>
<span data-ttu-id="86db8-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="86db8-121">Here is a JSON representation of the resource.</span></span>
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



