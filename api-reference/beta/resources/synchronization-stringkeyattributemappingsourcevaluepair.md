---
title: Тип ресурса Стрингкэйаттрибутемаппингсаурцевалуепаир
description: Представляет собой комбинацию "ключ-значение", в которой ключ является строкой, а значение — Аттрибутемаппингсаурце.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d70337be1a3f28e9ba30734ccc919c5459dcbd0b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48026196"
---
# <a name="stringkeyattributemappingsourcevaluepair-resource-type"></a><span data-ttu-id="4e60c-103">Тип ресурса Стрингкэйаттрибутемаппингсаурцевалуепаир</span><span class="sxs-lookup"><span data-stu-id="4e60c-103">stringKeyAttributeMappingSourceValuePair resource type</span></span>

<span data-ttu-id="4e60c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e60c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4e60c-105">Представляет собой комбинацию "ключ-значение", в которой ключ является строкой, а значение — [аттрибутемаппингсаурце](synchronization-attributemappingsource.md).</span><span class="sxs-lookup"><span data-stu-id="4e60c-105">Represents a key-value pair where the key is a string and the value is [attributeMappingSource](synchronization-attributemappingsource.md).</span></span>

## <a name="properties"></a><span data-ttu-id="4e60c-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="4e60c-106">Properties</span></span>
| <span data-ttu-id="4e60c-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="4e60c-107">Property</span></span>     | <span data-ttu-id="4e60c-108">Тип</span><span class="sxs-lookup"><span data-stu-id="4e60c-108">Type</span></span>   |<span data-ttu-id="4e60c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="4e60c-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4e60c-110">key</span><span class="sxs-lookup"><span data-stu-id="4e60c-110">key</span></span>|<span data-ttu-id="4e60c-111">String</span><span class="sxs-lookup"><span data-stu-id="4e60c-111">String</span></span>|<span data-ttu-id="4e60c-112">Имя параметра.</span><span class="sxs-lookup"><span data-stu-id="4e60c-112">The name of the parameter.</span></span>|
|<span data-ttu-id="4e60c-113">значение</span><span class="sxs-lookup"><span data-stu-id="4e60c-113">value</span></span>|[<span data-ttu-id="4e60c-114">аттрибутемаппингсаурце</span><span class="sxs-lookup"><span data-stu-id="4e60c-114">attributeMappingSource</span></span>](synchronization-attributemappingsource.md)|<span data-ttu-id="4e60c-115">Значение параметра.</span><span class="sxs-lookup"><span data-stu-id="4e60c-115">The value of the parameter.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4e60c-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4e60c-116">JSON representation</span></span>

<span data-ttu-id="4e60c-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4e60c-117">The following is a JSON representation of the resource.</span></span>

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


