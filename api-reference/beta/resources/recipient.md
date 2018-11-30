---
title: Тип ресурса recipient
description: 'Представляет сведения о пользователе, который отправляет или получает событие, сообщение или запись в группе. '
ms.openlocfilehash: 2ecf92f314c8b29da529b8dc07cada71dd8571f2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080551"
---
# <a name="recipient-resource-type"></a><span data-ttu-id="ed103-103">Тип ресурса recipient</span><span class="sxs-lookup"><span data-stu-id="ed103-103">recipient resource type</span></span>

> <span data-ttu-id="ed103-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ed103-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ed103-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ed103-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ed103-106">Представляет сведения о пользователе, который отправляет или получает событие, сообщение или запись в группе.</span><span class="sxs-lookup"><span data-stu-id="ed103-106">Represents information about a user in the sending or receiving end of an event, message or group post.</span></span> 

## <a name="properties"></a><span data-ttu-id="ed103-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="ed103-107">Properties</span></span>
| <span data-ttu-id="ed103-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="ed103-108">Property</span></span>     | <span data-ttu-id="ed103-109">Тип</span><span class="sxs-lookup"><span data-stu-id="ed103-109">Type</span></span>   |<span data-ttu-id="ed103-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ed103-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ed103-111">emailAddress</span><span class="sxs-lookup"><span data-stu-id="ed103-111">emailAddress</span></span>|[<span data-ttu-id="ed103-112">EmailAddress</span><span class="sxs-lookup"><span data-stu-id="ed103-112">EmailAddress</span></span>](emailaddress.md)|<span data-ttu-id="ed103-113">Электронный адрес получателя.</span><span class="sxs-lookup"><span data-stu-id="ed103-113">The recipient's email address.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ed103-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ed103-114">JSON representation</span></span>

<span data-ttu-id="ed103-115">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ed103-115">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recipient"
}-->

```json
{
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "recipient resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->