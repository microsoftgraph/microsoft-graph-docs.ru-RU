---
title: Тип ресурса mediaContentRatingJapan
description: Пока не задокументировано.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8c4e4268857f2d76e1dcf01e047a492f80492a89
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031390"
---
# <a name="mediacontentratingjapan-resource-type"></a><span data-ttu-id="38cd6-103">Тип ресурса mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="38cd6-103">mediaContentRatingJapan resource type</span></span>

> <span data-ttu-id="38cd6-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="38cd6-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="38cd6-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="38cd6-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="38cd6-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="38cd6-106">Properties</span></span>
|<span data-ttu-id="38cd6-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="38cd6-107">Property</span></span>|<span data-ttu-id="38cd6-108">Тип</span><span class="sxs-lookup"><span data-stu-id="38cd6-108">Type</span></span>|<span data-ttu-id="38cd6-109">Описание</span><span class="sxs-lookup"><span data-stu-id="38cd6-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38cd6-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="38cd6-110">movieRating</span></span>|[<span data-ttu-id="38cd6-111">Ратингжапанмовиестипе</span><span class="sxs-lookup"><span data-stu-id="38cd6-111">ratingJapanMoviesType</span></span>](../resources/intune-deviceconfig-ratingjapanmoviestype.md)|<span data-ttu-id="38cd6-112">Оценка фильмов выбрана для Японии.</span><span class="sxs-lookup"><span data-stu-id="38cd6-112">Movies rating selected for Japan.</span></span> <span data-ttu-id="38cd6-113">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="38cd6-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="38cd6-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="38cd6-114">tvRating</span></span>|[<span data-ttu-id="38cd6-115">Ратингжапантелевисионтипе</span><span class="sxs-lookup"><span data-stu-id="38cd6-115">ratingJapanTelevisionType</span></span>](../resources/intune-deviceconfig-ratingjapantelevisiontype.md)|<span data-ttu-id="38cd6-116">Рейтинг для телевизора выбран для Японии.</span><span class="sxs-lookup"><span data-stu-id="38cd6-116">TV rating selected for Japan.</span></span> <span data-ttu-id="38cd6-117">Возможные значения: `allAllowed`, `allBlocked`, `explicitAllowed`.</span><span class="sxs-lookup"><span data-stu-id="38cd6-117">Possible values are: `allAllowed`, `allBlocked`, `explicitAllowed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="38cd6-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="38cd6-118">Relationships</span></span>
<span data-ttu-id="38cd6-119">Нет</span><span class="sxs-lookup"><span data-stu-id="38cd6-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="38cd6-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="38cd6-120">JSON Representation</span></span>
<span data-ttu-id="38cd6-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="38cd6-121">Here is a JSON representation of the resource.</span></span>
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



