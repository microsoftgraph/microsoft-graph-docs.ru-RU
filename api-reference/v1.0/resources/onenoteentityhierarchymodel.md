---
title: onenoteEntityHierarchyModel ресурсов
description: Это базовый тип для сущностей OneNote.
author: Jewan-microsoft
ms.openlocfilehash: a142e9206aefbb118f21b2f1a85d00cbc4a3a315
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27362022"
---
# <a name="onenoteentityhierarchymodel-resource"></a><span data-ttu-id="667d7-103">onenoteEntityHierarchyModel ресурсов</span><span class="sxs-lookup"><span data-stu-id="667d7-103">onenoteEntityHierarchyModel resource</span></span>

<span data-ttu-id="667d7-104">Это базовый тип для сущностей OneNote.</span><span class="sxs-lookup"><span data-stu-id="667d7-104">This is a base type for OneNote entities.</span></span>

## <a name="json-representation"></a><span data-ttu-id="667d7-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="667d7-105">JSON representation</span></span>

<span data-ttu-id="667d7-106">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="667d7-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="667d7-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="667d7-107">Properties</span></span>
## <a name="properties"></a><span data-ttu-id="667d7-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="667d7-108">Properties</span></span>
| <span data-ttu-id="667d7-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="667d7-109">Property</span></span>     | <span data-ttu-id="667d7-110">Тип</span><span class="sxs-lookup"><span data-stu-id="667d7-110">Type</span></span>   |<span data-ttu-id="667d7-111">Описание</span><span class="sxs-lookup"><span data-stu-id="667d7-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="667d7-112">displayName</span><span class="sxs-lookup"><span data-stu-id="667d7-112">displayName</span></span>|<span data-ttu-id="667d7-113">Строка</span><span class="sxs-lookup"><span data-stu-id="667d7-113">String</span></span>|<span data-ttu-id="667d7-114">Имя записной книжки.</span><span class="sxs-lookup"><span data-stu-id="667d7-114">The name of the notebook.</span></span>|
|<span data-ttu-id="667d7-115">createdBy</span><span class="sxs-lookup"><span data-stu-id="667d7-115">createdBy</span></span>|[<span data-ttu-id="667d7-116">identitySet</span><span class="sxs-lookup"><span data-stu-id="667d7-116">identitySet</span></span>](identityset.md)|<span data-ttu-id="667d7-p101">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="667d7-p101">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="667d7-119">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="667d7-119">lastModifiedBy</span></span>|[<span data-ttu-id="667d7-120">identitySet</span><span class="sxs-lookup"><span data-stu-id="667d7-120">identitySet</span></span>](identityset.md)|<span data-ttu-id="667d7-p102">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="667d7-p102">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="667d7-123">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="667d7-123">lastModifiedDateTime</span></span>|<span data-ttu-id="667d7-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="667d7-124">DateTimeOffset</span></span>|<span data-ttu-id="667d7-p103">Дата и время последнего изменения записной книжки. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="667d7-p103">The date and time when the notebook was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|

<!-- uuid: 8b1af557-1a7c-4432-86eb-94989c2d4b54
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->