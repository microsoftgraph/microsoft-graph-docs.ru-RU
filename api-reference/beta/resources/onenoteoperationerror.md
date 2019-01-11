---
title: Тип ресурса onenoteOperationError
description: Ошибка, возникшая в результате сбоя операции OneNote.
author: Jewan-microsoft
localization_priority: Normal
ms.openlocfilehash: cfe859bea40f15311a631e8b1d2b3c3a3c179d0c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27891534"
---
# <a name="onenoteoperationerror-resource-type"></a><span data-ttu-id="25f0c-103">Тип ресурса onenoteOperationError</span><span class="sxs-lookup"><span data-stu-id="25f0c-103">onenoteOperationError resource type</span></span>

> <span data-ttu-id="25f0c-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="25f0c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="25f0c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="25f0c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="25f0c-106">Ошибка, возникшая в результате сбоя операции OneNote.</span><span class="sxs-lookup"><span data-stu-id="25f0c-106">An error from a failed OneNote operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="25f0c-107">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="25f0c-107">JSON representation</span></span>

<span data-ttu-id="25f0c-108">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="25f0c-108">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="25f0c-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="25f0c-109">Properties</span></span>
| <span data-ttu-id="25f0c-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="25f0c-110">Property</span></span>     | <span data-ttu-id="25f0c-111">Тип</span><span class="sxs-lookup"><span data-stu-id="25f0c-111">Type</span></span>   |<span data-ttu-id="25f0c-112">Описание</span><span class="sxs-lookup"><span data-stu-id="25f0c-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="25f0c-113">code</span><span class="sxs-lookup"><span data-stu-id="25f0c-113">code</span></span>|<span data-ttu-id="25f0c-114">строка</span><span class="sxs-lookup"><span data-stu-id="25f0c-114">string</span></span>|<span data-ttu-id="25f0c-115">Код ошибки.</span><span class="sxs-lookup"><span data-stu-id="25f0c-115">The error code.</span></span>|
|<span data-ttu-id="25f0c-116">message</span><span class="sxs-lookup"><span data-stu-id="25f0c-116">message</span></span>|<span data-ttu-id="25f0c-117">строка</span><span class="sxs-lookup"><span data-stu-id="25f0c-117">string</span></span>|<span data-ttu-id="25f0c-118">Сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="25f0c-118">The error message.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteOperationError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
