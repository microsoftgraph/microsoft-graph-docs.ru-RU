---
title: Тип ресурса onenoteOperationError
description: Ошибка, возникшая в результате сбоя операции OneNote.
author: Jewan-microsoft
ms.openlocfilehash: e31d47f9351a050eef134cde2f6a6a8bbdf526d7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27320694"
---
# <a name="onenoteoperationerror-resource-type"></a><span data-ttu-id="f74de-103">Тип ресурса onenoteOperationError</span><span class="sxs-lookup"><span data-stu-id="f74de-103">onenoteOperationError resource type</span></span>

<span data-ttu-id="f74de-104">Ошибка, возникшая в результате сбоя операции OneNote.</span><span class="sxs-lookup"><span data-stu-id="f74de-104">An error from a failed OneNote operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f74de-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="f74de-105">JSON representation</span></span>

<span data-ttu-id="f74de-106">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f74de-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="f74de-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="f74de-107">Properties</span></span>
| <span data-ttu-id="f74de-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="f74de-108">Property</span></span>     | <span data-ttu-id="f74de-109">Тип</span><span class="sxs-lookup"><span data-stu-id="f74de-109">Type</span></span>   |<span data-ttu-id="f74de-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f74de-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f74de-111">code</span><span class="sxs-lookup"><span data-stu-id="f74de-111">code</span></span>|<span data-ttu-id="f74de-112">строка</span><span class="sxs-lookup"><span data-stu-id="f74de-112">string</span></span>|<span data-ttu-id="f74de-113">Код ошибки.</span><span class="sxs-lookup"><span data-stu-id="f74de-113">The error code.</span></span>|
|<span data-ttu-id="f74de-114">message</span><span class="sxs-lookup"><span data-stu-id="f74de-114">message</span></span>|<span data-ttu-id="f74de-115">строка</span><span class="sxs-lookup"><span data-stu-id="f74de-115">string</span></span>|<span data-ttu-id="f74de-116">Сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="f74de-116">The error message.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteOperationError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
