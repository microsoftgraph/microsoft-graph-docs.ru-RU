---
title: Тип ресурса уведомлений
description: Ниже указано представление ресурса в формате JSON.
ms.openlocfilehash: 96246491c386971fe18184f26269d4abe3af6e6e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082500"
---
# <a name="notifications-resource-type"></a><span data-ttu-id="773c0-103">Тип ресурса уведомлений</span><span class="sxs-lookup"><span data-stu-id="773c0-103">notifications resource type</span></span>

> <span data-ttu-id="773c0-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="773c0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="773c0-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="773c0-105">Use of these APIs in production applications is not supported.</span></span>

## <a name="properties"></a><span data-ttu-id="773c0-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="773c0-106">Properties</span></span>

| <span data-ttu-id="773c0-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="773c0-107">Property</span></span>       | <span data-ttu-id="773c0-108">Тип</span><span class="sxs-lookup"><span data-stu-id="773c0-108">Type</span></span>                                       | <span data-ttu-id="773c0-109">Описание</span><span class="sxs-lookup"><span data-stu-id="773c0-109">Description</span></span> |
|:---------------|:-------------------------------------------|:------------|
| <span data-ttu-id="773c0-110">value</span><span class="sxs-lookup"><span data-stu-id="773c0-110">value</span></span>          | <span data-ttu-id="773c0-111">[уведомления](commsnotification.md) семейства сайтов</span><span class="sxs-lookup"><span data-stu-id="773c0-111">[notification](commsnotification.md) collection</span></span> | <span data-ttu-id="773c0-112">Уведомление об изменении в ресурсе.</span><span class="sxs-lookup"><span data-stu-id="773c0-112">The notification of a change in the resource.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="773c0-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="773c0-113">JSON representation</span></span>

<span data-ttu-id="773c0-114">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="773c0-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "value": [ { "@odata.type": "#microsoft.graph.commsNotification" } ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "notifications resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->