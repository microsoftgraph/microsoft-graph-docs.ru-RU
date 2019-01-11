---
title: Тип ресурса onenoteOperationError
description: Ошибка, возникшая в результате сбоя операции OneNote.
author: Jewan-microsoft
localization_priority: Normal
ms.openlocfilehash: df0bfd768d26c751a303f42e1f1123b863388faa
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837340"
---
# <a name="onenoteoperationerror-resource-type"></a><span data-ttu-id="35979-103">Тип ресурса onenoteOperationError</span><span class="sxs-lookup"><span data-stu-id="35979-103">onenoteOperationError resource type</span></span>

<span data-ttu-id="35979-104">Ошибка, возникшая в результате сбоя операции OneNote.</span><span class="sxs-lookup"><span data-stu-id="35979-104">An error from a failed OneNote operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="35979-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="35979-105">JSON representation</span></span>

<span data-ttu-id="35979-106">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="35979-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="35979-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="35979-107">Properties</span></span>
| <span data-ttu-id="35979-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="35979-108">Property</span></span>     | <span data-ttu-id="35979-109">Тип</span><span class="sxs-lookup"><span data-stu-id="35979-109">Type</span></span>   |<span data-ttu-id="35979-110">Описание</span><span class="sxs-lookup"><span data-stu-id="35979-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="35979-111">code</span><span class="sxs-lookup"><span data-stu-id="35979-111">code</span></span>|<span data-ttu-id="35979-112">строка</span><span class="sxs-lookup"><span data-stu-id="35979-112">string</span></span>|<span data-ttu-id="35979-113">Код ошибки.</span><span class="sxs-lookup"><span data-stu-id="35979-113">The error code.</span></span>|
|<span data-ttu-id="35979-114">message</span><span class="sxs-lookup"><span data-stu-id="35979-114">message</span></span>|<span data-ttu-id="35979-115">строка</span><span class="sxs-lookup"><span data-stu-id="35979-115">string</span></span>|<span data-ttu-id="35979-116">Сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="35979-116">The error message.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteOperationError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
