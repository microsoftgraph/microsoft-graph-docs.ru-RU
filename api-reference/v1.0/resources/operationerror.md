---
title: Тип ресурса Оператионеррор
description: Описание ошибок в Теамсасинкоператион.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 8a46943fad974c2e7a12041e9def6a8a6ad6c9a3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035716"
---
# <a name="operationerror-resource-type"></a><span data-ttu-id="83e10-103">Тип ресурса Оператионеррор</span><span class="sxs-lookup"><span data-stu-id="83e10-103">operationError resource type</span></span>



<span data-ttu-id="83e10-104">Описание ошибок в [теамсасинкоператион](teamsasyncoperation.md).</span><span class="sxs-lookup"><span data-stu-id="83e10-104">Describes errors in [teamsAsyncOperation](teamsasyncoperation.md).</span></span>

## <a name="operationerror-properties"></a><span data-ttu-id="83e10-105">Свойства Оператионеррор</span><span class="sxs-lookup"><span data-stu-id="83e10-105">operationError Properties</span></span>
| <span data-ttu-id="83e10-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="83e10-106">Property</span></span>     | <span data-ttu-id="83e10-107">Тип</span><span class="sxs-lookup"><span data-stu-id="83e10-107">Type</span></span>   |<span data-ttu-id="83e10-108">Описание</span><span class="sxs-lookup"><span data-stu-id="83e10-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="83e10-109">code</span><span class="sxs-lookup"><span data-stu-id="83e10-109">code</span></span>|<span data-ttu-id="83e10-110">string (только для чтения)</span><span class="sxs-lookup"><span data-stu-id="83e10-110">string (readonly)</span></span>|<span data-ttu-id="83e10-111">Код ошибки операции.</span><span class="sxs-lookup"><span data-stu-id="83e10-111">Operation error code.</span></span>|
|<span data-ttu-id="83e10-112">message</span><span class="sxs-lookup"><span data-stu-id="83e10-112">message</span></span>|<span data-ttu-id="83e10-113">string (только для чтения)</span><span class="sxs-lookup"><span data-stu-id="83e10-113">string (readonly)</span></span>|<span data-ttu-id="83e10-114">Сообщение об ошибке операции.</span><span class="sxs-lookup"><span data-stu-id="83e10-114">Operation error message.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="83e10-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="83e10-115">JSON representation</span></span>

<span data-ttu-id="83e10-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="83e10-116">The following is a JSON representation of the resource.</span></span>

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
