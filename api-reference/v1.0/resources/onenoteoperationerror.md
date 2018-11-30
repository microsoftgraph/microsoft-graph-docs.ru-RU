---
title: Тип ресурса onenoteOperationError
description: Ошибка, возникшая в результате сбоя операции OneNote.
ms.openlocfilehash: 3e09bd4b4ec0a8fc36113c278ebe7cab25392ecf
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024792"
---
# <a name="onenoteoperationerror-resource-type"></a><span data-ttu-id="be35a-103">Тип ресурса onenoteOperationError</span><span class="sxs-lookup"><span data-stu-id="be35a-103">onenoteOperationError resource type</span></span>

<span data-ttu-id="be35a-104">Ошибка, возникшая в результате сбоя операции OneNote.</span><span class="sxs-lookup"><span data-stu-id="be35a-104">An error from a failed OneNote operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="be35a-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="be35a-105">JSON representation</span></span>

<span data-ttu-id="be35a-106">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="be35a-106">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteOperationError"
}-->

```json
{
  "code": "string",
  "message": "string"
}

```
## <a name="properties"></a><span data-ttu-id="be35a-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="be35a-107">Properties</span></span>
| <span data-ttu-id="be35a-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="be35a-108">Property</span></span>     | <span data-ttu-id="be35a-109">Тип</span><span class="sxs-lookup"><span data-stu-id="be35a-109">Type</span></span>   |<span data-ttu-id="be35a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="be35a-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="be35a-111">code</span><span class="sxs-lookup"><span data-stu-id="be35a-111">code</span></span>|<span data-ttu-id="be35a-112">строка</span><span class="sxs-lookup"><span data-stu-id="be35a-112">string</span></span>|<span data-ttu-id="be35a-113">Код ошибки.</span><span class="sxs-lookup"><span data-stu-id="be35a-113">The error code.</span></span>|
|<span data-ttu-id="be35a-114">message</span><span class="sxs-lookup"><span data-stu-id="be35a-114">message</span></span>|<span data-ttu-id="be35a-115">строка</span><span class="sxs-lookup"><span data-stu-id="be35a-115">string</span></span>|<span data-ttu-id="be35a-116">Сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="be35a-116">The error message.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteOperationError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
