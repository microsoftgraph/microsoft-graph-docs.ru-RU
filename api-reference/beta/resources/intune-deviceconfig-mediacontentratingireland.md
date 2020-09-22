---
title: Тип ресурса mediaContentRatingIreland
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 58f4903bf2295caf48f483c95c2e42331796bc99
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47993814"
---
# <a name="mediacontentratingireland-resource-type"></a><span data-ttu-id="a181c-103">Тип ресурса mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="a181c-103">mediaContentRatingIreland resource type</span></span>

<span data-ttu-id="a181c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a181c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a181c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a181c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a181c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a181c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a181c-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="a181c-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="a181c-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="a181c-108">Properties</span></span>
|<span data-ttu-id="a181c-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="a181c-109">Property</span></span>|<span data-ttu-id="a181c-110">Тип</span><span class="sxs-lookup"><span data-stu-id="a181c-110">Type</span></span>|<span data-ttu-id="a181c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a181c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a181c-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="a181c-112">movieRating</span></span>|[<span data-ttu-id="a181c-113">ратингиреландмовиестипе</span><span class="sxs-lookup"><span data-stu-id="a181c-113">ratingIrelandMoviesType</span></span>](../resources/intune-deviceconfig-ratingirelandmoviestype.md)|<span data-ttu-id="a181c-114">Оценка фильмов выбрана для Ирландии.</span><span class="sxs-lookup"><span data-stu-id="a181c-114">Movies rating selected for Ireland.</span></span> <span data-ttu-id="a181c-115">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="a181c-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="a181c-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="a181c-116">tvRating</span></span>|[<span data-ttu-id="a181c-117">ратингиреландтелевисионтипе</span><span class="sxs-lookup"><span data-stu-id="a181c-117">ratingIrelandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingirelandtelevisiontype.md)|<span data-ttu-id="a181c-118">Рейтинг телевизора выбран для Ирландии.</span><span class="sxs-lookup"><span data-stu-id="a181c-118">TV rating selected for Ireland.</span></span> <span data-ttu-id="a181c-119">Возможные значения: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span><span class="sxs-lookup"><span data-stu-id="a181c-119">Possible values are: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a181c-120">Связи</span><span class="sxs-lookup"><span data-stu-id="a181c-120">Relationships</span></span>
<span data-ttu-id="a181c-121">Нет</span><span class="sxs-lookup"><span data-stu-id="a181c-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a181c-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a181c-122">JSON Representation</span></span>
<span data-ttu-id="a181c-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a181c-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingIreland"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingIreland",
  "movieRating": "String",
  "tvRating": "String"
}
```






