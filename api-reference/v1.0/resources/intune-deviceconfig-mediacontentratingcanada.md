---
title: Тип ресурса mediaContentRatingCanada
description: Пока не задокументировано.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 88975975b07eb2805ee5f73cc416e3803d5fe24f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32572355"
---
# <a name="mediacontentratingcanada-resource-type"></a><span data-ttu-id="b8847-103">Тип ресурса mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="b8847-103">mediaContentRatingCanada resource type</span></span>

> <span data-ttu-id="b8847-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b8847-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b8847-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="b8847-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="b8847-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="b8847-106">Properties</span></span>
|<span data-ttu-id="b8847-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="b8847-107">Property</span></span>|<span data-ttu-id="b8847-108">Тип</span><span class="sxs-lookup"><span data-stu-id="b8847-108">Type</span></span>|<span data-ttu-id="b8847-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b8847-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8847-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="b8847-110">movieRating</span></span>|[<span data-ttu-id="b8847-111">Ратингканадамовиестипе</span><span class="sxs-lookup"><span data-stu-id="b8847-111">ratingCanadaMoviesType</span></span>](../resources/intune-deviceconfig-ratingcanadamoviestype.md)|<span data-ttu-id="b8847-112">Оценка фильмов выбрана для Канады.</span><span class="sxs-lookup"><span data-stu-id="b8847-112">Movies rating selected for Canada.</span></span> <span data-ttu-id="b8847-113">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span><span class="sxs-lookup"><span data-stu-id="b8847-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span></span>|
|<span data-ttu-id="b8847-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="b8847-114">tvRating</span></span>|[<span data-ttu-id="b8847-115">Ратингканадателевисионтипе</span><span class="sxs-lookup"><span data-stu-id="b8847-115">ratingCanadaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingcanadatelevisiontype.md)|<span data-ttu-id="b8847-116">Рейтинг для телевизора выбран для Канады.</span><span class="sxs-lookup"><span data-stu-id="b8847-116">TV rating selected for Canada.</span></span> <span data-ttu-id="b8847-117">Возможные значения: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="b8847-117">Possible values are: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b8847-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="b8847-118">Relationships</span></span>
<span data-ttu-id="b8847-119">Нет</span><span class="sxs-lookup"><span data-stu-id="b8847-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b8847-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b8847-120">JSON Representation</span></span>
<span data-ttu-id="b8847-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b8847-121">Here is a JSON representation of the resource.</span></span>
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



