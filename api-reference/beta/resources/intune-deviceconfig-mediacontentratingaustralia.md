---
title: Тип ресурса mediaContentRatingAustralia
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f16db693a751641c1b03692f0500cd5dc6d3bfc8
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48710001"
---
# <a name="mediacontentratingaustralia-resource-type"></a><span data-ttu-id="8958f-103">Тип ресурса mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="8958f-103">mediaContentRatingAustralia resource type</span></span>

<span data-ttu-id="8958f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8958f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8958f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8958f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8958f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8958f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8958f-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="8958f-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="8958f-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="8958f-108">Properties</span></span>
|<span data-ttu-id="8958f-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="8958f-109">Property</span></span>|<span data-ttu-id="8958f-110">Тип</span><span class="sxs-lookup"><span data-stu-id="8958f-110">Type</span></span>|<span data-ttu-id="8958f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="8958f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8958f-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="8958f-112">movieRating</span></span>|[<span data-ttu-id="8958f-113">ратингаустралиамовиестипе</span><span class="sxs-lookup"><span data-stu-id="8958f-113">ratingAustraliaMoviesType</span></span>](../resources/intune-deviceconfig-ratingaustraliamoviestype.md)|<span data-ttu-id="8958f-114">Оценка фильмов выбрана для Австралии.</span><span class="sxs-lookup"><span data-stu-id="8958f-114">Movies rating selected for Australia.</span></span> <span data-ttu-id="8958f-115">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="8958f-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="8958f-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="8958f-116">tvRating</span></span>|[<span data-ttu-id="8958f-117">ратингаустралиателевисионтипе</span><span class="sxs-lookup"><span data-stu-id="8958f-117">ratingAustraliaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingaustraliatelevisiontype.md)|<span data-ttu-id="8958f-118">Рейтинг для телевизора выбран для Австралии.</span><span class="sxs-lookup"><span data-stu-id="8958f-118">TV rating selected for Australia.</span></span> <span data-ttu-id="8958f-119">Возможные значения: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span><span class="sxs-lookup"><span data-stu-id="8958f-119">Possible values are: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8958f-120">Связи</span><span class="sxs-lookup"><span data-stu-id="8958f-120">Relationships</span></span>
<span data-ttu-id="8958f-121">Нет</span><span class="sxs-lookup"><span data-stu-id="8958f-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8958f-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8958f-122">JSON Representation</span></span>
<span data-ttu-id="8958f-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8958f-123">Here is a JSON representation of the resource.</span></span>
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





