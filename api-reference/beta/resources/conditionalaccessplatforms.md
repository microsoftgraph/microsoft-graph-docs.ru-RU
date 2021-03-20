---
title: тип ресурса conditionalAccessPlatforms
description: Платформы, включенные и исключенные из области политики.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 71c8b38b59d30ce1e8e1fa1c7668c41a5d2288c2
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50945707"
---
# <a name="conditionalaccessplatforms-resource-type"></a><span data-ttu-id="f6732-103">тип ресурса conditionalAccessPlatforms</span><span class="sxs-lookup"><span data-stu-id="f6732-103">conditionalAccessPlatforms resource type</span></span>

<span data-ttu-id="f6732-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f6732-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f6732-105">Платформы, включенные и исключенные из области политики.</span><span class="sxs-lookup"><span data-stu-id="f6732-105">Platforms included in and excluded from the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="f6732-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="f6732-106">Properties</span></span>

| <span data-ttu-id="f6732-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="f6732-107">Property</span></span>     | <span data-ttu-id="f6732-108">Тип</span><span class="sxs-lookup"><span data-stu-id="f6732-108">Type</span></span>        | <span data-ttu-id="f6732-109">Описание</span><span class="sxs-lookup"><span data-stu-id="f6732-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f6732-110">includePlatforms</span><span class="sxs-lookup"><span data-stu-id="f6732-110">includePlatforms</span></span>|<span data-ttu-id="f6732-111">коллекция conditionalAccessDevicePlatform</span><span class="sxs-lookup"><span data-stu-id="f6732-111">conditionalAccessDevicePlatform collection</span></span>| <span data-ttu-id="f6732-112">Возможные значения: `android`, `iOS`, `windows`, `windowsPhone`, `macOS`, `all`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="f6732-112">Possible values are: `android`, `iOS`, `windows`, `windowsPhone`, `macOS`, `all`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="f6732-113">excludePlatforms</span><span class="sxs-lookup"><span data-stu-id="f6732-113">excludePlatforms</span></span>|<span data-ttu-id="f6732-114">коллекция conditionalAccessDevicePlatform</span><span class="sxs-lookup"><span data-stu-id="f6732-114">conditionalAccessDevicePlatform collection</span></span>| <span data-ttu-id="f6732-115">Возможные значения: `android`, `iOS`, `windows`, `windowsPhone`, `macOS`, `all`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="f6732-115">Possible values are: `android`, `iOS`, `windows`, `windowsPhone`, `macOS`, `all`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f6732-116">Связи</span><span class="sxs-lookup"><span data-stu-id="f6732-116">Relationships</span></span>

<span data-ttu-id="f6732-117">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f6732-117">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f6732-118">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="f6732-118">JSON representation</span></span>

<span data-ttu-id="f6732-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f6732-119">The following is a JSON representation of the resource.</span></span>

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

