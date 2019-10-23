---
title: Тип ресурса Кондитионалакцессплатформс
description: Платформы, включенные в область политики и исключенные из нее.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9de4d82cac659e73c1b4a898d6de9017c8e3e830
ms.sourcegitcommit: 3ee6a3a949be7f0a9028bde90092a10a42e0f1fc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/23/2019
ms.locfileid: "37638507"
---
# <a name="conditionalaccessplatforms-resource-type"></a><span data-ttu-id="888a7-103">Тип ресурса Кондитионалакцессплатформс</span><span class="sxs-lookup"><span data-stu-id="888a7-103">conditionalAccessPlatforms resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="888a7-104">Платформы, включенные в область политики и исключенные из нее.</span><span class="sxs-lookup"><span data-stu-id="888a7-104">Platforms included in and excluded from the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="888a7-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="888a7-105">Properties</span></span>

| <span data-ttu-id="888a7-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="888a7-106">Property</span></span>     | <span data-ttu-id="888a7-107">Тип</span><span class="sxs-lookup"><span data-stu-id="888a7-107">Type</span></span>        | <span data-ttu-id="888a7-108">Описание</span><span class="sxs-lookup"><span data-stu-id="888a7-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="888a7-109">инклудеплатформс</span><span class="sxs-lookup"><span data-stu-id="888a7-109">includePlatforms</span></span>|<span data-ttu-id="888a7-110">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="888a7-110">String collection</span></span>| <span data-ttu-id="888a7-111">Возможные значения: `android`, `iOS`, `windows`, `windowsPhone`, `macOS`, `all`.</span><span class="sxs-lookup"><span data-stu-id="888a7-111">Possible values are: `android`, `iOS`, `windows`, `windowsPhone`, `macOS`, `all`.</span></span>|
|<span data-ttu-id="888a7-112">ексклудеплатформс</span><span class="sxs-lookup"><span data-stu-id="888a7-112">excludePlatforms</span></span>|<span data-ttu-id="888a7-113">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="888a7-113">String collection</span></span>| <span data-ttu-id="888a7-114">Возможные значения: `android`, `iOS`, `windows`, `windowsPhone`, `macOS`.</span><span class="sxs-lookup"><span data-stu-id="888a7-114">Possible values are: `android`, `iOS`, `windows`, `windowsPhone`, `macOS`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="888a7-115">Связи</span><span class="sxs-lookup"><span data-stu-id="888a7-115">Relationships</span></span>

<span data-ttu-id="888a7-116">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="888a7-116">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="888a7-117">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="888a7-117">JSON representation</span></span>

<span data-ttu-id="888a7-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="888a7-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.conditionalAccessPlatforms",
  "baseType": null
}-->

```json
{
  "includePlatforms": ["String"],
  "excludePlatforms": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessPlatforms resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->