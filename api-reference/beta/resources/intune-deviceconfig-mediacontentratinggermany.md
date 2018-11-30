---
title: Тип ресурса mediaContentRatingGermany
description: Н/Д
ms.openlocfilehash: 821a648f839e531c2efaa3da4b4b1aead65c9673
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078267"
---
# <a name="mediacontentratinggermany-resource-type"></a><span data-ttu-id="95192-103">Тип ресурса mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="95192-103">mediaContentRatingGermany resource type</span></span>

> <span data-ttu-id="95192-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="95192-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="95192-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="95192-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="95192-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="95192-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="95192-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="95192-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="95192-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="95192-108">Properties</span></span>
|<span data-ttu-id="95192-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="95192-109">Property</span></span>|<span data-ttu-id="95192-110">Тип</span><span class="sxs-lookup"><span data-stu-id="95192-110">Type</span></span>|<span data-ttu-id="95192-111">Описание</span><span class="sxs-lookup"><span data-stu-id="95192-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95192-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="95192-112">movieRating</span></span>|[<span data-ttu-id="95192-113">ratingGermanyMoviesType</span><span class="sxs-lookup"><span data-stu-id="95192-113">ratingGermanyMoviesType</span></span>](../resources/intune-deviceconfig-ratinggermanymoviestype.md)|<span data-ttu-id="95192-114">Оценка выбранных для Германии фильмы.</span><span class="sxs-lookup"><span data-stu-id="95192-114">Movies rating selected for Germany.</span></span> <span data-ttu-id="95192-115">Возможные значения: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="95192-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="95192-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="95192-116">tvRating</span></span>|[<span data-ttu-id="95192-117">ratingGermanyTelevisionType</span><span class="sxs-lookup"><span data-stu-id="95192-117">ratingGermanyTelevisionType</span></span>](../resources/intune-deviceconfig-ratinggermanytelevisiontype.md)|<span data-ttu-id="95192-118">Оценка TV, выбранной для Германии.</span><span class="sxs-lookup"><span data-stu-id="95192-118">TV rating selected for Germany.</span></span> <span data-ttu-id="95192-119">Возможные значения: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="95192-119">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="95192-120">Связи</span><span class="sxs-lookup"><span data-stu-id="95192-120">Relationships</span></span>
<span data-ttu-id="95192-121">Нет</span><span class="sxs-lookup"><span data-stu-id="95192-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="95192-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="95192-122">JSON Representation</span></span>
<span data-ttu-id="95192-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="95192-123">Here is a JSON representation of the resource.</span></span>
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





