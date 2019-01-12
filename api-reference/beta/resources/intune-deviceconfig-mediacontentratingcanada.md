---
title: Тип ресурса mediaContentRatingCanada
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 0e6b3c84801ecf1338a04e356d9141d4b45286de
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27981002"
---
# <a name="mediacontentratingcanada-resource-type"></a><span data-ttu-id="88024-103">Тип ресурса mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="88024-103">mediaContentRatingCanada resource type</span></span>

> <span data-ttu-id="88024-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="88024-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="88024-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="88024-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="88024-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="88024-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="88024-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="88024-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="88024-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="88024-108">Properties</span></span>
|<span data-ttu-id="88024-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="88024-109">Property</span></span>|<span data-ttu-id="88024-110">Тип</span><span class="sxs-lookup"><span data-stu-id="88024-110">Type</span></span>|<span data-ttu-id="88024-111">Описание</span><span class="sxs-lookup"><span data-stu-id="88024-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88024-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="88024-112">movieRating</span></span>|[<span data-ttu-id="88024-113">ratingCanadaMoviesType</span><span class="sxs-lookup"><span data-stu-id="88024-113">ratingCanadaMoviesType</span></span>](../resources/intune-deviceconfig-ratingcanadamoviestype.md)|<span data-ttu-id="88024-114">Оценка выбранных для Канады фильмы.</span><span class="sxs-lookup"><span data-stu-id="88024-114">Movies rating selected for Canada.</span></span> <span data-ttu-id="88024-115">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span><span class="sxs-lookup"><span data-stu-id="88024-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span></span>|
|<span data-ttu-id="88024-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="88024-116">tvRating</span></span>|[<span data-ttu-id="88024-117">ratingCanadaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="88024-117">ratingCanadaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingcanadatelevisiontype.md)|<span data-ttu-id="88024-118">Оценка TV, выбранной для Канады.</span><span class="sxs-lookup"><span data-stu-id="88024-118">TV rating selected for Canada.</span></span> <span data-ttu-id="88024-119">Возможные значения: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="88024-119">Possible values are: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="88024-120">Связи</span><span class="sxs-lookup"><span data-stu-id="88024-120">Relationships</span></span>
<span data-ttu-id="88024-121">Нет</span><span class="sxs-lookup"><span data-stu-id="88024-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="88024-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="88024-122">JSON Representation</span></span>
<span data-ttu-id="88024-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="88024-123">Here is a JSON representation of the resource.</span></span>
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





