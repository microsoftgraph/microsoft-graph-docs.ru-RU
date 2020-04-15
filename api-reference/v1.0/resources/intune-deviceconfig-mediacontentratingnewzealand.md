---
title: Тип ресурса mediaContentRatingNewZealand
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6787ec82cf70aa10c72a20ab60619449dbb14327
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43473108"
---
# <a name="mediacontentratingnewzealand-resource-type"></a><span data-ttu-id="20630-103">Тип ресурса mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="20630-103">mediaContentRatingNewZealand resource type</span></span>

<span data-ttu-id="20630-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="20630-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="20630-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="20630-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="20630-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="20630-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="20630-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="20630-107">Properties</span></span>
|<span data-ttu-id="20630-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="20630-108">Property</span></span>|<span data-ttu-id="20630-109">Тип</span><span class="sxs-lookup"><span data-stu-id="20630-109">Type</span></span>|<span data-ttu-id="20630-110">Описание</span><span class="sxs-lookup"><span data-stu-id="20630-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="20630-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="20630-111">movieRating</span></span>|[<span data-ttu-id="20630-112">ратингневзеаландмовиестипе</span><span class="sxs-lookup"><span data-stu-id="20630-112">ratingNewZealandMoviesType</span></span>](../resources/intune-deviceconfig-ratingnewzealandmoviestype.md)|<span data-ttu-id="20630-113">Рейтинг фильмов, выбранный для Новой Зеландии.</span><span class="sxs-lookup"><span data-stu-id="20630-113">Movies rating selected for New Zealand.</span></span> <span data-ttu-id="20630-114">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span><span class="sxs-lookup"><span data-stu-id="20630-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span></span>|
|<span data-ttu-id="20630-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="20630-115">tvRating</span></span>|[<span data-ttu-id="20630-116">ратингневзеаландтелевисионтипе</span><span class="sxs-lookup"><span data-stu-id="20630-116">ratingNewZealandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingnewzealandtelevisiontype.md)|<span data-ttu-id="20630-117">Рейтинг для телевизора, выбранный для Новой Зеландии.</span><span class="sxs-lookup"><span data-stu-id="20630-117">TV rating selected for New Zealand.</span></span> <span data-ttu-id="20630-118">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="20630-118">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="20630-119">Отношения</span><span class="sxs-lookup"><span data-stu-id="20630-119">Relationships</span></span>
<span data-ttu-id="20630-120">Нет</span><span class="sxs-lookup"><span data-stu-id="20630-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="20630-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="20630-121">JSON Representation</span></span>
<span data-ttu-id="20630-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="20630-122">Here is a JSON representation of the resource.</span></span>
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







