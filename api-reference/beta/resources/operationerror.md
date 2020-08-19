---
title: Тип ресурса Оператионеррор
description: Описание ошибок в Теамсасинкоператион.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: billbliss
ms.openlocfilehash: 2419d4230e5618f601a5d8fe0743ec9ef807cf00
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46809329"
---
# <a name="operationerror-resource-type"></a><span data-ttu-id="d3ba9-103">Тип ресурса Оператионеррор</span><span class="sxs-lookup"><span data-stu-id="d3ba9-103">operationError resource type</span></span>

<span data-ttu-id="d3ba9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3ba9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d3ba9-105">Описание ошибок в [теамсасинкоператион](teamsasyncoperation.md).</span><span class="sxs-lookup"><span data-stu-id="d3ba9-105">Describes errors in [teamsAsyncOperation](teamsasyncoperation.md).</span></span>

## <a name="operationerror-properties"></a><span data-ttu-id="d3ba9-106">Свойства Оператионеррор</span><span class="sxs-lookup"><span data-stu-id="d3ba9-106">operationError Properties</span></span>
| <span data-ttu-id="d3ba9-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="d3ba9-107">Property</span></span>     | <span data-ttu-id="d3ba9-108">Тип</span><span class="sxs-lookup"><span data-stu-id="d3ba9-108">Type</span></span>   |<span data-ttu-id="d3ba9-109">Описание</span><span class="sxs-lookup"><span data-stu-id="d3ba9-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d3ba9-110">code</span><span class="sxs-lookup"><span data-stu-id="d3ba9-110">code</span></span>|<span data-ttu-id="d3ba9-111">string (только для чтения)</span><span class="sxs-lookup"><span data-stu-id="d3ba9-111">string (readonly)</span></span>|<span data-ttu-id="d3ba9-112">Код ошибки операции.</span><span class="sxs-lookup"><span data-stu-id="d3ba9-112">Operation error code.</span></span>|
|<span data-ttu-id="d3ba9-113">message</span><span class="sxs-lookup"><span data-stu-id="d3ba9-113">message</span></span>|<span data-ttu-id="d3ba9-114">string (только для чтения)</span><span class="sxs-lookup"><span data-stu-id="d3ba9-114">string (readonly)</span></span>|<span data-ttu-id="d3ba9-115">Сообщение об ошибке операции.</span><span class="sxs-lookup"><span data-stu-id="d3ba9-115">Operation error message.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d3ba9-116">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="d3ba9-116">JSON representation</span></span>

<span data-ttu-id="d3ba9-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d3ba9-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.operationError"
}-->

```json
{
    "code": "TeamUnavailable",
    "message": "The team was not found."
}
```

<!-- uuid: 069fadaa-52db-4ced-85d5-74f7caa2c66f
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "operation error resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
