---
title: Тип ресурса Оператионеррор
description: Описание ошибок в Теамсасинкоператион.
localization_priority: Normal
author: billbliss
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 6ae6215d00bc573e6c8d004de743b10c0d381e43
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46808164"
---
# <a name="operationerror-resource-type"></a><span data-ttu-id="5ad83-103">Тип ресурса Оператионеррор</span><span class="sxs-lookup"><span data-stu-id="5ad83-103">operationError resource type</span></span>

<span data-ttu-id="5ad83-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5ad83-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="5ad83-105">Описание ошибок в [теамсасинкоператион](teamsasyncoperation.md).</span><span class="sxs-lookup"><span data-stu-id="5ad83-105">Describes errors in [teamsAsyncOperation](teamsasyncoperation.md).</span></span>

## <a name="operationerror-properties"></a><span data-ttu-id="5ad83-106">Свойства Оператионеррор</span><span class="sxs-lookup"><span data-stu-id="5ad83-106">operationError Properties</span></span>
| <span data-ttu-id="5ad83-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="5ad83-107">Property</span></span>     | <span data-ttu-id="5ad83-108">Тип</span><span class="sxs-lookup"><span data-stu-id="5ad83-108">Type</span></span>   |<span data-ttu-id="5ad83-109">Описание</span><span class="sxs-lookup"><span data-stu-id="5ad83-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5ad83-110">code</span><span class="sxs-lookup"><span data-stu-id="5ad83-110">code</span></span>|<span data-ttu-id="5ad83-111">string (только для чтения)</span><span class="sxs-lookup"><span data-stu-id="5ad83-111">string (readonly)</span></span>|<span data-ttu-id="5ad83-112">Код ошибки операции.</span><span class="sxs-lookup"><span data-stu-id="5ad83-112">Operation error code.</span></span>|
|<span data-ttu-id="5ad83-113">message</span><span class="sxs-lookup"><span data-stu-id="5ad83-113">message</span></span>|<span data-ttu-id="5ad83-114">string (только для чтения)</span><span class="sxs-lookup"><span data-stu-id="5ad83-114">string (readonly)</span></span>|<span data-ttu-id="5ad83-115">Сообщение об ошибке операции.</span><span class="sxs-lookup"><span data-stu-id="5ad83-115">Operation error message.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5ad83-116">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="5ad83-116">JSON representation</span></span>

<span data-ttu-id="5ad83-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5ad83-117">The following is a JSON representation of the resource.</span></span>

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
