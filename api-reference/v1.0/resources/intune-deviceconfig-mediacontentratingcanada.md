---
title: Тип ресурса mediaContentRatingCanada
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2abc1018d6f9aa271e444560d53f6db6c566a7c0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532451"
---
# <a name="mediacontentratingcanada-resource-type"></a><span data-ttu-id="05a1c-103">Тип ресурса mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="05a1c-103">mediaContentRatingCanada resource type</span></span>

<span data-ttu-id="05a1c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="05a1c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="05a1c-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="05a1c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="05a1c-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="05a1c-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="05a1c-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="05a1c-107">Properties</span></span>
|<span data-ttu-id="05a1c-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="05a1c-108">Property</span></span>|<span data-ttu-id="05a1c-109">Тип</span><span class="sxs-lookup"><span data-stu-id="05a1c-109">Type</span></span>|<span data-ttu-id="05a1c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="05a1c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05a1c-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="05a1c-111">movieRating</span></span>|[<span data-ttu-id="05a1c-112">ратингканадамовиестипе</span><span class="sxs-lookup"><span data-stu-id="05a1c-112">ratingCanadaMoviesType</span></span>](../resources/intune-deviceconfig-ratingcanadamoviestype.md)|<span data-ttu-id="05a1c-113">Оценка фильмов выбрана для Канады.</span><span class="sxs-lookup"><span data-stu-id="05a1c-113">Movies rating selected for Canada.</span></span> <span data-ttu-id="05a1c-114">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span><span class="sxs-lookup"><span data-stu-id="05a1c-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span></span>|
|<span data-ttu-id="05a1c-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="05a1c-115">tvRating</span></span>|[<span data-ttu-id="05a1c-116">ратингканадателевисионтипе</span><span class="sxs-lookup"><span data-stu-id="05a1c-116">ratingCanadaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingcanadatelevisiontype.md)|<span data-ttu-id="05a1c-117">Рейтинг для телевизора выбран для Канады.</span><span class="sxs-lookup"><span data-stu-id="05a1c-117">TV rating selected for Canada.</span></span> <span data-ttu-id="05a1c-118">Возможные значения: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="05a1c-118">Possible values are: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="05a1c-119">Связи</span><span class="sxs-lookup"><span data-stu-id="05a1c-119">Relationships</span></span>
<span data-ttu-id="05a1c-120">Нет</span><span class="sxs-lookup"><span data-stu-id="05a1c-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="05a1c-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="05a1c-121">JSON Representation</span></span>
<span data-ttu-id="05a1c-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="05a1c-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingCanada"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingCanada",
  "movieRating": "String",
  "tvRating": "String"
}
```




