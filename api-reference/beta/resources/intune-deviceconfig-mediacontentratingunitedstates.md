---
title: Тип ресурса mediaContentRatingUnitedStates
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7ccfd31d7e47d4a4e08a63e163661c4a2a82da7c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48052700"
---
# <a name="mediacontentratingunitedstates-resource-type"></a><span data-ttu-id="bb588-103">Тип ресурса mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="bb588-103">mediaContentRatingUnitedStates resource type</span></span>

<span data-ttu-id="bb588-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bb588-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bb588-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb588-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bb588-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bb588-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb588-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="bb588-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="bb588-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="bb588-108">Properties</span></span>
|<span data-ttu-id="bb588-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="bb588-109">Property</span></span>|<span data-ttu-id="bb588-110">Тип</span><span class="sxs-lookup"><span data-stu-id="bb588-110">Type</span></span>|<span data-ttu-id="bb588-111">Описание</span><span class="sxs-lookup"><span data-stu-id="bb588-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb588-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="bb588-112">movieRating</span></span>|[<span data-ttu-id="bb588-113">ратингунитедстатесмовиестипе</span><span class="sxs-lookup"><span data-stu-id="bb588-113">ratingUnitedStatesMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedstatesmoviestype.md)|<span data-ttu-id="bb588-114">Оценка фильмов, выбранных для США.</span><span class="sxs-lookup"><span data-stu-id="bb588-114">Movies rating selected for United States.</span></span> <span data-ttu-id="bb588-115">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="bb588-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span></span>|
|<span data-ttu-id="bb588-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="bb588-116">tvRating</span></span>|[<span data-ttu-id="bb588-117">ратингунитедстатестелевисионтипе</span><span class="sxs-lookup"><span data-stu-id="bb588-117">ratingUnitedStatesTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedstatestelevisiontype.md)|<span data-ttu-id="bb588-118">Рейтинг для телевизора выбран для США.</span><span class="sxs-lookup"><span data-stu-id="bb588-118">TV rating selected for United States.</span></span> <span data-ttu-id="bb588-119">Возможные значения: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="bb588-119">Possible values are: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bb588-120">Связи</span><span class="sxs-lookup"><span data-stu-id="bb588-120">Relationships</span></span>
<span data-ttu-id="bb588-121">Нет</span><span class="sxs-lookup"><span data-stu-id="bb588-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bb588-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bb588-122">JSON Representation</span></span>
<span data-ttu-id="bb588-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bb588-123">Here is a JSON representation of the resource.</span></span>
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






