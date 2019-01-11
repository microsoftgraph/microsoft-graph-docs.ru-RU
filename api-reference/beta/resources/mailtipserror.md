---
title: Тип ресурса mailTipsError
description: Ошибка, возникающая во время действия.
localization_priority: Normal
ms.openlocfilehash: 7df13bb45471d89fdf25b4a251e441bbf2dfad9e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27865626"
---
# <a name="mailtipserror-resource-type"></a><span data-ttu-id="b2398-103">Тип ресурса mailTipsError</span><span class="sxs-lookup"><span data-stu-id="b2398-103">mailTipsError resource type</span></span>

> <span data-ttu-id="b2398-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b2398-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b2398-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2398-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b2398-106">Ошибка, возникающая во время действия.</span><span class="sxs-lookup"><span data-stu-id="b2398-106">An error that occurs during an action.</span></span>

## <a name="properties"></a><span data-ttu-id="b2398-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="b2398-107">Properties</span></span>
| <span data-ttu-id="b2398-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="b2398-108">Property</span></span>     | <span data-ttu-id="b2398-109">Тип</span><span class="sxs-lookup"><span data-stu-id="b2398-109">Type</span></span>   |<span data-ttu-id="b2398-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b2398-110">Description</span></span>|
|:-----|:-----|:-----|
| <span data-ttu-id="b2398-111">message</span><span class="sxs-lookup"><span data-stu-id="b2398-111">message</span></span> | <span data-ttu-id="b2398-112">String</span><span class="sxs-lookup"><span data-stu-id="b2398-112">String</span></span> | <span data-ttu-id="b2398-113">Сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="b2398-113">The error message.</span></span> |
| <span data-ttu-id="b2398-114">code</span><span class="sxs-lookup"><span data-stu-id="b2398-114">code</span></span> | <span data-ttu-id="b2398-115">Строка</span><span class="sxs-lookup"><span data-stu-id="b2398-115">String</span></span> | <span data-ttu-id="b2398-116">Код ошибки.</span><span class="sxs-lookup"><span data-stu-id="b2398-116">The error code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b2398-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b2398-117">JSON representation</span></span>

<span data-ttu-id="b2398-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b2398-118">Here is a JSON representation of the resource.</span></span>

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
