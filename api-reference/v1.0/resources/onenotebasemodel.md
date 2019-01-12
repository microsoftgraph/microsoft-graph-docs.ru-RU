---
title: onenoteEntityBaseModel ресурсов
description: Это базовый тип для сущности OneNote.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 53ed86ae22f3ac9fccdef98e56382cd9440e71e2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923133"
---
# <a name="onenoteentitybasemodel-resource"></a><span data-ttu-id="336e4-103">onenoteEntityBaseModel ресурсов</span><span class="sxs-lookup"><span data-stu-id="336e4-103">onenoteEntityBaseModel resource</span></span>

<span data-ttu-id="336e4-104">Это базовый тип для сущности OneNote.</span><span class="sxs-lookup"><span data-stu-id="336e4-104">This is the base type for OneNote entities.</span></span>

## <a name="json-representation"></a><span data-ttu-id="336e4-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="336e4-105">JSON representation</span></span>

<span data-ttu-id="336e4-106">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="336e4-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="336e4-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="336e4-107">Properties</span></span>
| <span data-ttu-id="336e4-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="336e4-108">Property</span></span>     | <span data-ttu-id="336e4-109">Тип</span><span class="sxs-lookup"><span data-stu-id="336e4-109">Type</span></span>   |<span data-ttu-id="336e4-110">Описание</span><span class="sxs-lookup"><span data-stu-id="336e4-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="336e4-111">self</span><span class="sxs-lookup"><span data-stu-id="336e4-111">self</span></span>|<span data-ttu-id="336e4-112">Строка</span><span class="sxs-lookup"><span data-stu-id="336e4-112">String</span></span>|<span data-ttu-id="336e4-p101">Конечная точка, в которой можно получить сведения о странице. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="336e4-p101">The endpoint where you can get details about the page. Read-only.</span></span>|

<!-- uuid: bfb567de-2a2a-4b81-bf47-a55626a0c166
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
