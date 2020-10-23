---
title: Тип ресурса mediaContentRatingUnitedStates
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9af3916d29bfc3f48ee3d4c04dc17ab1f0fa3045
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48707166"
---
# <a name="mediacontentratingunitedstates-resource-type"></a><span data-ttu-id="bbe4a-103">Тип ресурса mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="bbe4a-103">mediaContentRatingUnitedStates resource type</span></span>

<span data-ttu-id="bbe4a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bbe4a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bbe4a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bbe4a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bbe4a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bbe4a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bbe4a-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="bbe4a-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="bbe4a-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="bbe4a-108">Properties</span></span>
|<span data-ttu-id="bbe4a-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="bbe4a-109">Property</span></span>|<span data-ttu-id="bbe4a-110">Тип</span><span class="sxs-lookup"><span data-stu-id="bbe4a-110">Type</span></span>|<span data-ttu-id="bbe4a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="bbe4a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bbe4a-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="bbe4a-112">movieRating</span></span>|[<span data-ttu-id="bbe4a-113">ратингунитедстатесмовиестипе</span><span class="sxs-lookup"><span data-stu-id="bbe4a-113">ratingUnitedStatesMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedstatesmoviestype.md)|<span data-ttu-id="bbe4a-114">Оценка фильмов, выбранных для США.</span><span class="sxs-lookup"><span data-stu-id="bbe4a-114">Movies rating selected for United States.</span></span> <span data-ttu-id="bbe4a-115">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="bbe4a-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span></span>|
|<span data-ttu-id="bbe4a-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="bbe4a-116">tvRating</span></span>|[<span data-ttu-id="bbe4a-117">ратингунитедстатестелевисионтипе</span><span class="sxs-lookup"><span data-stu-id="bbe4a-117">ratingUnitedStatesTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedstatestelevisiontype.md)|<span data-ttu-id="bbe4a-118">Рейтинг для телевизора выбран для США.</span><span class="sxs-lookup"><span data-stu-id="bbe4a-118">TV rating selected for United States.</span></span> <span data-ttu-id="bbe4a-119">Возможные значения: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="bbe4a-119">Possible values are: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bbe4a-120">Связи</span><span class="sxs-lookup"><span data-stu-id="bbe4a-120">Relationships</span></span>
<span data-ttu-id="bbe4a-121">Нет</span><span class="sxs-lookup"><span data-stu-id="bbe4a-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bbe4a-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bbe4a-122">JSON Representation</span></span>
<span data-ttu-id="bbe4a-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bbe4a-123">Here is a JSON representation of the resource.</span></span>
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





