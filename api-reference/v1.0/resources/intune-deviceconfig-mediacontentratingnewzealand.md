---
title: Тип ресурса mediaContentRatingNewZealand
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 943a2d12ea1774bff6f12acd958b22f884cfa749
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532442"
---
# <a name="mediacontentratingnewzealand-resource-type"></a><span data-ttu-id="6f108-103">Тип ресурса mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="6f108-103">mediaContentRatingNewZealand resource type</span></span>

<span data-ttu-id="6f108-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6f108-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6f108-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6f108-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6f108-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="6f108-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="6f108-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="6f108-107">Properties</span></span>
|<span data-ttu-id="6f108-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="6f108-108">Property</span></span>|<span data-ttu-id="6f108-109">Тип</span><span class="sxs-lookup"><span data-stu-id="6f108-109">Type</span></span>|<span data-ttu-id="6f108-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6f108-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f108-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="6f108-111">movieRating</span></span>|[<span data-ttu-id="6f108-112">ратингневзеаландмовиестипе</span><span class="sxs-lookup"><span data-stu-id="6f108-112">ratingNewZealandMoviesType</span></span>](../resources/intune-deviceconfig-ratingnewzealandmoviestype.md)|<span data-ttu-id="6f108-113">Рейтинг фильмов, выбранный для Новой Зеландии.</span><span class="sxs-lookup"><span data-stu-id="6f108-113">Movies rating selected for New Zealand.</span></span> <span data-ttu-id="6f108-114">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span><span class="sxs-lookup"><span data-stu-id="6f108-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span></span>|
|<span data-ttu-id="6f108-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="6f108-115">tvRating</span></span>|[<span data-ttu-id="6f108-116">ратингневзеаландтелевисионтипе</span><span class="sxs-lookup"><span data-stu-id="6f108-116">ratingNewZealandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingnewzealandtelevisiontype.md)|<span data-ttu-id="6f108-117">Рейтинг для телевизора, выбранный для Новой Зеландии.</span><span class="sxs-lookup"><span data-stu-id="6f108-117">TV rating selected for New Zealand.</span></span> <span data-ttu-id="6f108-118">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="6f108-118">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6f108-119">Связи</span><span class="sxs-lookup"><span data-stu-id="6f108-119">Relationships</span></span>
<span data-ttu-id="6f108-120">Нет</span><span class="sxs-lookup"><span data-stu-id="6f108-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6f108-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6f108-121">JSON Representation</span></span>
<span data-ttu-id="6f108-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6f108-122">Here is a JSON representation of the resource.</span></span>
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




