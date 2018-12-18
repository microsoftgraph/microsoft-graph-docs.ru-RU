---
title: onenoteEntityBaseModel ресурсов
description: Это базовый тип для сущности OneNote.
author: Jewan-microsoft
ms.openlocfilehash: 25e2da6732fd831c6bbec5ae86bddeae7b702aa5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27310467"
---
# <a name="onenoteentitybasemodel-resource"></a><span data-ttu-id="6720d-103">onenoteEntityBaseModel ресурсов</span><span class="sxs-lookup"><span data-stu-id="6720d-103">onenoteEntityBaseModel resource</span></span>

<span data-ttu-id="6720d-104">Это базовый тип для сущности OneNote.</span><span class="sxs-lookup"><span data-stu-id="6720d-104">This is the base type for OneNote entities.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6720d-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6720d-105">JSON representation</span></span>

<span data-ttu-id="6720d-106">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6720d-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="6720d-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="6720d-107">Properties</span></span>
| <span data-ttu-id="6720d-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="6720d-108">Property</span></span>     | <span data-ttu-id="6720d-109">Тип</span><span class="sxs-lookup"><span data-stu-id="6720d-109">Type</span></span>   |<span data-ttu-id="6720d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6720d-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6720d-111">self</span><span class="sxs-lookup"><span data-stu-id="6720d-111">self</span></span>|<span data-ttu-id="6720d-112">Строка</span><span class="sxs-lookup"><span data-stu-id="6720d-112">String</span></span>|<span data-ttu-id="6720d-p101">Конечная точка, в которой можно получить сведения о странице. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6720d-p101">The endpoint where you can get details about the page. Read-only.</span></span>|

<!-- uuid: bfb567de-2a2a-4b81-bf47-a55626a0c166
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->