---
title: ресурс Оненотинтитисчемаобжектмодел
description: Это базовый тип для объектов OneNote.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: 1d7f4cd1ef452acbae902c1d4f2aadaa16f69ffe
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48079034"
---
# <a name="onenoteentityschemaobjectmodel-resource"></a><span data-ttu-id="eb6bf-103">ресурс Оненотинтитисчемаобжектмодел</span><span class="sxs-lookup"><span data-stu-id="eb6bf-103">onenoteEntitySchemaObjectModel resource</span></span>

<span data-ttu-id="eb6bf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eb6bf-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="eb6bf-105">Это базовый тип для объектов OneNote.</span><span class="sxs-lookup"><span data-stu-id="eb6bf-105">This is a base type for OneNote entities.</span></span>

## <a name="json-representation"></a><span data-ttu-id="eb6bf-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="eb6bf-106">JSON representation</span></span>

<span data-ttu-id="eb6bf-107">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eb6bf-107">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "abstract": true,
  "baseType": "microsoft.graph.onenoteEntityBaseModel",
  "optionalProperties": [
    "self"
  ],
  "@odata.type": "microsoft.graph.onenoteEntitySchemaObjectModel"
}-->

```json
{
  "createdDateTime": "String (timestamp)"
}

```
## <a name="properties"></a><span data-ttu-id="eb6bf-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="eb6bf-108">Properties</span></span>
| <span data-ttu-id="eb6bf-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="eb6bf-109">Property</span></span>     | <span data-ttu-id="eb6bf-110">Тип</span><span class="sxs-lookup"><span data-stu-id="eb6bf-110">Type</span></span>   |<span data-ttu-id="eb6bf-111">Описание</span><span class="sxs-lookup"><span data-stu-id="eb6bf-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eb6bf-112">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="eb6bf-112">createdDateTime</span></span>|<span data-ttu-id="eb6bf-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eb6bf-113">DateTimeOffset</span></span>|<span data-ttu-id="eb6bf-114">Дата и время создания страницы.</span><span class="sxs-lookup"><span data-stu-id="eb6bf-114">The date and time when the page was created.</span></span> <span data-ttu-id="eb6bf-115">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="eb6bf-115">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="eb6bf-116">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="eb6bf-116">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="eb6bf-117">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="eb6bf-117">Read-only.</span></span>|

<!-- uuid: bfb567de-2a2a-4b81-bf47-a55626a0c166
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

