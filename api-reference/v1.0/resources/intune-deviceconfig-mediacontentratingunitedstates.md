---
title: Тип ресурса mediaContentRatingUnitedStates
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0175f6f0894df0c859f9951f43c3bb4b857a2256
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760010"
---
# <a name="mediacontentratingunitedstates-resource-type"></a><span data-ttu-id="5c549-103">Тип ресурса mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="5c549-103">mediaContentRatingUnitedStates resource type</span></span>

<span data-ttu-id="5c549-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5c549-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5c549-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5c549-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5c549-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="5c549-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="5c549-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="5c549-107">Properties</span></span>
|<span data-ttu-id="5c549-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="5c549-108">Property</span></span>|<span data-ttu-id="5c549-109">Тип</span><span class="sxs-lookup"><span data-stu-id="5c549-109">Type</span></span>|<span data-ttu-id="5c549-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5c549-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c549-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="5c549-111">movieRating</span></span>|[<span data-ttu-id="5c549-112">ratingUnitedStatesMoviesType</span><span class="sxs-lookup"><span data-stu-id="5c549-112">ratingUnitedStatesMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedstatesmoviestype.md)|<span data-ttu-id="5c549-113">Рейтинг фильмов, выбранный для США.</span><span class="sxs-lookup"><span data-stu-id="5c549-113">Movies rating selected for United States.</span></span> <span data-ttu-id="5c549-114">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="5c549-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span></span>|
|<span data-ttu-id="5c549-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="5c549-115">tvRating</span></span>|[<span data-ttu-id="5c549-116">ratingUnitedStatesTelevisionType</span><span class="sxs-lookup"><span data-stu-id="5c549-116">ratingUnitedStatesTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedstatestelevisiontype.md)|<span data-ttu-id="5c549-117">Телевизионный рейтинг, выбранный для США.</span><span class="sxs-lookup"><span data-stu-id="5c549-117">TV rating selected for United States.</span></span> <span data-ttu-id="5c549-118">Возможные значения: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="5c549-118">Possible values are: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5c549-119">Связи</span><span class="sxs-lookup"><span data-stu-id="5c549-119">Relationships</span></span>
<span data-ttu-id="5c549-120">Нет</span><span class="sxs-lookup"><span data-stu-id="5c549-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5c549-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5c549-121">JSON Representation</span></span>
<span data-ttu-id="5c549-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5c549-122">Here is a JSON representation of the resource.</span></span>
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




