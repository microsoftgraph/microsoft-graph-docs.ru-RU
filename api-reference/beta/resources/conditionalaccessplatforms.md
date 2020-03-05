---
title: Тип ресурса Кондитионалакцессплатформс
description: Платформы, включенные в область политики и исключенные из нее.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 2612b352f512d1177bc9137603b6ecda1ad96f66
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507536"
---
# <a name="conditionalaccessplatforms-resource-type"></a><span data-ttu-id="ee17a-103">Тип ресурса Кондитионалакцессплатформс</span><span class="sxs-lookup"><span data-stu-id="ee17a-103">conditionalAccessPlatforms resource type</span></span>

<span data-ttu-id="ee17a-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ee17a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ee17a-105">Платформы, включенные в область политики и исключенные из нее.</span><span class="sxs-lookup"><span data-stu-id="ee17a-105">Platforms included in and excluded from the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="ee17a-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="ee17a-106">Properties</span></span>

| <span data-ttu-id="ee17a-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="ee17a-107">Property</span></span>     | <span data-ttu-id="ee17a-108">Тип</span><span class="sxs-lookup"><span data-stu-id="ee17a-108">Type</span></span>        | <span data-ttu-id="ee17a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="ee17a-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ee17a-110">инклудеплатформс</span><span class="sxs-lookup"><span data-stu-id="ee17a-110">includePlatforms</span></span>|<span data-ttu-id="ee17a-111">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ee17a-111">String collection</span></span>| <span data-ttu-id="ee17a-112">Возможные значения: `android`, `iOS`, `windows`, `windowsPhone`, `macOS`, `all`.</span><span class="sxs-lookup"><span data-stu-id="ee17a-112">Possible values are: `android`, `iOS`, `windows`, `windowsPhone`, `macOS`, `all`.</span></span>|
|<span data-ttu-id="ee17a-113">ексклудеплатформс</span><span class="sxs-lookup"><span data-stu-id="ee17a-113">excludePlatforms</span></span>|<span data-ttu-id="ee17a-114">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ee17a-114">String collection</span></span>| <span data-ttu-id="ee17a-115">Возможные значения: `android`, `iOS`, `windows`, `windowsPhone`, `macOS`.</span><span class="sxs-lookup"><span data-stu-id="ee17a-115">Possible values are: `android`, `iOS`, `windows`, `windowsPhone`, `macOS`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ee17a-116">Связи</span><span class="sxs-lookup"><span data-stu-id="ee17a-116">Relationships</span></span>

<span data-ttu-id="ee17a-117">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="ee17a-117">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ee17a-118">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="ee17a-118">JSON representation</span></span>

<span data-ttu-id="ee17a-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ee17a-119">The following is a JSON representation of the resource.</span></span>

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