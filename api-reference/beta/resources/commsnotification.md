---
title: Тип ресурса уведомлений
description: Ниже указано представление ресурса в формате JSON.
ms.openlocfilehash: c09927cbe133c945b83a3bfc1b0eb74ef00bce2b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081265"
---
# <a name="notification-resource-type"></a><span data-ttu-id="c5af6-103">Тип ресурса уведомлений</span><span class="sxs-lookup"><span data-stu-id="c5af6-103">notification resource type</span></span>

> <span data-ttu-id="c5af6-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c5af6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c5af6-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5af6-105">Use of these APIs in production applications is not supported.</span></span>

## <a name="properties"></a><span data-ttu-id="c5af6-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="c5af6-106">Properties</span></span>
| <span data-ttu-id="c5af6-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="c5af6-107">Property</span></span>       | <span data-ttu-id="c5af6-108">Тип</span><span class="sxs-lookup"><span data-stu-id="c5af6-108">Type</span></span>    | <span data-ttu-id="c5af6-109">Описание</span><span class="sxs-lookup"><span data-stu-id="c5af6-109">Description</span></span>                                                |
|:---------------|:--------|:-----------------------------------------------------------|
| <span data-ttu-id="c5af6-110">changeType</span><span class="sxs-lookup"><span data-stu-id="c5af6-110">changeType</span></span>     | <span data-ttu-id="c5af6-111">String</span><span class="sxs-lookup"><span data-stu-id="c5af6-111">String</span></span>  | <span data-ttu-id="c5af6-112">Возможные значения: `created`, `updated`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="c5af6-112">Possible values are: `created`, `updated`, `deleted`.</span></span>      |
| <span data-ttu-id="c5af6-113">resource</span><span class="sxs-lookup"><span data-stu-id="c5af6-113">resource</span></span>       | <span data-ttu-id="c5af6-114">String</span><span class="sxs-lookup"><span data-stu-id="c5af6-114">String</span></span>  | <span data-ttu-id="c5af6-115">URI-идентификатор ресурса, который был изменен.</span><span class="sxs-lookup"><span data-stu-id="c5af6-115">URI of the resource that was changed.</span></span>                      |

> <span data-ttu-id="c5af6-116">**Примечание:** `resourceData` доступен в качестве дополнительных данных.</span><span class="sxs-lookup"><span data-stu-id="c5af6-116">**Note:** `resourceData` is available as additional data.</span></span> <span data-ttu-id="c5af6-117">Это объект или Collection(entity) в зависимости от изменений, упакованный в уведомления.</span><span class="sxs-lookup"><span data-stu-id="c5af6-117">It is an entity or Collection(entity) depending on the number of changes packaged in the notification.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c5af6-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c5af6-118">JSON representation</span></span>

<span data-ttu-id="c5af6-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c5af6-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "resourceData"
  ],
  "@odata.type": "microsoft.graph.commsNotification",
  "openType": true
}-->
```json
{
  "changeType": "created | updated | deleted",
  "resource": "String"
}
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications",
  "truncated": true
}-->
```json
{
  "value": [
    {
      "changeType": "created",
      "resource": "/app/calls/1D6DE2D4-CD51-4309-8DAA-70768651088E",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "id": "1D6DE2D4-CD51-4309-8DAA-70768651088E",
        "state": "incoming"
      }
    }
  ]
}
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications",
  "truncated": true
}-->
```json
{
  "value": [
    {
      "changeType": "created",
      "resource": "/app/calls/1D6DE2D4-CD51-4309-8DAA-70768651088E/participants",
      "resourceData": [
        {
          "@odata.type": "#microsoft.graph.participant",
          "id": "1D6DE2D4-CD51-4309-8DAA-70768651088E"
        },
        {
          "@odata.type": "#microsoft.graph.participant",
          "id": "8fcb5dbc-d5aa-4681-8e31-b001d5168d79"
        }
      ]
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "notification resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->