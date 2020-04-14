---
title: Тип ресурса mediaContentRatingUnitedStates
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 570a79280762af3977f88cf374a994a45dfaee4e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43437142"
---
# <a name="mediacontentratingunitedstates-resource-type"></a><span data-ttu-id="62be9-103">Тип ресурса mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="62be9-103">mediaContentRatingUnitedStates resource type</span></span>

<span data-ttu-id="62be9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="62be9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="62be9-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="62be9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="62be9-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="62be9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="62be9-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="62be9-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="62be9-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="62be9-108">Properties</span></span>
|<span data-ttu-id="62be9-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="62be9-109">Property</span></span>|<span data-ttu-id="62be9-110">Тип</span><span class="sxs-lookup"><span data-stu-id="62be9-110">Type</span></span>|<span data-ttu-id="62be9-111">Описание</span><span class="sxs-lookup"><span data-stu-id="62be9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62be9-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="62be9-112">movieRating</span></span>|[<span data-ttu-id="62be9-113">ратингунитедстатесмовиестипе</span><span class="sxs-lookup"><span data-stu-id="62be9-113">ratingUnitedStatesMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedstatesmoviestype.md)|<span data-ttu-id="62be9-114">Оценка фильмов, выбранных для США.</span><span class="sxs-lookup"><span data-stu-id="62be9-114">Movies rating selected for United States.</span></span> <span data-ttu-id="62be9-115">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="62be9-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span></span>|
|<span data-ttu-id="62be9-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="62be9-116">tvRating</span></span>|[<span data-ttu-id="62be9-117">ратингунитедстатестелевисионтипе</span><span class="sxs-lookup"><span data-stu-id="62be9-117">ratingUnitedStatesTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedstatestelevisiontype.md)|<span data-ttu-id="62be9-118">Рейтинг для телевизора выбран для США.</span><span class="sxs-lookup"><span data-stu-id="62be9-118">TV rating selected for United States.</span></span> <span data-ttu-id="62be9-119">Возможные значения: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="62be9-119">Possible values are: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="62be9-120">Связи</span><span class="sxs-lookup"><span data-stu-id="62be9-120">Relationships</span></span>
<span data-ttu-id="62be9-121">Нет</span><span class="sxs-lookup"><span data-stu-id="62be9-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="62be9-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="62be9-122">JSON Representation</span></span>
<span data-ttu-id="62be9-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="62be9-123">Here is a JSON representation of the resource.</span></span>
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



