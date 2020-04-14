---
title: Тип ресурса mediaContentRatingFrance
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c7ac9e4309f2f6cf97c0caf6faed36f43347d5a8
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43437224"
---
# <a name="mediacontentratingfrance-resource-type"></a><span data-ttu-id="482e7-103">Тип ресурса mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="482e7-103">mediaContentRatingFrance resource type</span></span>

<span data-ttu-id="482e7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="482e7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="482e7-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="482e7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="482e7-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="482e7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="482e7-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="482e7-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="482e7-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="482e7-108">Properties</span></span>
|<span data-ttu-id="482e7-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="482e7-109">Property</span></span>|<span data-ttu-id="482e7-110">Тип</span><span class="sxs-lookup"><span data-stu-id="482e7-110">Type</span></span>|<span data-ttu-id="482e7-111">Описание</span><span class="sxs-lookup"><span data-stu-id="482e7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="482e7-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="482e7-112">movieRating</span></span>|[<span data-ttu-id="482e7-113">ратингфранцемовиестипе</span><span class="sxs-lookup"><span data-stu-id="482e7-113">ratingFranceMoviesType</span></span>](../resources/intune-deviceconfig-ratingfrancemoviestype.md)|<span data-ttu-id="482e7-114">Оценка фильмов выбрана для Франции.</span><span class="sxs-lookup"><span data-stu-id="482e7-114">Movies rating selected for France.</span></span> <span data-ttu-id="482e7-115">Возможные значения: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="482e7-115">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|
|<span data-ttu-id="482e7-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="482e7-116">tvRating</span></span>|[<span data-ttu-id="482e7-117">ратингфранцетелевисионтипе</span><span class="sxs-lookup"><span data-stu-id="482e7-117">ratingFranceTelevisionType</span></span>](../resources/intune-deviceconfig-ratingfrancetelevisiontype.md)|<span data-ttu-id="482e7-118">Рейтинг телевизора выбран для Франции.</span><span class="sxs-lookup"><span data-stu-id="482e7-118">TV rating selected for France.</span></span> <span data-ttu-id="482e7-119">Возможные значения: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="482e7-119">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="482e7-120">Связи</span><span class="sxs-lookup"><span data-stu-id="482e7-120">Relationships</span></span>
<span data-ttu-id="482e7-121">Нет</span><span class="sxs-lookup"><span data-stu-id="482e7-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="482e7-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="482e7-122">JSON Representation</span></span>
<span data-ttu-id="482e7-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="482e7-123">Here is a JSON representation of the resource.</span></span>
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



