---
title: Тип ресурса mediaContentRatingUnitedStates
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6574921d91273ebc07f31d404441c492cf71e0bf
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529604"
---
# <a name="mediacontentratingunitedstates-resource-type"></a><span data-ttu-id="4b929-103">Тип ресурса mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="4b929-103">mediaContentRatingUnitedStates resource type</span></span>

<span data-ttu-id="4b929-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="4b929-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4b929-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b929-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4b929-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4b929-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4b929-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="4b929-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="4b929-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="4b929-108">Properties</span></span>
|<span data-ttu-id="4b929-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="4b929-109">Property</span></span>|<span data-ttu-id="4b929-110">Тип</span><span class="sxs-lookup"><span data-stu-id="4b929-110">Type</span></span>|<span data-ttu-id="4b929-111">Описание</span><span class="sxs-lookup"><span data-stu-id="4b929-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b929-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="4b929-112">movieRating</span></span>|[<span data-ttu-id="4b929-113">ратингунитедстатесмовиестипе</span><span class="sxs-lookup"><span data-stu-id="4b929-113">ratingUnitedStatesMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedstatesmoviestype.md)|<span data-ttu-id="4b929-114">Оценка фильмов, выбранных для США.</span><span class="sxs-lookup"><span data-stu-id="4b929-114">Movies rating selected for United States.</span></span> <span data-ttu-id="4b929-115">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="4b929-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span></span>|
|<span data-ttu-id="4b929-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="4b929-116">tvRating</span></span>|[<span data-ttu-id="4b929-117">ратингунитедстатестелевисионтипе</span><span class="sxs-lookup"><span data-stu-id="4b929-117">ratingUnitedStatesTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedstatestelevisiontype.md)|<span data-ttu-id="4b929-118">Рейтинг для телевизора выбран для США.</span><span class="sxs-lookup"><span data-stu-id="4b929-118">TV rating selected for United States.</span></span> <span data-ttu-id="4b929-119">Возможные значения: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="4b929-119">Possible values are: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4b929-120">Связи</span><span class="sxs-lookup"><span data-stu-id="4b929-120">Relationships</span></span>
<span data-ttu-id="4b929-121">Нет</span><span class="sxs-lookup"><span data-stu-id="4b929-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4b929-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4b929-122">JSON Representation</span></span>
<span data-ttu-id="4b929-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4b929-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingUnitedStates"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingUnitedStates",
  "movieRating": "String",
  "tvRating": "String"
}
```



