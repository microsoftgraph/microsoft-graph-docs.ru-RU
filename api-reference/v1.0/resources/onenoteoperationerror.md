---
title: Тип ресурса onenoteOperationError
description: Ошибка, возникшая в результате сбоя операции OneNote.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 3291f70e8cc18ee532f636feb1de9e8bb5751e02
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27932464"
---
# <a name="onenoteoperationerror-resource-type"></a><span data-ttu-id="c99ca-103">Тип ресурса onenoteOperationError</span><span class="sxs-lookup"><span data-stu-id="c99ca-103">onenoteOperationError resource type</span></span>

<span data-ttu-id="c99ca-104">Ошибка, возникшая в результате сбоя операции OneNote.</span><span class="sxs-lookup"><span data-stu-id="c99ca-104">An error from a failed OneNote operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c99ca-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="c99ca-105">JSON representation</span></span>

<span data-ttu-id="c99ca-106">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c99ca-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="c99ca-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="c99ca-107">Properties</span></span>
| <span data-ttu-id="c99ca-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="c99ca-108">Property</span></span>     | <span data-ttu-id="c99ca-109">Тип</span><span class="sxs-lookup"><span data-stu-id="c99ca-109">Type</span></span>   |<span data-ttu-id="c99ca-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c99ca-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c99ca-111">code</span><span class="sxs-lookup"><span data-stu-id="c99ca-111">code</span></span>|<span data-ttu-id="c99ca-112">строка</span><span class="sxs-lookup"><span data-stu-id="c99ca-112">string</span></span>|<span data-ttu-id="c99ca-113">Код ошибки.</span><span class="sxs-lookup"><span data-stu-id="c99ca-113">The error code.</span></span>|
|<span data-ttu-id="c99ca-114">message</span><span class="sxs-lookup"><span data-stu-id="c99ca-114">message</span></span>|<span data-ttu-id="c99ca-115">строка</span><span class="sxs-lookup"><span data-stu-id="c99ca-115">string</span></span>|<span data-ttu-id="c99ca-116">Сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="c99ca-116">The error message.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteOperationError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
