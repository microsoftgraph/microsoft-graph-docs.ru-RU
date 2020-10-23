---
title: Тип ресурса mediaContentRatingFrance
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9ef83c2b02832f46a85a4d2605fdad62f7a42a19
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48702476"
---
# <a name="mediacontentratingfrance-resource-type"></a><span data-ttu-id="1837f-103">Тип ресурса mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="1837f-103">mediaContentRatingFrance resource type</span></span>

<span data-ttu-id="1837f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1837f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1837f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1837f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1837f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1837f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1837f-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="1837f-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="1837f-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="1837f-108">Properties</span></span>
|<span data-ttu-id="1837f-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="1837f-109">Property</span></span>|<span data-ttu-id="1837f-110">Тип</span><span class="sxs-lookup"><span data-stu-id="1837f-110">Type</span></span>|<span data-ttu-id="1837f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="1837f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1837f-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="1837f-112">movieRating</span></span>|[<span data-ttu-id="1837f-113">ратингфранцемовиестипе</span><span class="sxs-lookup"><span data-stu-id="1837f-113">ratingFranceMoviesType</span></span>](../resources/intune-deviceconfig-ratingfrancemoviestype.md)|<span data-ttu-id="1837f-114">Оценка фильмов выбрана для Франции.</span><span class="sxs-lookup"><span data-stu-id="1837f-114">Movies rating selected for France.</span></span> <span data-ttu-id="1837f-115">Возможные значения: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="1837f-115">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|
|<span data-ttu-id="1837f-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="1837f-116">tvRating</span></span>|[<span data-ttu-id="1837f-117">ратингфранцетелевисионтипе</span><span class="sxs-lookup"><span data-stu-id="1837f-117">ratingFranceTelevisionType</span></span>](../resources/intune-deviceconfig-ratingfrancetelevisiontype.md)|<span data-ttu-id="1837f-118">Рейтинг телевизора выбран для Франции.</span><span class="sxs-lookup"><span data-stu-id="1837f-118">TV rating selected for France.</span></span> <span data-ttu-id="1837f-119">Возможные значения: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="1837f-119">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1837f-120">Связи</span><span class="sxs-lookup"><span data-stu-id="1837f-120">Relationships</span></span>
<span data-ttu-id="1837f-121">Нет</span><span class="sxs-lookup"><span data-stu-id="1837f-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1837f-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1837f-122">JSON Representation</span></span>
<span data-ttu-id="1837f-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1837f-123">Here is a JSON representation of the resource.</span></span>
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





