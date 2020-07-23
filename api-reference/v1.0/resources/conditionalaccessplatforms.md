---
title: Тип ресурса Кондитионалакцессплатформс
description: Платформы, включенные в область политики и исключенные из нее.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 88d40fa1557102bc04ef9a46bba93a50097d66cd
ms.sourcegitcommit: fec7d5002dbeb8d58587c89f1b678d4a54645422
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/23/2020
ms.locfileid: "45384657"
---
# <a name="conditionalaccessplatforms-resource-type"></a><span data-ttu-id="0b7ef-103">Тип ресурса Кондитионалакцессплатформс</span><span class="sxs-lookup"><span data-stu-id="0b7ef-103">conditionalAccessPlatforms resource type</span></span>

<span data-ttu-id="0b7ef-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0b7ef-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0b7ef-105">Платформы, включенные в область политики и исключенные из нее.</span><span class="sxs-lookup"><span data-stu-id="0b7ef-105">Platforms included in and excluded from the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="0b7ef-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="0b7ef-106">Properties</span></span>

| <span data-ttu-id="0b7ef-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="0b7ef-107">Property</span></span>     | <span data-ttu-id="0b7ef-108">Тип</span><span class="sxs-lookup"><span data-stu-id="0b7ef-108">Type</span></span>        | <span data-ttu-id="0b7ef-109">Описание</span><span class="sxs-lookup"><span data-stu-id="0b7ef-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0b7ef-110">инклудеплатформс</span><span class="sxs-lookup"><span data-stu-id="0b7ef-110">includePlatforms</span></span>|<span data-ttu-id="0b7ef-111">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="0b7ef-111">String collection</span></span>| <span data-ttu-id="0b7ef-112">Возможные значения: `android`, `iOS`, `windows`, `windowsPhone`, `macOS`, `all`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="0b7ef-112">Possible values are: `android`, `iOS`, `windows`, `windowsPhone`, `macOS`, `all`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="0b7ef-113">ексклудеплатформс</span><span class="sxs-lookup"><span data-stu-id="0b7ef-113">excludePlatforms</span></span>|<span data-ttu-id="0b7ef-114">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="0b7ef-114">String collection</span></span>| <span data-ttu-id="0b7ef-115">Возможные значения: `android`, `iOS`, `windows`, `windowsPhone`, `macOS`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="0b7ef-115">Possible values are: `android`, `iOS`, `windows`, `windowsPhone`, `macOS`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0b7ef-116">Связи</span><span class="sxs-lookup"><span data-stu-id="0b7ef-116">Relationships</span></span>

<span data-ttu-id="0b7ef-117">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="0b7ef-117">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0b7ef-118">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="0b7ef-118">JSON representation</span></span>

<span data-ttu-id="0b7ef-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0b7ef-119">The following is a JSON representation of the resource.</span></span>

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
