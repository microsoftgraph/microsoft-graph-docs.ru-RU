---
title: Тип ресурса Кондитионалакцессплатформс
description: Платформы, включенные в область политики и исключенные из нее.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 27cf8f2b6a022f4d5ca17d716b35b6f357d23471
ms.sourcegitcommit: 79988a42d91cc25bdd1c531b5f3261901d720a9a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2020
ms.locfileid: "43916797"
---
# <a name="conditionalaccessplatforms-resource-type"></a><span data-ttu-id="7ddf4-103">Тип ресурса Кондитионалакцессплатформс</span><span class="sxs-lookup"><span data-stu-id="7ddf4-103">conditionalAccessPlatforms resource type</span></span>

<span data-ttu-id="7ddf4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ddf4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7ddf4-105">Платформы, включенные в область политики и исключенные из нее.</span><span class="sxs-lookup"><span data-stu-id="7ddf4-105">Platforms included in and excluded from the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="7ddf4-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="7ddf4-106">Properties</span></span>

| <span data-ttu-id="7ddf4-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="7ddf4-107">Property</span></span>     | <span data-ttu-id="7ddf4-108">Тип</span><span class="sxs-lookup"><span data-stu-id="7ddf4-108">Type</span></span>        | <span data-ttu-id="7ddf4-109">Описание</span><span class="sxs-lookup"><span data-stu-id="7ddf4-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7ddf4-110">инклудеплатформс</span><span class="sxs-lookup"><span data-stu-id="7ddf4-110">includePlatforms</span></span>|<span data-ttu-id="7ddf4-111">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="7ddf4-111">String collection</span></span>| <span data-ttu-id="7ddf4-112">Возможные значения: `android`, `iOS`, `windows`, `windowsPhone`, `macOS`, `all`.</span><span class="sxs-lookup"><span data-stu-id="7ddf4-112">Possible values are: `android`, `iOS`, `windows`, `windowsPhone`, `macOS`, `all`.</span></span>|
|<span data-ttu-id="7ddf4-113">ексклудеплатформс</span><span class="sxs-lookup"><span data-stu-id="7ddf4-113">excludePlatforms</span></span>|<span data-ttu-id="7ddf4-114">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="7ddf4-114">String collection</span></span>| <span data-ttu-id="7ddf4-115">Возможные значения: `android`, `iOS`, `windows`, `windowsPhone`, `macOS`.</span><span class="sxs-lookup"><span data-stu-id="7ddf4-115">Possible values are: `android`, `iOS`, `windows`, `windowsPhone`, `macOS`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7ddf4-116">Связи</span><span class="sxs-lookup"><span data-stu-id="7ddf4-116">Relationships</span></span>

<span data-ttu-id="7ddf4-117">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="7ddf4-117">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7ddf4-118">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="7ddf4-118">JSON representation</span></span>

<span data-ttu-id="7ddf4-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7ddf4-119">The following is a JSON representation of the resource.</span></span>

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