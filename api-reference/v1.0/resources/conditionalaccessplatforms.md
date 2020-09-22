---
title: Тип ресурса Кондитионалакцессплатформс
description: Платформы, включенные в область политики и исключенные из нее.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: dc421f5527833cfd3193243b6ddb8b94c54a0855
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48018864"
---
# <a name="conditionalaccessplatforms-resource-type"></a><span data-ttu-id="a9fb1-103">Тип ресурса Кондитионалакцессплатформс</span><span class="sxs-lookup"><span data-stu-id="a9fb1-103">conditionalAccessPlatforms resource type</span></span>

<span data-ttu-id="a9fb1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a9fb1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a9fb1-105">Платформы, включенные в область политики и исключенные из нее.</span><span class="sxs-lookup"><span data-stu-id="a9fb1-105">Platforms included in and excluded from the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="a9fb1-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="a9fb1-106">Properties</span></span>

| <span data-ttu-id="a9fb1-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="a9fb1-107">Property</span></span>     | <span data-ttu-id="a9fb1-108">Тип</span><span class="sxs-lookup"><span data-stu-id="a9fb1-108">Type</span></span>        | <span data-ttu-id="a9fb1-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a9fb1-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a9fb1-110">инклудеплатформс</span><span class="sxs-lookup"><span data-stu-id="a9fb1-110">includePlatforms</span></span>|<span data-ttu-id="a9fb1-111">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a9fb1-111">String collection</span></span>| <span data-ttu-id="a9fb1-112">Возможные значения: `android`, `iOS`, `windows`, `windowsPhone`, `macOS`, `all`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="a9fb1-112">Possible values are: `android`, `iOS`, `windows`, `windowsPhone`, `macOS`, `all`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="a9fb1-113">ексклудеплатформс</span><span class="sxs-lookup"><span data-stu-id="a9fb1-113">excludePlatforms</span></span>|<span data-ttu-id="a9fb1-114">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a9fb1-114">String collection</span></span>| <span data-ttu-id="a9fb1-115">Возможные значения: `android`, `iOS`, `windows`, `windowsPhone`, `macOS`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="a9fb1-115">Possible values are: `android`, `iOS`, `windows`, `windowsPhone`, `macOS`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a9fb1-116">Связи</span><span class="sxs-lookup"><span data-stu-id="a9fb1-116">Relationships</span></span>

<span data-ttu-id="a9fb1-117">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="a9fb1-117">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a9fb1-118">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="a9fb1-118">JSON representation</span></span>

<span data-ttu-id="a9fb1-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a9fb1-119">The following is a JSON representation of the resource.</span></span>

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

