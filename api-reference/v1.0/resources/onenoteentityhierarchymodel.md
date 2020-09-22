---
title: ресурс Оненотинтитихиерарчимодел
description: Это базовый тип для объектов OneNote.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: 8547839597e5f98cf0bcceef80f28814888d539e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48079027"
---
# <a name="onenoteentityhierarchymodel-resource"></a><span data-ttu-id="ba278-103">ресурс Оненотинтитихиерарчимодел</span><span class="sxs-lookup"><span data-stu-id="ba278-103">onenoteEntityHierarchyModel resource</span></span>

<span data-ttu-id="ba278-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ba278-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ba278-105">Это базовый тип для объектов OneNote.</span><span class="sxs-lookup"><span data-stu-id="ba278-105">This is a base type for OneNote entities.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ba278-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ba278-106">JSON representation</span></span>

<span data-ttu-id="ba278-107">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ba278-107">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="ba278-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="ba278-108">Properties</span></span>
## <a name="properties"></a><span data-ttu-id="ba278-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="ba278-109">Properties</span></span>
| <span data-ttu-id="ba278-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="ba278-110">Property</span></span>     | <span data-ttu-id="ba278-111">Тип</span><span class="sxs-lookup"><span data-stu-id="ba278-111">Type</span></span>   |<span data-ttu-id="ba278-112">Описание</span><span class="sxs-lookup"><span data-stu-id="ba278-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ba278-113">displayName</span><span class="sxs-lookup"><span data-stu-id="ba278-113">displayName</span></span>|<span data-ttu-id="ba278-114">Строка</span><span class="sxs-lookup"><span data-stu-id="ba278-114">String</span></span>|<span data-ttu-id="ba278-115">Имя записной книжки.</span><span class="sxs-lookup"><span data-stu-id="ba278-115">The name of the notebook.</span></span>|
|<span data-ttu-id="ba278-116">createdBy</span><span class="sxs-lookup"><span data-stu-id="ba278-116">createdBy</span></span>|[<span data-ttu-id="ba278-117">identitySet</span><span class="sxs-lookup"><span data-stu-id="ba278-117">identitySet</span></span>](identityset.md)|<span data-ttu-id="ba278-p101">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ba278-p101">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="ba278-120">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="ba278-120">lastModifiedBy</span></span>|[<span data-ttu-id="ba278-121">identitySet</span><span class="sxs-lookup"><span data-stu-id="ba278-121">identitySet</span></span>](identityset.md)|<span data-ttu-id="ba278-p102">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ba278-p102">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="ba278-124">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ba278-124">lastModifiedDateTime</span></span>|<span data-ttu-id="ba278-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ba278-125">DateTimeOffset</span></span>|<span data-ttu-id="ba278-126">Дата и время последнего изменения записной книжки.</span><span class="sxs-lookup"><span data-stu-id="ba278-126">The date and time when the notebook was last modified.</span></span> <span data-ttu-id="ba278-127">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="ba278-127">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ba278-128">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="ba278-128">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="ba278-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ba278-129">Read-only.</span></span>|

<!-- uuid: 8b1af557-1a7c-4432-86eb-94989c2d4b54
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

