---
title: Тип ресурса mediaContentRatingIreland
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b2da5f800d719558e0ba3990fbb7efb7b9280176
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529620"
---
# <a name="mediacontentratingireland-resource-type"></a><span data-ttu-id="949ce-103">Тип ресурса mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="949ce-103">mediaContentRatingIreland resource type</span></span>

<span data-ttu-id="949ce-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="949ce-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="949ce-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="949ce-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="949ce-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="949ce-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="949ce-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="949ce-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="949ce-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="949ce-108">Properties</span></span>
|<span data-ttu-id="949ce-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="949ce-109">Property</span></span>|<span data-ttu-id="949ce-110">Тип</span><span class="sxs-lookup"><span data-stu-id="949ce-110">Type</span></span>|<span data-ttu-id="949ce-111">Описание</span><span class="sxs-lookup"><span data-stu-id="949ce-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="949ce-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="949ce-112">movieRating</span></span>|[<span data-ttu-id="949ce-113">ратингиреландмовиестипе</span><span class="sxs-lookup"><span data-stu-id="949ce-113">ratingIrelandMoviesType</span></span>](../resources/intune-deviceconfig-ratingirelandmoviestype.md)|<span data-ttu-id="949ce-114">Оценка фильмов выбрана для Ирландии.</span><span class="sxs-lookup"><span data-stu-id="949ce-114">Movies rating selected for Ireland.</span></span> <span data-ttu-id="949ce-115">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="949ce-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="949ce-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="949ce-116">tvRating</span></span>|[<span data-ttu-id="949ce-117">ратингиреландтелевисионтипе</span><span class="sxs-lookup"><span data-stu-id="949ce-117">ratingIrelandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingirelandtelevisiontype.md)|<span data-ttu-id="949ce-118">Рейтинг телевизора выбран для Ирландии.</span><span class="sxs-lookup"><span data-stu-id="949ce-118">TV rating selected for Ireland.</span></span> <span data-ttu-id="949ce-119">Возможные значения: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span><span class="sxs-lookup"><span data-stu-id="949ce-119">Possible values are: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="949ce-120">Связи</span><span class="sxs-lookup"><span data-stu-id="949ce-120">Relationships</span></span>
<span data-ttu-id="949ce-121">Нет</span><span class="sxs-lookup"><span data-stu-id="949ce-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="949ce-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="949ce-122">JSON Representation</span></span>
<span data-ttu-id="949ce-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="949ce-123">Here is a JSON representation of the resource.</span></span>
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



