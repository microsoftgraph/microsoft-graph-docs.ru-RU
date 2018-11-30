---
title: onenoteEntityBaseModel ресурсов
description: Это базовый тип для сущности OneNote.
ms.openlocfilehash: 68a864437cec59d9b5f0d3e69161b49bca80231c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025938"
---
# <a name="onenoteentitybasemodel-resource"></a><span data-ttu-id="0028c-103">onenoteEntityBaseModel ресурсов</span><span class="sxs-lookup"><span data-stu-id="0028c-103">onenoteEntityBaseModel resource</span></span>

<span data-ttu-id="0028c-104">Это базовый тип для сущности OneNote.</span><span class="sxs-lookup"><span data-stu-id="0028c-104">This is the base type for OneNote entities.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0028c-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0028c-105">JSON representation</span></span>

<span data-ttu-id="0028c-106">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0028c-106">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "abstract": true,
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [
    "self"
  ],
  "@odata.type": "microsoft.graph.onenoteEntityBaseModel"
}-->

```json
{
  "self": "string"
}

```
## <a name="properties"></a><span data-ttu-id="0028c-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="0028c-107">Properties</span></span>
| <span data-ttu-id="0028c-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="0028c-108">Property</span></span>     | <span data-ttu-id="0028c-109">Тип</span><span class="sxs-lookup"><span data-stu-id="0028c-109">Type</span></span>   |<span data-ttu-id="0028c-110">Description</span><span class="sxs-lookup"><span data-stu-id="0028c-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0028c-111">self</span><span class="sxs-lookup"><span data-stu-id="0028c-111">self</span></span>|<span data-ttu-id="0028c-112">String</span><span class="sxs-lookup"><span data-stu-id="0028c-112">String</span></span>|<span data-ttu-id="0028c-p101">Конечная точка, в которой можно получить сведения о странице. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0028c-p101">The endpoint where you can get details about the page. Read-only.</span></span>|

<!-- uuid: bfb567de-2a2a-4b81-bf47-a55626a0c166
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->