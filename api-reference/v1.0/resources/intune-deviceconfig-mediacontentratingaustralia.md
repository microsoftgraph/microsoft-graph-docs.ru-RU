---
title: Тип ресурса mediaContentRatingAustralia
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 973c8abcbb2cc0cdc523fc4175282c523266b58c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42418155"
---
# <a name="mediacontentratingaustralia-resource-type"></a><span data-ttu-id="8d989-103">Тип ресурса mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="8d989-103">mediaContentRatingAustralia resource type</span></span>

<span data-ttu-id="8d989-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="8d989-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8d989-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8d989-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8d989-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="8d989-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="8d989-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="8d989-107">Properties</span></span>
|<span data-ttu-id="8d989-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="8d989-108">Property</span></span>|<span data-ttu-id="8d989-109">Тип</span><span class="sxs-lookup"><span data-stu-id="8d989-109">Type</span></span>|<span data-ttu-id="8d989-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8d989-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d989-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="8d989-111">movieRating</span></span>|[<span data-ttu-id="8d989-112">ратингаустралиамовиестипе</span><span class="sxs-lookup"><span data-stu-id="8d989-112">ratingAustraliaMoviesType</span></span>](../resources/intune-deviceconfig-ratingaustraliamoviestype.md)|<span data-ttu-id="8d989-113">Оценка фильмов выбрана для Австралии.</span><span class="sxs-lookup"><span data-stu-id="8d989-113">Movies rating selected for Australia.</span></span> <span data-ttu-id="8d989-114">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="8d989-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="8d989-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="8d989-115">tvRating</span></span>|[<span data-ttu-id="8d989-116">ратингаустралиателевисионтипе</span><span class="sxs-lookup"><span data-stu-id="8d989-116">ratingAustraliaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingaustraliatelevisiontype.md)|<span data-ttu-id="8d989-117">Рейтинг для телевизора выбран для Австралии.</span><span class="sxs-lookup"><span data-stu-id="8d989-117">TV rating selected for Australia.</span></span> <span data-ttu-id="8d989-118">Возможные значения: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span><span class="sxs-lookup"><span data-stu-id="8d989-118">Possible values are: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8d989-119">Связи</span><span class="sxs-lookup"><span data-stu-id="8d989-119">Relationships</span></span>
<span data-ttu-id="8d989-120">Нет</span><span class="sxs-lookup"><span data-stu-id="8d989-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8d989-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8d989-121">JSON Representation</span></span>
<span data-ttu-id="8d989-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8d989-122">Here is a JSON representation of the resource.</span></span>
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




