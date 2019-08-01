---
title: ресурс Оненотинтитихиерарчимодел
description: Это базовый тип для объектов OneNote.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: febe87c3c57612dae06e3a34a187399e6b94c55a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035828"
---
# <a name="onenoteentityhierarchymodel-resource"></a><span data-ttu-id="1f1b5-103">ресурс Оненотинтитихиерарчимодел</span><span class="sxs-lookup"><span data-stu-id="1f1b5-103">onenoteEntityHierarchyModel resource</span></span>

<span data-ttu-id="1f1b5-104">Это базовый тип для объектов OneNote.</span><span class="sxs-lookup"><span data-stu-id="1f1b5-104">This is a base type for OneNote entities.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1f1b5-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1f1b5-105">JSON representation</span></span>

<span data-ttu-id="1f1b5-106">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1f1b5-106">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "abstract": true,
  "baseType": "microsoft.graph.onenoteEntitySchemaObjectModel",
  "optionalProperties": [
    "self"
  ],
  "@odata.type": "microsoft.graph.onenoteEntityHierarchyModel"
}-->

```json
{
  "displayName": "string",
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)"
}

```
## <a name="properties"></a><span data-ttu-id="1f1b5-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="1f1b5-107">Properties</span></span>
## <a name="properties"></a><span data-ttu-id="1f1b5-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="1f1b5-108">Properties</span></span>
| <span data-ttu-id="1f1b5-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="1f1b5-109">Property</span></span>     | <span data-ttu-id="1f1b5-110">Тип</span><span class="sxs-lookup"><span data-stu-id="1f1b5-110">Type</span></span>   |<span data-ttu-id="1f1b5-111">Описание</span><span class="sxs-lookup"><span data-stu-id="1f1b5-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1f1b5-112">displayName</span><span class="sxs-lookup"><span data-stu-id="1f1b5-112">displayName</span></span>|<span data-ttu-id="1f1b5-113">String</span><span class="sxs-lookup"><span data-stu-id="1f1b5-113">String</span></span>|<span data-ttu-id="1f1b5-114">Имя записной книжки.</span><span class="sxs-lookup"><span data-stu-id="1f1b5-114">The name of the notebook.</span></span>|
|<span data-ttu-id="1f1b5-115">createdBy</span><span class="sxs-lookup"><span data-stu-id="1f1b5-115">createdBy</span></span>|[<span data-ttu-id="1f1b5-116">identitySet</span><span class="sxs-lookup"><span data-stu-id="1f1b5-116">identitySet</span></span>](identityset.md)|<span data-ttu-id="1f1b5-p101">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1f1b5-p101">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="1f1b5-119">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="1f1b5-119">lastModifiedBy</span></span>|[<span data-ttu-id="1f1b5-120">identitySet</span><span class="sxs-lookup"><span data-stu-id="1f1b5-120">identitySet</span></span>](identityset.md)|<span data-ttu-id="1f1b5-p102">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1f1b5-p102">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="1f1b5-123">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1f1b5-123">lastModifiedDateTime</span></span>|<span data-ttu-id="1f1b5-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1f1b5-124">DateTimeOffset</span></span>|<span data-ttu-id="1f1b5-125">Дата и время последнего изменения записной книжки.</span><span class="sxs-lookup"><span data-stu-id="1f1b5-125">The date and time when the notebook was last modified.</span></span> <span data-ttu-id="1f1b5-126">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="1f1b5-126">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="1f1b5-127">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="1f1b5-127">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="1f1b5-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1f1b5-128">Read-only.</span></span>|

<!-- uuid: 8b1af557-1a7c-4432-86eb-94989c2d4b54
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
