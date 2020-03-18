---
title: Тип ресурса mediaContentRatingUnitedStates
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 59029a86d21cc0f185f66222b054618cb34977cd
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42788550"
---
# <a name="mediacontentratingunitedstates-resource-type"></a><span data-ttu-id="9fca1-103">Тип ресурса mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="9fca1-103">mediaContentRatingUnitedStates resource type</span></span>

> <span data-ttu-id="9fca1-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9fca1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9fca1-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9fca1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9fca1-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="9fca1-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="9fca1-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="9fca1-107">Properties</span></span>
|<span data-ttu-id="9fca1-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="9fca1-108">Property</span></span>|<span data-ttu-id="9fca1-109">Тип</span><span class="sxs-lookup"><span data-stu-id="9fca1-109">Type</span></span>|<span data-ttu-id="9fca1-110">Описание</span><span class="sxs-lookup"><span data-stu-id="9fca1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9fca1-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="9fca1-111">movieRating</span></span>|[<span data-ttu-id="9fca1-112">ратингунитедстатесмовиестипе</span><span class="sxs-lookup"><span data-stu-id="9fca1-112">ratingUnitedStatesMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedstatesmoviestype.md)|<span data-ttu-id="9fca1-113">Оценка фильмов, выбранных для США.</span><span class="sxs-lookup"><span data-stu-id="9fca1-113">Movies rating selected for United States.</span></span> <span data-ttu-id="9fca1-114">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="9fca1-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span></span>|
|<span data-ttu-id="9fca1-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="9fca1-115">tvRating</span></span>|[<span data-ttu-id="9fca1-116">ратингунитедстатестелевисионтипе</span><span class="sxs-lookup"><span data-stu-id="9fca1-116">ratingUnitedStatesTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedstatestelevisiontype.md)|<span data-ttu-id="9fca1-117">Рейтинг для телевизора выбран для США.</span><span class="sxs-lookup"><span data-stu-id="9fca1-117">TV rating selected for United States.</span></span> <span data-ttu-id="9fca1-118">Возможные значения: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="9fca1-118">Possible values are: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9fca1-119">Связи</span><span class="sxs-lookup"><span data-stu-id="9fca1-119">Relationships</span></span>
<span data-ttu-id="9fca1-120">Нет</span><span class="sxs-lookup"><span data-stu-id="9fca1-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9fca1-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9fca1-121">JSON Representation</span></span>
<span data-ttu-id="9fca1-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9fca1-122">Here is a JSON representation of the resource.</span></span>
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



