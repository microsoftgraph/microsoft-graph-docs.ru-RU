---
title: onenoteEntityBaseModel ресурсов
description: Это базовый тип для сущности OneNote.
author: Jewan-microsoft
localization_priority: Normal
ms.openlocfilehash: 0c6a3d4916bf54eeec5856f51af87fa79e1f6e6c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27821233"
---
# <a name="onenoteentitybasemodel-resource"></a><span data-ttu-id="ca17a-103">onenoteEntityBaseModel ресурсов</span><span class="sxs-lookup"><span data-stu-id="ca17a-103">onenoteEntityBaseModel resource</span></span>

<span data-ttu-id="ca17a-104">Это базовый тип для сущности OneNote.</span><span class="sxs-lookup"><span data-stu-id="ca17a-104">This is the base type for OneNote entities.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ca17a-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ca17a-105">JSON representation</span></span>

<span data-ttu-id="ca17a-106">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ca17a-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="ca17a-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="ca17a-107">Properties</span></span>
| <span data-ttu-id="ca17a-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="ca17a-108">Property</span></span>     | <span data-ttu-id="ca17a-109">Тип</span><span class="sxs-lookup"><span data-stu-id="ca17a-109">Type</span></span>   |<span data-ttu-id="ca17a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ca17a-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ca17a-111">self</span><span class="sxs-lookup"><span data-stu-id="ca17a-111">self</span></span>|<span data-ttu-id="ca17a-112">Строка</span><span class="sxs-lookup"><span data-stu-id="ca17a-112">String</span></span>|<span data-ttu-id="ca17a-p101">Конечная точка, в которой можно получить сведения о странице. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ca17a-p101">The endpoint where you can get details about the page. Read-only.</span></span>|

<!-- uuid: bfb567de-2a2a-4b81-bf47-a55626a0c166
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
