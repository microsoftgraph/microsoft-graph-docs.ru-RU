---
title: Тип ресурса mediaContentRatingAustralia
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: eb1cfcafca5b369d8c68103be0795c54842d083f
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52742876"
---
# <a name="mediacontentratingaustralia-resource-type"></a><span data-ttu-id="3e9aa-103">Тип ресурса mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="3e9aa-103">mediaContentRatingAustralia resource type</span></span>

<span data-ttu-id="3e9aa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3e9aa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3e9aa-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3e9aa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3e9aa-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="3e9aa-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="3e9aa-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="3e9aa-107">Properties</span></span>
|<span data-ttu-id="3e9aa-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="3e9aa-108">Property</span></span>|<span data-ttu-id="3e9aa-109">Тип</span><span class="sxs-lookup"><span data-stu-id="3e9aa-109">Type</span></span>|<span data-ttu-id="3e9aa-110">Описание</span><span class="sxs-lookup"><span data-stu-id="3e9aa-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e9aa-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="3e9aa-111">movieRating</span></span>|[<span data-ttu-id="3e9aa-112">ratingAustraliaMoviesType</span><span class="sxs-lookup"><span data-stu-id="3e9aa-112">ratingAustraliaMoviesType</span></span>](../resources/intune-deviceconfig-ratingaustraliamoviestype.md)|<span data-ttu-id="3e9aa-113">Рейтинг фильмов, выбранный для Австралии.</span><span class="sxs-lookup"><span data-stu-id="3e9aa-113">Movies rating selected for Australia.</span></span> <span data-ttu-id="3e9aa-114">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="3e9aa-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="3e9aa-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="3e9aa-115">tvRating</span></span>|[<span data-ttu-id="3e9aa-116">ratingAustraliaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="3e9aa-116">ratingAustraliaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingaustraliatelevisiontype.md)|<span data-ttu-id="3e9aa-117">Телевизионный рейтинг, выбранный для Австралии.</span><span class="sxs-lookup"><span data-stu-id="3e9aa-117">TV rating selected for Australia.</span></span> <span data-ttu-id="3e9aa-118">Возможные значения: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span><span class="sxs-lookup"><span data-stu-id="3e9aa-118">Possible values are: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3e9aa-119">Отношения</span><span class="sxs-lookup"><span data-stu-id="3e9aa-119">Relationships</span></span>
<span data-ttu-id="3e9aa-120">Нет</span><span class="sxs-lookup"><span data-stu-id="3e9aa-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3e9aa-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3e9aa-121">JSON Representation</span></span>
<span data-ttu-id="3e9aa-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3e9aa-122">Here is a JSON representation of the resource.</span></span>
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




