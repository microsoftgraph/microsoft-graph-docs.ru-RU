---
title: Тип ресурса mediaContentRatingJapan
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 64f4a45d9fda194f18ccecc6a03102d2dfb24894
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48707187"
---
# <a name="mediacontentratingjapan-resource-type"></a><span data-ttu-id="81bd8-103">Тип ресурса mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="81bd8-103">mediaContentRatingJapan resource type</span></span>

<span data-ttu-id="81bd8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="81bd8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="81bd8-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="81bd8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="81bd8-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="81bd8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81bd8-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="81bd8-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="81bd8-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="81bd8-108">Properties</span></span>
|<span data-ttu-id="81bd8-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="81bd8-109">Property</span></span>|<span data-ttu-id="81bd8-110">Тип</span><span class="sxs-lookup"><span data-stu-id="81bd8-110">Type</span></span>|<span data-ttu-id="81bd8-111">Описание</span><span class="sxs-lookup"><span data-stu-id="81bd8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81bd8-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="81bd8-112">movieRating</span></span>|[<span data-ttu-id="81bd8-113">ратингжапанмовиестипе</span><span class="sxs-lookup"><span data-stu-id="81bd8-113">ratingJapanMoviesType</span></span>](../resources/intune-deviceconfig-ratingjapanmoviestype.md)|<span data-ttu-id="81bd8-114">Оценка фильмов выбрана для Японии.</span><span class="sxs-lookup"><span data-stu-id="81bd8-114">Movies rating selected for Japan.</span></span> <span data-ttu-id="81bd8-115">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="81bd8-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="81bd8-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="81bd8-116">tvRating</span></span>|[<span data-ttu-id="81bd8-117">ратингжапантелевисионтипе</span><span class="sxs-lookup"><span data-stu-id="81bd8-117">ratingJapanTelevisionType</span></span>](../resources/intune-deviceconfig-ratingjapantelevisiontype.md)|<span data-ttu-id="81bd8-118">Рейтинг для телевизора выбран для Японии.</span><span class="sxs-lookup"><span data-stu-id="81bd8-118">TV rating selected for Japan.</span></span> <span data-ttu-id="81bd8-119">Возможные значения: `allAllowed`, `allBlocked`, `explicitAllowed`.</span><span class="sxs-lookup"><span data-stu-id="81bd8-119">Possible values are: `allAllowed`, `allBlocked`, `explicitAllowed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="81bd8-120">Связи</span><span class="sxs-lookup"><span data-stu-id="81bd8-120">Relationships</span></span>
<span data-ttu-id="81bd8-121">Нет</span><span class="sxs-lookup"><span data-stu-id="81bd8-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="81bd8-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="81bd8-122">JSON Representation</span></span>
<span data-ttu-id="81bd8-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="81bd8-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingJapan"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingJapan",
  "movieRating": "String",
  "tvRating": "String"
}
```





