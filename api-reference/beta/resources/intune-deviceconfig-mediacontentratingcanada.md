---
title: Тип ресурса mediaContentRatingCanada
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8358946454e1a27b11fd91ab1acec6ce52d53c17
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526043"
---
# <a name="mediacontentratingcanada-resource-type"></a><span data-ttu-id="0076c-103">Тип ресурса mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="0076c-103">mediaContentRatingCanada resource type</span></span>

<span data-ttu-id="0076c-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="0076c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0076c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0076c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0076c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0076c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0076c-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="0076c-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="0076c-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="0076c-108">Properties</span></span>
|<span data-ttu-id="0076c-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="0076c-109">Property</span></span>|<span data-ttu-id="0076c-110">Тип</span><span class="sxs-lookup"><span data-stu-id="0076c-110">Type</span></span>|<span data-ttu-id="0076c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0076c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0076c-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="0076c-112">movieRating</span></span>|[<span data-ttu-id="0076c-113">ратингканадамовиестипе</span><span class="sxs-lookup"><span data-stu-id="0076c-113">ratingCanadaMoviesType</span></span>](../resources/intune-deviceconfig-ratingcanadamoviestype.md)|<span data-ttu-id="0076c-114">Оценка фильмов выбрана для Канады.</span><span class="sxs-lookup"><span data-stu-id="0076c-114">Movies rating selected for Canada.</span></span> <span data-ttu-id="0076c-115">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span><span class="sxs-lookup"><span data-stu-id="0076c-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span></span>|
|<span data-ttu-id="0076c-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="0076c-116">tvRating</span></span>|[<span data-ttu-id="0076c-117">ратингканадателевисионтипе</span><span class="sxs-lookup"><span data-stu-id="0076c-117">ratingCanadaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingcanadatelevisiontype.md)|<span data-ttu-id="0076c-118">Рейтинг для телевизора выбран для Канады.</span><span class="sxs-lookup"><span data-stu-id="0076c-118">TV rating selected for Canada.</span></span> <span data-ttu-id="0076c-119">Возможные значения: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="0076c-119">Possible values are: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0076c-120">Связи</span><span class="sxs-lookup"><span data-stu-id="0076c-120">Relationships</span></span>
<span data-ttu-id="0076c-121">Нет</span><span class="sxs-lookup"><span data-stu-id="0076c-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0076c-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0076c-122">JSON Representation</span></span>
<span data-ttu-id="0076c-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0076c-123">Here is a JSON representation of the resource.</span></span>
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



