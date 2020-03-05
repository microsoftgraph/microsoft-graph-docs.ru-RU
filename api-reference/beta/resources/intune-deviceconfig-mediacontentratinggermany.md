---
title: Тип ресурса mediaContentRatingGermany
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d9c55acb14d9e1d184da95a343edac6b3a6dcf4b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526036"
---
# <a name="mediacontentratinggermany-resource-type"></a><span data-ttu-id="c3f9b-103">Тип ресурса mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="c3f9b-103">mediaContentRatingGermany resource type</span></span>

<span data-ttu-id="c3f9b-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c3f9b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c3f9b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3f9b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c3f9b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c3f9b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3f9b-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="c3f9b-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="c3f9b-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="c3f9b-108">Properties</span></span>
|<span data-ttu-id="c3f9b-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="c3f9b-109">Property</span></span>|<span data-ttu-id="c3f9b-110">Тип</span><span class="sxs-lookup"><span data-stu-id="c3f9b-110">Type</span></span>|<span data-ttu-id="c3f9b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c3f9b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3f9b-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="c3f9b-112">movieRating</span></span>|[<span data-ttu-id="c3f9b-113">ратингжерманимовиестипе</span><span class="sxs-lookup"><span data-stu-id="c3f9b-113">ratingGermanyMoviesType</span></span>](../resources/intune-deviceconfig-ratinggermanymoviestype.md)|<span data-ttu-id="c3f9b-114">Оценка фильмов выбрана для Германии.</span><span class="sxs-lookup"><span data-stu-id="c3f9b-114">Movies rating selected for Germany.</span></span> <span data-ttu-id="c3f9b-115">Возможные значения: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="c3f9b-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="c3f9b-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="c3f9b-116">tvRating</span></span>|[<span data-ttu-id="c3f9b-117">ратингжерманителевисионтипе</span><span class="sxs-lookup"><span data-stu-id="c3f9b-117">ratingGermanyTelevisionType</span></span>](../resources/intune-deviceconfig-ratinggermanytelevisiontype.md)|<span data-ttu-id="c3f9b-118">Рейтинг для телевизора выбран в Германии.</span><span class="sxs-lookup"><span data-stu-id="c3f9b-118">TV rating selected for Germany.</span></span> <span data-ttu-id="c3f9b-119">Возможные значения: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="c3f9b-119">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c3f9b-120">Связи</span><span class="sxs-lookup"><span data-stu-id="c3f9b-120">Relationships</span></span>
<span data-ttu-id="c3f9b-121">Нет</span><span class="sxs-lookup"><span data-stu-id="c3f9b-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c3f9b-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c3f9b-122">JSON Representation</span></span>
<span data-ttu-id="c3f9b-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c3f9b-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingGermany"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingGermany",
  "movieRating": "String",
  "tvRating": "String"
}
```



