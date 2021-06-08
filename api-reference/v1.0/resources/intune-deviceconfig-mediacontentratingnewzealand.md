---
title: Тип ресурса mediaContentRatingNewZealand
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4fc7374d8e71714a5c66da1b2dc66aa5175c3e33
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760253"
---
# <a name="mediacontentratingnewzealand-resource-type"></a><span data-ttu-id="3af62-103">Тип ресурса mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="3af62-103">mediaContentRatingNewZealand resource type</span></span>

<span data-ttu-id="3af62-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3af62-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3af62-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3af62-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3af62-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="3af62-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="3af62-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="3af62-107">Properties</span></span>
|<span data-ttu-id="3af62-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="3af62-108">Property</span></span>|<span data-ttu-id="3af62-109">Тип</span><span class="sxs-lookup"><span data-stu-id="3af62-109">Type</span></span>|<span data-ttu-id="3af62-110">Описание</span><span class="sxs-lookup"><span data-stu-id="3af62-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3af62-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="3af62-111">movieRating</span></span>|[<span data-ttu-id="3af62-112">ratingNewZealandMoviesType</span><span class="sxs-lookup"><span data-stu-id="3af62-112">ratingNewZealandMoviesType</span></span>](../resources/intune-deviceconfig-ratingnewzealandmoviestype.md)|<span data-ttu-id="3af62-113">Рейтинг фильмов, выбранный для Новой Зеландии.</span><span class="sxs-lookup"><span data-stu-id="3af62-113">Movies rating selected for New Zealand.</span></span> <span data-ttu-id="3af62-114">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span><span class="sxs-lookup"><span data-stu-id="3af62-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span></span>|
|<span data-ttu-id="3af62-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="3af62-115">tvRating</span></span>|[<span data-ttu-id="3af62-116">ratingNewZealandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="3af62-116">ratingNewZealandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingnewzealandtelevisiontype.md)|<span data-ttu-id="3af62-117">Телевизионный рейтинг, выбранный для Новой Зеландии.</span><span class="sxs-lookup"><span data-stu-id="3af62-117">TV rating selected for New Zealand.</span></span> <span data-ttu-id="3af62-118">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="3af62-118">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3af62-119">Связи</span><span class="sxs-lookup"><span data-stu-id="3af62-119">Relationships</span></span>
<span data-ttu-id="3af62-120">Нет</span><span class="sxs-lookup"><span data-stu-id="3af62-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3af62-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3af62-121">JSON Representation</span></span>
<span data-ttu-id="3af62-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3af62-122">Here is a JSON representation of the resource.</span></span>
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




