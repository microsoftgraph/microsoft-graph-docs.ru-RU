---
title: Тип ресурса recipient
description: 'Представляет сведения о пользователе, который отправляет или получает событие, сообщение или запись в группе. '
ms.openlocfilehash: 7ae272d239f44c3d2f709a03438facb2f0247e49
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024971"
---
# <a name="recipient-resource-type"></a><span data-ttu-id="1d730-103">Тип ресурса recipient</span><span class="sxs-lookup"><span data-stu-id="1d730-103">recipient resource type</span></span>

<span data-ttu-id="1d730-104">Представляет сведения о пользователе, который отправляет или получает событие, сообщение или запись в группе.</span><span class="sxs-lookup"><span data-stu-id="1d730-104">Represents information about a user in the sending or receiving end of an event, message or group post.</span></span> 

## <a name="properties"></a><span data-ttu-id="1d730-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="1d730-105">Properties</span></span>
| <span data-ttu-id="1d730-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="1d730-106">Property</span></span>     | <span data-ttu-id="1d730-107">Тип</span><span class="sxs-lookup"><span data-stu-id="1d730-107">Type</span></span>   |<span data-ttu-id="1d730-108">Описание</span><span class="sxs-lookup"><span data-stu-id="1d730-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1d730-109">emailAddress</span><span class="sxs-lookup"><span data-stu-id="1d730-109">emailAddress</span></span>|[<span data-ttu-id="1d730-110">EmailAddress</span><span class="sxs-lookup"><span data-stu-id="1d730-110">EmailAddress</span></span>](emailaddress.md)|<span data-ttu-id="1d730-111">Электронный адрес получателя.</span><span class="sxs-lookup"><span data-stu-id="1d730-111">The recipient's email address.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1d730-112">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1d730-112">JSON representation</span></span>

<span data-ttu-id="1d730-113">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1d730-113">Here is a JSON representation of the resource</span></span>

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