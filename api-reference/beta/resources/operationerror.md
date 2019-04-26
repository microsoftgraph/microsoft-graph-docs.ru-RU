---
title: Тип ресурса Оператионеррор
description: Описание ошибок в Теамсасинкоператион.
localization_priority: Normal
ms.openlocfilehash: 1f07fe064d7bbd255f2693071c86842a34fdffa0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568915"
---
# <a name="operationerror-resource-type"></a><span data-ttu-id="95a1b-103">Тип ресурса Оператионеррор</span><span class="sxs-lookup"><span data-stu-id="95a1b-103">operationError resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="95a1b-104">Описание ошибок в [теамсасинкоператион](teamsasyncoperation.md).</span><span class="sxs-lookup"><span data-stu-id="95a1b-104">Describes errors in [teamsAsyncOperation](teamsasyncoperation.md).</span></span>

## <a name="operationerror-properties"></a><span data-ttu-id="95a1b-105">Свойства Оператионеррор</span><span class="sxs-lookup"><span data-stu-id="95a1b-105">operationError Properties</span></span>
| <span data-ttu-id="95a1b-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="95a1b-106">Property</span></span>     | <span data-ttu-id="95a1b-107">Тип</span><span class="sxs-lookup"><span data-stu-id="95a1b-107">Type</span></span>   |<span data-ttu-id="95a1b-108">Описание</span><span class="sxs-lookup"><span data-stu-id="95a1b-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="95a1b-109">code</span><span class="sxs-lookup"><span data-stu-id="95a1b-109">code</span></span>|<span data-ttu-id="95a1b-110">string (только для чтения)</span><span class="sxs-lookup"><span data-stu-id="95a1b-110">string (readonly)</span></span>|<span data-ttu-id="95a1b-111">Код ошибки операции.</span><span class="sxs-lookup"><span data-stu-id="95a1b-111">Operation error code.</span></span>|
|<span data-ttu-id="95a1b-112">message</span><span class="sxs-lookup"><span data-stu-id="95a1b-112">message</span></span>|<span data-ttu-id="95a1b-113">string (только для чтения)</span><span class="sxs-lookup"><span data-stu-id="95a1b-113">string (readonly)</span></span>|<span data-ttu-id="95a1b-114">Сообщение об ошибке операции.</span><span class="sxs-lookup"><span data-stu-id="95a1b-114">Operation error message.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="95a1b-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="95a1b-115">JSON representation</span></span>

<span data-ttu-id="95a1b-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="95a1b-116">The following is a JSON representation of the resource.</span></span>

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
