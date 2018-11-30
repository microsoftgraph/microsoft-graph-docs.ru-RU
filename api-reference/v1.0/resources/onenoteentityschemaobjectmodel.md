---
title: onenoteEntitySchemaObjectModel ресурсов
description: Это базовый тип для сущностей OneNote.
ms.openlocfilehash: 04333a19aa1f42398040b064b462144a3636e3da
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27028037"
---
# <a name="onenoteentityschemaobjectmodel-resource"></a><span data-ttu-id="3be4d-103">onenoteEntitySchemaObjectModel ресурсов</span><span class="sxs-lookup"><span data-stu-id="3be4d-103">onenoteEntitySchemaObjectModel resource</span></span>

<span data-ttu-id="3be4d-104">Это базовый тип для сущностей OneNote.</span><span class="sxs-lookup"><span data-stu-id="3be4d-104">This is a base type for OneNote entities.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3be4d-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3be4d-105">JSON representation</span></span>

<span data-ttu-id="3be4d-106">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3be4d-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="3be4d-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="3be4d-107">Properties</span></span>
| <span data-ttu-id="3be4d-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="3be4d-108">Property</span></span>     | <span data-ttu-id="3be4d-109">Тип</span><span class="sxs-lookup"><span data-stu-id="3be4d-109">Type</span></span>   |<span data-ttu-id="3be4d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="3be4d-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3be4d-111">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3be4d-111">createdDateTime</span></span>|<span data-ttu-id="3be4d-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3be4d-112">DateTimeOffset</span></span>|<span data-ttu-id="3be4d-p101">Дата и время создания страницы. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3be4d-p101">The date and time when the page was created. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|

<!-- uuid: bfb567de-2a2a-4b81-bf47-a55626a0c166
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->