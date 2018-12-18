---
title: Тип ресурса mediaContentRatingUnitedStates
description: Н/Д
author: tfitzmac
ms.openlocfilehash: ee10df5dd5e3f915e166cb77e747f8b3f7cc2d37
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27341323"
---
# <a name="mediacontentratingunitedstates-resource-type"></a><span data-ttu-id="bed1f-103">Тип ресурса mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="bed1f-103">mediaContentRatingUnitedStates resource type</span></span>

> <span data-ttu-id="bed1f-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="bed1f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bed1f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bed1f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bed1f-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="bed1f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bed1f-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="bed1f-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="bed1f-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="bed1f-108">Properties</span></span>
|<span data-ttu-id="bed1f-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="bed1f-109">Property</span></span>|<span data-ttu-id="bed1f-110">Тип</span><span class="sxs-lookup"><span data-stu-id="bed1f-110">Type</span></span>|<span data-ttu-id="bed1f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="bed1f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bed1f-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="bed1f-112">movieRating</span></span>|[<span data-ttu-id="bed1f-113">ratingUnitedStatesMoviesType</span><span class="sxs-lookup"><span data-stu-id="bed1f-113">ratingUnitedStatesMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedstatesmoviestype.md)|<span data-ttu-id="bed1f-114">Фильмы рейтинг выбранных для США.</span><span class="sxs-lookup"><span data-stu-id="bed1f-114">Movies rating selected for United States.</span></span> <span data-ttu-id="bed1f-115">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="bed1f-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span></span>|
|<span data-ttu-id="bed1f-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="bed1f-116">tvRating</span></span>|[<span data-ttu-id="bed1f-117">ratingUnitedStatesTelevisionType</span><span class="sxs-lookup"><span data-stu-id="bed1f-117">ratingUnitedStatesTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedstatestelevisiontype.md)|<span data-ttu-id="bed1f-118">Оценка TV, выбранной для США.</span><span class="sxs-lookup"><span data-stu-id="bed1f-118">TV rating selected for United States.</span></span> <span data-ttu-id="bed1f-119">Возможные значения: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="bed1f-119">Possible values are: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bed1f-120">Связи</span><span class="sxs-lookup"><span data-stu-id="bed1f-120">Relationships</span></span>
<span data-ttu-id="bed1f-121">Нет</span><span class="sxs-lookup"><span data-stu-id="bed1f-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="bed1f-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bed1f-122">JSON Representation</span></span>
<span data-ttu-id="bed1f-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bed1f-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingUnitedStates"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingUnitedStates",
  "movieRating": "String",
  "tvRating": "String"
}
```





