---
title: Тип ресурса mediaContentRatingFrance
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d24763bd209c389235dd9e2198ed8f86cad85169
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33944854"
---
# <a name="mediacontentratingfrance-resource-type"></a><span data-ttu-id="df259-103">Тип ресурса mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="df259-103">mediaContentRatingFrance resource type</span></span>

> <span data-ttu-id="df259-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="df259-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="df259-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="df259-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="df259-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="df259-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="df259-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="df259-107">Properties</span></span>
|<span data-ttu-id="df259-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="df259-108">Property</span></span>|<span data-ttu-id="df259-109">Тип</span><span class="sxs-lookup"><span data-stu-id="df259-109">Type</span></span>|<span data-ttu-id="df259-110">Описание</span><span class="sxs-lookup"><span data-stu-id="df259-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df259-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="df259-111">movieRating</span></span>|[<span data-ttu-id="df259-112">Ратингфранцемовиестипе</span><span class="sxs-lookup"><span data-stu-id="df259-112">ratingFranceMoviesType</span></span>](../resources/intune-deviceconfig-ratingfrancemoviestype.md)|<span data-ttu-id="df259-113">Оценка фильмов выбрана для Франции.</span><span class="sxs-lookup"><span data-stu-id="df259-113">Movies rating selected for France.</span></span> <span data-ttu-id="df259-114">Возможные значения: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="df259-114">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|
|<span data-ttu-id="df259-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="df259-115">tvRating</span></span>|[<span data-ttu-id="df259-116">Ратингфранцетелевисионтипе</span><span class="sxs-lookup"><span data-stu-id="df259-116">ratingFranceTelevisionType</span></span>](../resources/intune-deviceconfig-ratingfrancetelevisiontype.md)|<span data-ttu-id="df259-117">Рейтинг телевизора выбран для Франции.</span><span class="sxs-lookup"><span data-stu-id="df259-117">TV rating selected for France.</span></span> <span data-ttu-id="df259-118">Возможные значения: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="df259-118">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="df259-119">Связи</span><span class="sxs-lookup"><span data-stu-id="df259-119">Relationships</span></span>
<span data-ttu-id="df259-120">Нет</span><span class="sxs-lookup"><span data-stu-id="df259-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="df259-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="df259-121">JSON Representation</span></span>
<span data-ttu-id="df259-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="df259-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingFrance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingFrance",
  "movieRating": "String",
  "tvRating": "String"
}
```




