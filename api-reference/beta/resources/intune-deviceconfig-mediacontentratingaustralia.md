---
title: Тип ресурса mediaContentRatingAustralia
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9fc72352f667f0d5b6a3801b10582b6707489ed0
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33944931"
---
# <a name="mediacontentratingaustralia-resource-type"></a><span data-ttu-id="13bed-103">Тип ресурса mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="13bed-103">mediaContentRatingAustralia resource type</span></span>

> <span data-ttu-id="13bed-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="13bed-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="13bed-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="13bed-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13bed-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="13bed-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="13bed-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="13bed-107">Properties</span></span>
|<span data-ttu-id="13bed-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="13bed-108">Property</span></span>|<span data-ttu-id="13bed-109">Тип</span><span class="sxs-lookup"><span data-stu-id="13bed-109">Type</span></span>|<span data-ttu-id="13bed-110">Описание</span><span class="sxs-lookup"><span data-stu-id="13bed-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13bed-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="13bed-111">movieRating</span></span>|[<span data-ttu-id="13bed-112">Ратингаустралиамовиестипе</span><span class="sxs-lookup"><span data-stu-id="13bed-112">ratingAustraliaMoviesType</span></span>](../resources/intune-deviceconfig-ratingaustraliamoviestype.md)|<span data-ttu-id="13bed-113">Оценка фильмов выбрана для Австралии.</span><span class="sxs-lookup"><span data-stu-id="13bed-113">Movies rating selected for Australia.</span></span> <span data-ttu-id="13bed-114">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="13bed-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="13bed-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="13bed-115">tvRating</span></span>|[<span data-ttu-id="13bed-116">Ратингаустралиателевисионтипе</span><span class="sxs-lookup"><span data-stu-id="13bed-116">ratingAustraliaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingaustraliatelevisiontype.md)|<span data-ttu-id="13bed-117">Рейтинг для телевизора выбран для Австралии.</span><span class="sxs-lookup"><span data-stu-id="13bed-117">TV rating selected for Australia.</span></span> <span data-ttu-id="13bed-118">Возможные значения: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span><span class="sxs-lookup"><span data-stu-id="13bed-118">Possible values are: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="13bed-119">Связи</span><span class="sxs-lookup"><span data-stu-id="13bed-119">Relationships</span></span>
<span data-ttu-id="13bed-120">Нет</span><span class="sxs-lookup"><span data-stu-id="13bed-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="13bed-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="13bed-121">JSON Representation</span></span>
<span data-ttu-id="13bed-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="13bed-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingAustralia"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingAustralia",
  "movieRating": "String",
  "tvRating": "String"
}
```




