---
title: Тип ресурса Стрингкэйаттрибутемаппингсаурцевалуепаир
description: Представляет собой комбинацию "ключ-значение", в которой ключ является строкой, а значение — Аттрибутемаппингсаурце.
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: dab0376441904f7ec935aa87da3b825d2a0e197d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007881"
---
# <a name="stringkeyattributemappingsourcevaluepair-resource-type"></a><span data-ttu-id="35511-103">Тип ресурса Стрингкэйаттрибутемаппингсаурцевалуепаир</span><span class="sxs-lookup"><span data-stu-id="35511-103">stringKeyAttributeMappingSourceValuePair resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="35511-104">Представляет собой комбинацию "ключ-значение", в которой ключ является строкой, а значение — [аттрибутемаппингсаурце](synchronization-attributemappingsource.md).</span><span class="sxs-lookup"><span data-stu-id="35511-104">Represents a key-value pair where the key is a string and the value is [attributeMappingSource](synchronization-attributemappingsource.md).</span></span>

## <a name="properties"></a><span data-ttu-id="35511-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="35511-105">Properties</span></span>
| <span data-ttu-id="35511-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="35511-106">Property</span></span>     | <span data-ttu-id="35511-107">Тип</span><span class="sxs-lookup"><span data-stu-id="35511-107">Type</span></span>   |<span data-ttu-id="35511-108">Описание</span><span class="sxs-lookup"><span data-stu-id="35511-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="35511-109">key</span><span class="sxs-lookup"><span data-stu-id="35511-109">key</span></span>|<span data-ttu-id="35511-110">String</span><span class="sxs-lookup"><span data-stu-id="35511-110">String</span></span>|<span data-ttu-id="35511-111">Имя параметра.</span><span class="sxs-lookup"><span data-stu-id="35511-111">The name of the parameter.</span></span>|
|<span data-ttu-id="35511-112">значение</span><span class="sxs-lookup"><span data-stu-id="35511-112">value</span></span>|[<span data-ttu-id="35511-113">Аттрибутемаппингсаурце</span><span class="sxs-lookup"><span data-stu-id="35511-113">attributeMappingSource</span></span>](synchronization-attributemappingsource.md)|<span data-ttu-id="35511-114">Значение параметра.</span><span class="sxs-lookup"><span data-stu-id="35511-114">The value of the parameter.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="35511-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="35511-115">JSON representation</span></span>

<span data-ttu-id="35511-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="35511-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.stringKeyAttributeMappingSourceValuePair"
}-->

```json
{
  "key": "String",
  "value": {"@odata.type": "microsoft.graph.attributeMappingSource"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "stringKeyAttributeMappingSourceValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
