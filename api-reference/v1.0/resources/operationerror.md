---
title: Тип ресурса Оператионеррор
description: Описание ошибок в Теамсасинкоператион.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 0cf550b0c15d5bd6632490d40eae04c0b4f5f3f1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447285"
---
# <a name="operationerror-resource-type"></a><span data-ttu-id="027f9-103">Тип ресурса Оператионеррор</span><span class="sxs-lookup"><span data-stu-id="027f9-103">operationError resource type</span></span>

<span data-ttu-id="027f9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="027f9-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="027f9-105">Описание ошибок в [теамсасинкоператион](teamsasyncoperation.md).</span><span class="sxs-lookup"><span data-stu-id="027f9-105">Describes errors in [teamsAsyncOperation](teamsasyncoperation.md).</span></span>

## <a name="operationerror-properties"></a><span data-ttu-id="027f9-106">Свойства Оператионеррор</span><span class="sxs-lookup"><span data-stu-id="027f9-106">operationError Properties</span></span>
| <span data-ttu-id="027f9-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="027f9-107">Property</span></span>     | <span data-ttu-id="027f9-108">Тип</span><span class="sxs-lookup"><span data-stu-id="027f9-108">Type</span></span>   |<span data-ttu-id="027f9-109">Описание</span><span class="sxs-lookup"><span data-stu-id="027f9-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="027f9-110">code</span><span class="sxs-lookup"><span data-stu-id="027f9-110">code</span></span>|<span data-ttu-id="027f9-111">string (только для чтения)</span><span class="sxs-lookup"><span data-stu-id="027f9-111">string (readonly)</span></span>|<span data-ttu-id="027f9-112">Код ошибки операции.</span><span class="sxs-lookup"><span data-stu-id="027f9-112">Operation error code.</span></span>|
|<span data-ttu-id="027f9-113">message</span><span class="sxs-lookup"><span data-stu-id="027f9-113">message</span></span>|<span data-ttu-id="027f9-114">string (только для чтения)</span><span class="sxs-lookup"><span data-stu-id="027f9-114">string (readonly)</span></span>|<span data-ttu-id="027f9-115">Сообщение об ошибке операции.</span><span class="sxs-lookup"><span data-stu-id="027f9-115">Operation error message.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="027f9-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="027f9-116">JSON representation</span></span>

<span data-ttu-id="027f9-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="027f9-117">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "operation error resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
