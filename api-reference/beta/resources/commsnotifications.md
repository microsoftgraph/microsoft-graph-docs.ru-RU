---
title: Тип ресурса commsNotifications
description: Список уведомлений, используемого серверами коммуникаций для отправки нескольких уведомлений в одном пакете.
author: VinodRavichandran
ms.openlocfilehash: 052520a99081e5c09cd6e3ec3b74f74e9527d38d
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380452"
---
# <a name="commsnotifications-resource-type"></a><span data-ttu-id="d0e7e-103">Тип ресурса commsNotifications</span><span class="sxs-lookup"><span data-stu-id="d0e7e-103">commsNotifications resource type</span></span>

> <span data-ttu-id="d0e7e-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d0e7e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d0e7e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d0e7e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d0e7e-106">Список уведомлений, используемого серверами коммуникаций для отправки нескольких уведомлений в одном пакете.</span><span class="sxs-lookup"><span data-stu-id="d0e7e-106">List of notifications used by the Communications servers for sending multiple notifications in a single batch.</span></span>

## <a name="properties"></a><span data-ttu-id="d0e7e-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="d0e7e-107">Properties</span></span>

| <span data-ttu-id="d0e7e-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="d0e7e-108">Property</span></span>       | <span data-ttu-id="d0e7e-109">Тип</span><span class="sxs-lookup"><span data-stu-id="d0e7e-109">Type</span></span>                                                 | <span data-ttu-id="d0e7e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d0e7e-110">Description</span></span>                                   |
|:---------------|:-----------------------------------------------------|:----------------------------------------------|
| <span data-ttu-id="d0e7e-111">value</span><span class="sxs-lookup"><span data-stu-id="d0e7e-111">value</span></span>          | <span data-ttu-id="d0e7e-112">[commsNotification](commsnotification.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="d0e7e-112">[commsNotification](commsnotification.md) collection</span></span> | <span data-ttu-id="d0e7e-113">Уведомление об изменении в ресурсе.</span><span class="sxs-lookup"><span data-stu-id="d0e7e-113">The notification of a change in the resource.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d0e7e-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d0e7e-114">JSON representation</span></span>

<span data-ttu-id="d0e7e-115">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d0e7e-115">The following is a JSON representation of the resource.</span></span>

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
  "description": "commsNotifications resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->