---
title: Тип ресурса conditionalAccessPlatforms
description: Платформы, включенные в область политики и исключенные из нее.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 69191885dd3e21aa0ab1f7d4266a33cfe1514e34
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132358"
---
# <a name="conditionalaccessplatforms-resource-type"></a><span data-ttu-id="b1abc-103">Тип ресурса conditionalAccessPlatforms</span><span class="sxs-lookup"><span data-stu-id="b1abc-103">conditionalAccessPlatforms resource type</span></span>

<span data-ttu-id="b1abc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1abc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b1abc-105">Платформы, включенные в область политики и исключенные из нее.</span><span class="sxs-lookup"><span data-stu-id="b1abc-105">Platforms included in and excluded from the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="b1abc-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="b1abc-106">Properties</span></span>

| <span data-ttu-id="b1abc-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="b1abc-107">Property</span></span>     | <span data-ttu-id="b1abc-108">Тип</span><span class="sxs-lookup"><span data-stu-id="b1abc-108">Type</span></span>        | <span data-ttu-id="b1abc-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b1abc-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b1abc-110">includePlatforms</span><span class="sxs-lookup"><span data-stu-id="b1abc-110">includePlatforms</span></span>|<span data-ttu-id="b1abc-111">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="b1abc-111">String collection</span></span>| <span data-ttu-id="b1abc-112">Возможные значения: `android`, `iOS`, `windows`, `windowsPhone`, `macOS`, `all`.</span><span class="sxs-lookup"><span data-stu-id="b1abc-112">Possible values are: `android`, `iOS`, `windows`, `windowsPhone`, `macOS`, `all`.</span></span>|
|<span data-ttu-id="b1abc-113">excludePlatforms</span><span class="sxs-lookup"><span data-stu-id="b1abc-113">excludePlatforms</span></span>|<span data-ttu-id="b1abc-114">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="b1abc-114">String collection</span></span>| <span data-ttu-id="b1abc-115">Возможные значения: `android`, `iOS`, `windows`, `windowsPhone`, `macOS`.</span><span class="sxs-lookup"><span data-stu-id="b1abc-115">Possible values are: `android`, `iOS`, `windows`, `windowsPhone`, `macOS`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b1abc-116">Связи</span><span class="sxs-lookup"><span data-stu-id="b1abc-116">Relationships</span></span>

<span data-ttu-id="b1abc-117">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="b1abc-117">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b1abc-118">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="b1abc-118">JSON representation</span></span>

<span data-ttu-id="b1abc-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b1abc-119">The following is a JSON representation of the resource.</span></span>

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

