---
title: Тип ресурса mediaContentRatingGermany
description: Н/Д
author: tfitzmac
ms.openlocfilehash: b7e02226ccea817a609d6e7f3059bff8e6bdb9ce
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27318363"
---
# <a name="mediacontentratinggermany-resource-type"></a><span data-ttu-id="37d0e-103">Тип ресурса mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="37d0e-103">mediaContentRatingGermany resource type</span></span>

> <span data-ttu-id="37d0e-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="37d0e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="37d0e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="37d0e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="37d0e-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="37d0e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="37d0e-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="37d0e-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="37d0e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="37d0e-108">Properties</span></span>
|<span data-ttu-id="37d0e-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="37d0e-109">Property</span></span>|<span data-ttu-id="37d0e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="37d0e-110">Type</span></span>|<span data-ttu-id="37d0e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="37d0e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37d0e-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="37d0e-112">movieRating</span></span>|[<span data-ttu-id="37d0e-113">ratingGermanyMoviesType</span><span class="sxs-lookup"><span data-stu-id="37d0e-113">ratingGermanyMoviesType</span></span>](../resources/intune-deviceconfig-ratinggermanymoviestype.md)|<span data-ttu-id="37d0e-114">Оценка выбранных для Германии фильмы.</span><span class="sxs-lookup"><span data-stu-id="37d0e-114">Movies rating selected for Germany.</span></span> <span data-ttu-id="37d0e-115">Возможные значения: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="37d0e-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="37d0e-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="37d0e-116">tvRating</span></span>|[<span data-ttu-id="37d0e-117">ratingGermanyTelevisionType</span><span class="sxs-lookup"><span data-stu-id="37d0e-117">ratingGermanyTelevisionType</span></span>](../resources/intune-deviceconfig-ratinggermanytelevisiontype.md)|<span data-ttu-id="37d0e-118">Оценка TV, выбранной для Германии.</span><span class="sxs-lookup"><span data-stu-id="37d0e-118">TV rating selected for Germany.</span></span> <span data-ttu-id="37d0e-119">Возможные значения: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="37d0e-119">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="37d0e-120">Связи</span><span class="sxs-lookup"><span data-stu-id="37d0e-120">Relationships</span></span>
<span data-ttu-id="37d0e-121">Нет</span><span class="sxs-lookup"><span data-stu-id="37d0e-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="37d0e-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="37d0e-122">JSON Representation</span></span>
<span data-ttu-id="37d0e-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="37d0e-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingGermany"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingGermany",
  "movieRating": "String",
  "tvRating": "String"
}
```





