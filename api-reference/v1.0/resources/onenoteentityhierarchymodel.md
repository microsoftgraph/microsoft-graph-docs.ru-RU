---
title: ресурс onenoteEntityHierarchyModel
description: Это базовый тип для сущностям OneNote.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: 2ddad970ead6c8bd575267f04266426e54a66568
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720860"
---
# <a name="onenoteentityhierarchymodel-resource"></a><span data-ttu-id="d9c7d-103">ресурс onenoteEntityHierarchyModel</span><span class="sxs-lookup"><span data-stu-id="d9c7d-103">onenoteEntityHierarchyModel resource</span></span>

<span data-ttu-id="d9c7d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d9c7d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d9c7d-105">Это базовый тип для сущностям OneNote.</span><span class="sxs-lookup"><span data-stu-id="d9c7d-105">This is a base type for OneNote entities.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d9c7d-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d9c7d-106">JSON representation</span></span>

<span data-ttu-id="d9c7d-107">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d9c7d-107">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="d9c7d-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d9c7d-108">Properties</span></span>
## <a name="properties"></a><span data-ttu-id="d9c7d-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="d9c7d-109">Properties</span></span>
| <span data-ttu-id="d9c7d-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="d9c7d-110">Property</span></span>     | <span data-ttu-id="d9c7d-111">Тип</span><span class="sxs-lookup"><span data-stu-id="d9c7d-111">Type</span></span>   |<span data-ttu-id="d9c7d-112">Описание</span><span class="sxs-lookup"><span data-stu-id="d9c7d-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d9c7d-113">displayName</span><span class="sxs-lookup"><span data-stu-id="d9c7d-113">displayName</span></span>|<span data-ttu-id="d9c7d-114">String</span><span class="sxs-lookup"><span data-stu-id="d9c7d-114">String</span></span>|<span data-ttu-id="d9c7d-115">Имя записной книжки.</span><span class="sxs-lookup"><span data-stu-id="d9c7d-115">The name of the notebook.</span></span>|
|<span data-ttu-id="d9c7d-116">createdBy</span><span class="sxs-lookup"><span data-stu-id="d9c7d-116">createdBy</span></span>|[<span data-ttu-id="d9c7d-117">identitySet</span><span class="sxs-lookup"><span data-stu-id="d9c7d-117">identitySet</span></span>](identityset.md)|<span data-ttu-id="d9c7d-p101">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d9c7d-p101">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="d9c7d-120">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="d9c7d-120">lastModifiedBy</span></span>|[<span data-ttu-id="d9c7d-121">identitySet</span><span class="sxs-lookup"><span data-stu-id="d9c7d-121">identitySet</span></span>](identityset.md)|<span data-ttu-id="d9c7d-p102">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d9c7d-p102">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="d9c7d-124">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d9c7d-124">lastModifiedDateTime</span></span>|<span data-ttu-id="d9c7d-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d9c7d-125">DateTimeOffset</span></span>|<span data-ttu-id="d9c7d-126">Дата и время последнего изменения записной книжки.</span><span class="sxs-lookup"><span data-stu-id="d9c7d-126">The date and time when the notebook was last modified.</span></span> <span data-ttu-id="d9c7d-127">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="d9c7d-127">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d9c7d-128">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="d9c7d-128">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="d9c7d-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d9c7d-129">Read-only.</span></span>|

<!-- uuid: 8b1af557-1a7c-4432-86eb-94989c2d4b54
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

