---
title: Тип ресурса onenoteOperationError
description: Ошибка, возникшая в результате сбоя операции OneNote.
ms.openlocfilehash: 0dab8b405c99f2931d2cc02cc915df5f805322d8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081403"
---
# <a name="onenoteoperationerror-resource-type"></a><span data-ttu-id="4e212-103">Тип ресурса onenoteOperationError</span><span class="sxs-lookup"><span data-stu-id="4e212-103">onenoteOperationError resource type</span></span>

> <span data-ttu-id="4e212-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4e212-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4e212-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e212-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4e212-106">Ошибка, возникшая в результате сбоя операции OneNote.</span><span class="sxs-lookup"><span data-stu-id="4e212-106">An error from a failed OneNote operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4e212-107">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="4e212-107">JSON representation</span></span>

<span data-ttu-id="4e212-108">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4e212-108">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="4e212-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="4e212-109">Properties</span></span>
| <span data-ttu-id="4e212-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="4e212-110">Property</span></span>     | <span data-ttu-id="4e212-111">Тип</span><span class="sxs-lookup"><span data-stu-id="4e212-111">Type</span></span>   |<span data-ttu-id="4e212-112">Описание</span><span class="sxs-lookup"><span data-stu-id="4e212-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4e212-113">code</span><span class="sxs-lookup"><span data-stu-id="4e212-113">code</span></span>|<span data-ttu-id="4e212-114">строка</span><span class="sxs-lookup"><span data-stu-id="4e212-114">string</span></span>|<span data-ttu-id="4e212-115">Код ошибки.</span><span class="sxs-lookup"><span data-stu-id="4e212-115">The error code.</span></span>|
|<span data-ttu-id="4e212-116">message</span><span class="sxs-lookup"><span data-stu-id="4e212-116">message</span></span>|<span data-ttu-id="4e212-117">строка</span><span class="sxs-lookup"><span data-stu-id="4e212-117">string</span></span>|<span data-ttu-id="4e212-118">Сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="4e212-118">The error message.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteOperationError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
