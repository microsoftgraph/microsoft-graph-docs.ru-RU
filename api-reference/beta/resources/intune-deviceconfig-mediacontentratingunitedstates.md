---
title: Тип ресурса mediaContentRatingUnitedStates
description: Н/Д
ms.openlocfilehash: d62d656c4fbd8744560ab191786d71b732fe6c21
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074979"
---
# <a name="mediacontentratingunitedstates-resource-type"></a><span data-ttu-id="820fc-103">Тип ресурса mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="820fc-103">mediaContentRatingUnitedStates resource type</span></span>

> <span data-ttu-id="820fc-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="820fc-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="820fc-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="820fc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="820fc-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="820fc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="820fc-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="820fc-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="820fc-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="820fc-108">Properties</span></span>
|<span data-ttu-id="820fc-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="820fc-109">Property</span></span>|<span data-ttu-id="820fc-110">Тип</span><span class="sxs-lookup"><span data-stu-id="820fc-110">Type</span></span>|<span data-ttu-id="820fc-111">Описание</span><span class="sxs-lookup"><span data-stu-id="820fc-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="820fc-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="820fc-112">movieRating</span></span>|[<span data-ttu-id="820fc-113">ratingUnitedStatesMoviesType</span><span class="sxs-lookup"><span data-stu-id="820fc-113">ratingUnitedStatesMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedstatesmoviestype.md)|<span data-ttu-id="820fc-114">Фильмы рейтинг выбранных для США.</span><span class="sxs-lookup"><span data-stu-id="820fc-114">Movies rating selected for United States.</span></span> <span data-ttu-id="820fc-115">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="820fc-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span></span>|
|<span data-ttu-id="820fc-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="820fc-116">tvRating</span></span>|[<span data-ttu-id="820fc-117">ratingUnitedStatesTelevisionType</span><span class="sxs-lookup"><span data-stu-id="820fc-117">ratingUnitedStatesTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedstatestelevisiontype.md)|<span data-ttu-id="820fc-118">Оценка TV, выбранной для США.</span><span class="sxs-lookup"><span data-stu-id="820fc-118">TV rating selected for United States.</span></span> <span data-ttu-id="820fc-119">Возможные значения: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="820fc-119">Possible values are: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="820fc-120">Связи</span><span class="sxs-lookup"><span data-stu-id="820fc-120">Relationships</span></span>
<span data-ttu-id="820fc-121">Нет</span><span class="sxs-lookup"><span data-stu-id="820fc-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="820fc-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="820fc-122">JSON Representation</span></span>
<span data-ttu-id="820fc-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="820fc-123">Here is a JSON representation of the resource.</span></span>
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





