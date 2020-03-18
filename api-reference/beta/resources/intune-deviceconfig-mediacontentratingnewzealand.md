---
title: Тип ресурса mediaContentRatingNewZealand
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e61d2b5e9589bd0e337941dfce7cc1bfbbbc8dd4
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42788564"
---
# <a name="mediacontentratingnewzealand-resource-type"></a><span data-ttu-id="87a96-103">Тип ресурса mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="87a96-103">mediaContentRatingNewZealand resource type</span></span>

> <span data-ttu-id="87a96-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="87a96-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="87a96-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="87a96-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="87a96-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="87a96-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="87a96-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="87a96-107">Properties</span></span>
|<span data-ttu-id="87a96-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="87a96-108">Property</span></span>|<span data-ttu-id="87a96-109">Тип</span><span class="sxs-lookup"><span data-stu-id="87a96-109">Type</span></span>|<span data-ttu-id="87a96-110">Описание</span><span class="sxs-lookup"><span data-stu-id="87a96-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="87a96-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="87a96-111">movieRating</span></span>|[<span data-ttu-id="87a96-112">ратингневзеаландмовиестипе</span><span class="sxs-lookup"><span data-stu-id="87a96-112">ratingNewZealandMoviesType</span></span>](../resources/intune-deviceconfig-ratingnewzealandmoviestype.md)|<span data-ttu-id="87a96-113">Рейтинг фильмов, выбранный для Новой Зеландии.</span><span class="sxs-lookup"><span data-stu-id="87a96-113">Movies rating selected for New Zealand.</span></span> <span data-ttu-id="87a96-114">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span><span class="sxs-lookup"><span data-stu-id="87a96-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span></span>|
|<span data-ttu-id="87a96-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="87a96-115">tvRating</span></span>|[<span data-ttu-id="87a96-116">ратингневзеаландтелевисионтипе</span><span class="sxs-lookup"><span data-stu-id="87a96-116">ratingNewZealandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingnewzealandtelevisiontype.md)|<span data-ttu-id="87a96-117">Рейтинг для телевизора, выбранный для Новой Зеландии.</span><span class="sxs-lookup"><span data-stu-id="87a96-117">TV rating selected for New Zealand.</span></span> <span data-ttu-id="87a96-118">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="87a96-118">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="87a96-119">Связи</span><span class="sxs-lookup"><span data-stu-id="87a96-119">Relationships</span></span>
<span data-ttu-id="87a96-120">Нет</span><span class="sxs-lookup"><span data-stu-id="87a96-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="87a96-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="87a96-121">JSON Representation</span></span>
<span data-ttu-id="87a96-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="87a96-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingNewZealand"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingNewZealand",
  "movieRating": "String",
  "tvRating": "String"
}
```



