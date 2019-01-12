---
title: Тип ресурса onenoteOperationError
description: Ошибка, возникшая в результате сбоя операции OneNote.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 42f9f4777a98081a3fa18c010c301ba19a34b750
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27975507"
---
# <a name="onenoteoperationerror-resource-type"></a><span data-ttu-id="cfee5-103">Тип ресурса onenoteOperationError</span><span class="sxs-lookup"><span data-stu-id="cfee5-103">onenoteOperationError resource type</span></span>

> <span data-ttu-id="cfee5-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="cfee5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cfee5-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cfee5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cfee5-106">Ошибка, возникшая в результате сбоя операции OneNote.</span><span class="sxs-lookup"><span data-stu-id="cfee5-106">An error from a failed OneNote operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="cfee5-107">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="cfee5-107">JSON representation</span></span>

<span data-ttu-id="cfee5-108">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cfee5-108">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="cfee5-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="cfee5-109">Properties</span></span>
| <span data-ttu-id="cfee5-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="cfee5-110">Property</span></span>     | <span data-ttu-id="cfee5-111">Тип</span><span class="sxs-lookup"><span data-stu-id="cfee5-111">Type</span></span>   |<span data-ttu-id="cfee5-112">Описание</span><span class="sxs-lookup"><span data-stu-id="cfee5-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cfee5-113">code</span><span class="sxs-lookup"><span data-stu-id="cfee5-113">code</span></span>|<span data-ttu-id="cfee5-114">строка</span><span class="sxs-lookup"><span data-stu-id="cfee5-114">string</span></span>|<span data-ttu-id="cfee5-115">Код ошибки.</span><span class="sxs-lookup"><span data-stu-id="cfee5-115">The error code.</span></span>|
|<span data-ttu-id="cfee5-116">message</span><span class="sxs-lookup"><span data-stu-id="cfee5-116">message</span></span>|<span data-ttu-id="cfee5-117">строка</span><span class="sxs-lookup"><span data-stu-id="cfee5-117">string</span></span>|<span data-ttu-id="cfee5-118">Сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="cfee5-118">The error message.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteOperationError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
