---
title: Тип ресурса mediaContentRatingJapan
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 658141a661bd46374c63a2c7eb9378a16d4135aa
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47993800"
---
# <a name="mediacontentratingjapan-resource-type"></a><span data-ttu-id="f93b3-103">Тип ресурса mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="f93b3-103">mediaContentRatingJapan resource type</span></span>

<span data-ttu-id="f93b3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f93b3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f93b3-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f93b3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f93b3-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f93b3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f93b3-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="f93b3-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="f93b3-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="f93b3-108">Properties</span></span>
|<span data-ttu-id="f93b3-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="f93b3-109">Property</span></span>|<span data-ttu-id="f93b3-110">Тип</span><span class="sxs-lookup"><span data-stu-id="f93b3-110">Type</span></span>|<span data-ttu-id="f93b3-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f93b3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f93b3-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="f93b3-112">movieRating</span></span>|[<span data-ttu-id="f93b3-113">ратингжапанмовиестипе</span><span class="sxs-lookup"><span data-stu-id="f93b3-113">ratingJapanMoviesType</span></span>](../resources/intune-deviceconfig-ratingjapanmoviestype.md)|<span data-ttu-id="f93b3-114">Оценка фильмов выбрана для Японии.</span><span class="sxs-lookup"><span data-stu-id="f93b3-114">Movies rating selected for Japan.</span></span> <span data-ttu-id="f93b3-115">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="f93b3-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="f93b3-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="f93b3-116">tvRating</span></span>|[<span data-ttu-id="f93b3-117">ратингжапантелевисионтипе</span><span class="sxs-lookup"><span data-stu-id="f93b3-117">ratingJapanTelevisionType</span></span>](../resources/intune-deviceconfig-ratingjapantelevisiontype.md)|<span data-ttu-id="f93b3-118">Рейтинг для телевизора выбран для Японии.</span><span class="sxs-lookup"><span data-stu-id="f93b3-118">TV rating selected for Japan.</span></span> <span data-ttu-id="f93b3-119">Возможные значения: `allAllowed`, `allBlocked`, `explicitAllowed`.</span><span class="sxs-lookup"><span data-stu-id="f93b3-119">Possible values are: `allAllowed`, `allBlocked`, `explicitAllowed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f93b3-120">Связи</span><span class="sxs-lookup"><span data-stu-id="f93b3-120">Relationships</span></span>
<span data-ttu-id="f93b3-121">Нет</span><span class="sxs-lookup"><span data-stu-id="f93b3-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f93b3-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f93b3-122">JSON Representation</span></span>
<span data-ttu-id="f93b3-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f93b3-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingJapan"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingJapan",
  "movieRating": "String",
  "tvRating": "String"
}
```






