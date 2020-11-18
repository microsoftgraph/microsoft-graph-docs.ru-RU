---
title: Тип ресурса mediaContentRatingJapan
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b5efd89490b83994ab9ce771a235fa2c8ab0e144
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49198723"
---
# <a name="mediacontentratingjapan-resource-type"></a><span data-ttu-id="a9cbd-103">Тип ресурса mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="a9cbd-103">mediaContentRatingJapan resource type</span></span>

<span data-ttu-id="a9cbd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a9cbd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a9cbd-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a9cbd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a9cbd-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a9cbd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a9cbd-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="a9cbd-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="a9cbd-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="a9cbd-108">Properties</span></span>
|<span data-ttu-id="a9cbd-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="a9cbd-109">Property</span></span>|<span data-ttu-id="a9cbd-110">Тип</span><span class="sxs-lookup"><span data-stu-id="a9cbd-110">Type</span></span>|<span data-ttu-id="a9cbd-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a9cbd-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9cbd-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="a9cbd-112">movieRating</span></span>|[<span data-ttu-id="a9cbd-113">ратингжапанмовиестипе</span><span class="sxs-lookup"><span data-stu-id="a9cbd-113">ratingJapanMoviesType</span></span>](../resources/intune-deviceconfig-ratingjapanmoviestype.md)|<span data-ttu-id="a9cbd-114">Оценка фильмов выбрана для Японии.</span><span class="sxs-lookup"><span data-stu-id="a9cbd-114">Movies rating selected for Japan.</span></span> <span data-ttu-id="a9cbd-115">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="a9cbd-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="a9cbd-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="a9cbd-116">tvRating</span></span>|[<span data-ttu-id="a9cbd-117">ратингжапантелевисионтипе</span><span class="sxs-lookup"><span data-stu-id="a9cbd-117">ratingJapanTelevisionType</span></span>](../resources/intune-deviceconfig-ratingjapantelevisiontype.md)|<span data-ttu-id="a9cbd-118">Рейтинг для телевизора выбран для Японии.</span><span class="sxs-lookup"><span data-stu-id="a9cbd-118">TV rating selected for Japan.</span></span> <span data-ttu-id="a9cbd-119">Возможные значения: `allAllowed`, `allBlocked`, `explicitAllowed`.</span><span class="sxs-lookup"><span data-stu-id="a9cbd-119">Possible values are: `allAllowed`, `allBlocked`, `explicitAllowed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a9cbd-120">Связи</span><span class="sxs-lookup"><span data-stu-id="a9cbd-120">Relationships</span></span>
<span data-ttu-id="a9cbd-121">Нет</span><span class="sxs-lookup"><span data-stu-id="a9cbd-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a9cbd-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a9cbd-122">JSON Representation</span></span>
<span data-ttu-id="a9cbd-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a9cbd-123">Here is a JSON representation of the resource.</span></span>
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




