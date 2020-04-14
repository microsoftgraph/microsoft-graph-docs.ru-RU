---
title: Тип ресурса mediaContentRatingNewZealand
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4eb72612c61bfe90a6c7071f8645c3471bdd5be5
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43437164"
---
# <a name="mediacontentratingnewzealand-resource-type"></a><span data-ttu-id="55b11-103">Тип ресурса mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="55b11-103">mediaContentRatingNewZealand resource type</span></span>

<span data-ttu-id="55b11-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55b11-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="55b11-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="55b11-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="55b11-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="55b11-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="55b11-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="55b11-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="55b11-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="55b11-108">Properties</span></span>
|<span data-ttu-id="55b11-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="55b11-109">Property</span></span>|<span data-ttu-id="55b11-110">Тип</span><span class="sxs-lookup"><span data-stu-id="55b11-110">Type</span></span>|<span data-ttu-id="55b11-111">Описание</span><span class="sxs-lookup"><span data-stu-id="55b11-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55b11-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="55b11-112">movieRating</span></span>|[<span data-ttu-id="55b11-113">ратингневзеаландмовиестипе</span><span class="sxs-lookup"><span data-stu-id="55b11-113">ratingNewZealandMoviesType</span></span>](../resources/intune-deviceconfig-ratingnewzealandmoviestype.md)|<span data-ttu-id="55b11-114">Рейтинг фильмов, выбранный для Новой Зеландии.</span><span class="sxs-lookup"><span data-stu-id="55b11-114">Movies rating selected for New Zealand.</span></span> <span data-ttu-id="55b11-115">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span><span class="sxs-lookup"><span data-stu-id="55b11-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span></span>|
|<span data-ttu-id="55b11-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="55b11-116">tvRating</span></span>|[<span data-ttu-id="55b11-117">ратингневзеаландтелевисионтипе</span><span class="sxs-lookup"><span data-stu-id="55b11-117">ratingNewZealandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingnewzealandtelevisiontype.md)|<span data-ttu-id="55b11-118">Рейтинг для телевизора, выбранный для Новой Зеландии.</span><span class="sxs-lookup"><span data-stu-id="55b11-118">TV rating selected for New Zealand.</span></span> <span data-ttu-id="55b11-119">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="55b11-119">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="55b11-120">Связи</span><span class="sxs-lookup"><span data-stu-id="55b11-120">Relationships</span></span>
<span data-ttu-id="55b11-121">Нет</span><span class="sxs-lookup"><span data-stu-id="55b11-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="55b11-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="55b11-122">JSON Representation</span></span>
<span data-ttu-id="55b11-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="55b11-123">Here is a JSON representation of the resource.</span></span>
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



