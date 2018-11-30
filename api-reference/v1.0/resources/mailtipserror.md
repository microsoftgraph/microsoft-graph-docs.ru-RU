---
title: Тип ресурса mailTipsError
description: Ошибка, возникающая во время действия.
ms.openlocfilehash: 8604207844ade4e0c10981f30d03b33eacf4a0a2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025963"
---
# <a name="mailtipserror-resource-type"></a><span data-ttu-id="e030e-103">Тип ресурса mailTipsError</span><span class="sxs-lookup"><span data-stu-id="e030e-103">mailTipsError resource type</span></span>

<span data-ttu-id="e030e-104">Ошибка, возникающая во время действия.</span><span class="sxs-lookup"><span data-stu-id="e030e-104">An error that occurs during an action.</span></span>

## <a name="properties"></a><span data-ttu-id="e030e-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="e030e-105">Properties</span></span>
| <span data-ttu-id="e030e-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="e030e-106">Property</span></span>     | <span data-ttu-id="e030e-107">Тип</span><span class="sxs-lookup"><span data-stu-id="e030e-107">Type</span></span>   |<span data-ttu-id="e030e-108">Description</span><span class="sxs-lookup"><span data-stu-id="e030e-108">Description</span></span>|
|:-----|:-----|:-----|
| <span data-ttu-id="e030e-109">message</span><span class="sxs-lookup"><span data-stu-id="e030e-109">message</span></span> | <span data-ttu-id="e030e-110">String</span><span class="sxs-lookup"><span data-stu-id="e030e-110">String</span></span> | <span data-ttu-id="e030e-111">Сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="e030e-111">The error message.</span></span> |
| <span data-ttu-id="e030e-112">code</span><span class="sxs-lookup"><span data-stu-id="e030e-112">code</span></span> | <span data-ttu-id="e030e-113">String</span><span class="sxs-lookup"><span data-stu-id="e030e-113">String</span></span> | <span data-ttu-id="e030e-114">Код ошибки.</span><span class="sxs-lookup"><span data-stu-id="e030e-114">The error code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e030e-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e030e-115">JSON representation</span></span>

<span data-ttu-id="e030e-116">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e030e-116">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mailTipsError"
}-->

```json
{
  "message": "string",
  "code": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailTipsError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->