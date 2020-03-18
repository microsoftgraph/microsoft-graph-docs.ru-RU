---
title: Тип ресурса mediaContentRatingGermany
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f32a6ed59861dce47f5c38f7259b78879bf1681c
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42788585"
---
# <a name="mediacontentratinggermany-resource-type"></a><span data-ttu-id="ce5be-103">Тип ресурса mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="ce5be-103">mediaContentRatingGermany resource type</span></span>

> <span data-ttu-id="ce5be-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce5be-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ce5be-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ce5be-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ce5be-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="ce5be-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="ce5be-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="ce5be-107">Properties</span></span>
|<span data-ttu-id="ce5be-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="ce5be-108">Property</span></span>|<span data-ttu-id="ce5be-109">Тип</span><span class="sxs-lookup"><span data-stu-id="ce5be-109">Type</span></span>|<span data-ttu-id="ce5be-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ce5be-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ce5be-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="ce5be-111">movieRating</span></span>|[<span data-ttu-id="ce5be-112">ратингжерманимовиестипе</span><span class="sxs-lookup"><span data-stu-id="ce5be-112">ratingGermanyMoviesType</span></span>](../resources/intune-deviceconfig-ratinggermanymoviestype.md)|<span data-ttu-id="ce5be-113">Оценка фильмов выбрана для Германии.</span><span class="sxs-lookup"><span data-stu-id="ce5be-113">Movies rating selected for Germany.</span></span> <span data-ttu-id="ce5be-114">Возможные значения: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="ce5be-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="ce5be-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="ce5be-115">tvRating</span></span>|[<span data-ttu-id="ce5be-116">ратингжерманителевисионтипе</span><span class="sxs-lookup"><span data-stu-id="ce5be-116">ratingGermanyTelevisionType</span></span>](../resources/intune-deviceconfig-ratinggermanytelevisiontype.md)|<span data-ttu-id="ce5be-117">Рейтинг для телевизора выбран в Германии.</span><span class="sxs-lookup"><span data-stu-id="ce5be-117">TV rating selected for Germany.</span></span> <span data-ttu-id="ce5be-118">Возможные значения: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="ce5be-118">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ce5be-119">Связи</span><span class="sxs-lookup"><span data-stu-id="ce5be-119">Relationships</span></span>
<span data-ttu-id="ce5be-120">Нет</span><span class="sxs-lookup"><span data-stu-id="ce5be-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ce5be-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ce5be-121">JSON Representation</span></span>
<span data-ttu-id="ce5be-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ce5be-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingGermany"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingGermany",
  "movieRating": "String",
  "tvRating": "String"
}
```



