---
title: Тип ресурса mediaContentRatingNewZealand
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a1866a6bf0c8d1849eb2fbf478b4f5d14fa3e5c0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27916938"
---
# <a name="mediacontentratingnewzealand-resource-type"></a><span data-ttu-id="de125-103">Тип ресурса mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="de125-103">mediaContentRatingNewZealand resource type</span></span>

> <span data-ttu-id="de125-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="de125-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="de125-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de125-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="de125-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="de125-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="de125-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="de125-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="de125-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="de125-108">Properties</span></span>
|<span data-ttu-id="de125-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="de125-109">Property</span></span>|<span data-ttu-id="de125-110">Тип</span><span class="sxs-lookup"><span data-stu-id="de125-110">Type</span></span>|<span data-ttu-id="de125-111">Описание</span><span class="sxs-lookup"><span data-stu-id="de125-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de125-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="de125-112">movieRating</span></span>|[<span data-ttu-id="de125-113">ratingNewZealandMoviesType</span><span class="sxs-lookup"><span data-stu-id="de125-113">ratingNewZealandMoviesType</span></span>](../resources/intune-deviceconfig-ratingnewzealandmoviestype.md)|<span data-ttu-id="de125-114">Оценка выбранных для новой Зеландии фильмы.</span><span class="sxs-lookup"><span data-stu-id="de125-114">Movies rating selected for New Zealand.</span></span> <span data-ttu-id="de125-115">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span><span class="sxs-lookup"><span data-stu-id="de125-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span></span>|
|<span data-ttu-id="de125-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="de125-116">tvRating</span></span>|[<span data-ttu-id="de125-117">ratingNewZealandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="de125-117">ratingNewZealandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingnewzealandtelevisiontype.md)|<span data-ttu-id="de125-118">Оценка TV, выбранной для новой Зеландии.</span><span class="sxs-lookup"><span data-stu-id="de125-118">TV rating selected for New Zealand.</span></span> <span data-ttu-id="de125-119">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="de125-119">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="de125-120">Связи</span><span class="sxs-lookup"><span data-stu-id="de125-120">Relationships</span></span>
<span data-ttu-id="de125-121">Нет</span><span class="sxs-lookup"><span data-stu-id="de125-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="de125-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="de125-122">JSON Representation</span></span>
<span data-ttu-id="de125-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="de125-123">Here is a JSON representation of the resource.</span></span>
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





