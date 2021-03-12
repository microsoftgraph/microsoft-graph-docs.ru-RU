---
title: ресурс onenoteEntitySchemaObjectModel
description: Это базовый тип для сущностям OneNote.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: 9dd44c3360a58195f04632b849f5cafd73490676
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722337"
---
# <a name="onenoteentityschemaobjectmodel-resource"></a><span data-ttu-id="0d81f-103">ресурс onenoteEntitySchemaObjectModel</span><span class="sxs-lookup"><span data-stu-id="0d81f-103">onenoteEntitySchemaObjectModel resource</span></span>

<span data-ttu-id="0d81f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0d81f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0d81f-105">Это базовый тип для сущностям OneNote.</span><span class="sxs-lookup"><span data-stu-id="0d81f-105">This is a base type for OneNote entities.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0d81f-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0d81f-106">JSON representation</span></span>

<span data-ttu-id="0d81f-107">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0d81f-107">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="0d81f-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="0d81f-108">Properties</span></span>
| <span data-ttu-id="0d81f-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="0d81f-109">Property</span></span>     | <span data-ttu-id="0d81f-110">Тип</span><span class="sxs-lookup"><span data-stu-id="0d81f-110">Type</span></span>   |<span data-ttu-id="0d81f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0d81f-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0d81f-112">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0d81f-112">createdDateTime</span></span>|<span data-ttu-id="0d81f-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d81f-113">DateTimeOffset</span></span>|<span data-ttu-id="0d81f-114">Дата и время создания страницы.</span><span class="sxs-lookup"><span data-stu-id="0d81f-114">The date and time when the page was created.</span></span> <span data-ttu-id="0d81f-115">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="0d81f-115">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="0d81f-116">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="0d81f-116">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="0d81f-117">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0d81f-117">Read-only.</span></span>|

<!-- uuid: bfb567de-2a2a-4b81-bf47-a55626a0c166
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

