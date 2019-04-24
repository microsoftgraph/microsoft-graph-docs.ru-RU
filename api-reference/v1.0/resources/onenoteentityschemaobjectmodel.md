---
title: ресурс Оненотинтитисчемаобжектмодел
description: Это базовый тип для объектов OneNote.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 168359bbdaa659db461aa33af96e402a4a81783d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462594"
---
# <a name="onenoteentityschemaobjectmodel-resource"></a><span data-ttu-id="9d30a-103">ресурс Оненотинтитисчемаобжектмодел</span><span class="sxs-lookup"><span data-stu-id="9d30a-103">onenoteEntitySchemaObjectModel resource</span></span>

<span data-ttu-id="9d30a-104">Это базовый тип для объектов OneNote.</span><span class="sxs-lookup"><span data-stu-id="9d30a-104">This is a base type for OneNote entities.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9d30a-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9d30a-105">JSON representation</span></span>

<span data-ttu-id="9d30a-106">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9d30a-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="9d30a-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="9d30a-107">Properties</span></span>
| <span data-ttu-id="9d30a-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="9d30a-108">Property</span></span>     | <span data-ttu-id="9d30a-109">Тип</span><span class="sxs-lookup"><span data-stu-id="9d30a-109">Type</span></span>   |<span data-ttu-id="9d30a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="9d30a-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9d30a-111">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9d30a-111">createdDateTime</span></span>|<span data-ttu-id="9d30a-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9d30a-112">DateTimeOffset</span></span>|<span data-ttu-id="9d30a-113">Дата и время создания страницы.</span><span class="sxs-lookup"><span data-stu-id="9d30a-113">The date and time when the page was created.</span></span> <span data-ttu-id="9d30a-114">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="9d30a-114">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="9d30a-115">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="9d30a-115">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="9d30a-116">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9d30a-116">Read-only.</span></span>|

<!-- uuid: bfb567de-2a2a-4b81-bf47-a55626a0c166
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
