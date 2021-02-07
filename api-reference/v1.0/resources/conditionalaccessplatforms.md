---
title: Тип ресурса conditionalAccessPlatforms
description: Платформы, включенные в область политики и исключенные из нее.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 6d5a6d85e1341a7c742c1691a8fa126b1d5644dd
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130783"
---
# <a name="conditionalaccessplatforms-resource-type"></a><span data-ttu-id="8791f-103">Тип ресурса conditionalAccessPlatforms</span><span class="sxs-lookup"><span data-stu-id="8791f-103">conditionalAccessPlatforms resource type</span></span>

<span data-ttu-id="8791f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8791f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8791f-105">Платформы, включенные в область политики и исключенные из нее.</span><span class="sxs-lookup"><span data-stu-id="8791f-105">Platforms included in and excluded from the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="8791f-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="8791f-106">Properties</span></span>

| <span data-ttu-id="8791f-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="8791f-107">Property</span></span>     | <span data-ttu-id="8791f-108">Тип</span><span class="sxs-lookup"><span data-stu-id="8791f-108">Type</span></span>        | <span data-ttu-id="8791f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="8791f-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8791f-110">includePlatforms</span><span class="sxs-lookup"><span data-stu-id="8791f-110">includePlatforms</span></span>|<span data-ttu-id="8791f-111">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="8791f-111">String collection</span></span>| <span data-ttu-id="8791f-112">Возможные значения: `android`, `iOS`, `windows`, `windowsPhone`, `macOS`, `all`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="8791f-112">Possible values are: `android`, `iOS`, `windows`, `windowsPhone`, `macOS`, `all`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="8791f-113">excludePlatforms</span><span class="sxs-lookup"><span data-stu-id="8791f-113">excludePlatforms</span></span>|<span data-ttu-id="8791f-114">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="8791f-114">String collection</span></span>| <span data-ttu-id="8791f-115">Возможные значения: `android`, `iOS`, `windows`, `windowsPhone`, `macOS`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="8791f-115">Possible values are: `android`, `iOS`, `windows`, `windowsPhone`, `macOS`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8791f-116">Связи</span><span class="sxs-lookup"><span data-stu-id="8791f-116">Relationships</span></span>

<span data-ttu-id="8791f-117">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="8791f-117">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8791f-118">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="8791f-118">JSON representation</span></span>

<span data-ttu-id="8791f-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8791f-119">The following is a JSON representation of the resource.</span></span>

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

