---
title: Тип ресурса commsNotification
description: Связь уведомлений базовый тип, который был опубликован серверами коммуникаций для уведомление об изменениях.
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: 526ed88f4b1c5983a06b1830f5c0b0bb97cc874e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837151"
---
# <a name="commsnotification-resource-type"></a><span data-ttu-id="5438b-103">Тип ресурса commsNotification</span><span class="sxs-lookup"><span data-stu-id="5438b-103">commsNotification resource type</span></span>

> <span data-ttu-id="5438b-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5438b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5438b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5438b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5438b-106">Связь уведомлений базовый тип, который был опубликован серверами коммуникаций для уведомление об изменениях.</span><span class="sxs-lookup"><span data-stu-id="5438b-106">Communications notification base type that is published by Communications servers to notify changes.</span></span>

## <a name="properties"></a><span data-ttu-id="5438b-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="5438b-107">Properties</span></span>
| <span data-ttu-id="5438b-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="5438b-108">Property</span></span>       | <span data-ttu-id="5438b-109">Тип</span><span class="sxs-lookup"><span data-stu-id="5438b-109">Type</span></span>    | <span data-ttu-id="5438b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5438b-110">Description</span></span>                                                |
|:---------------|:--------|:-----------------------------------------------------------|
| <span data-ttu-id="5438b-111">changeType</span><span class="sxs-lookup"><span data-stu-id="5438b-111">changeType</span></span>     | <span data-ttu-id="5438b-112">Строка</span><span class="sxs-lookup"><span data-stu-id="5438b-112">String</span></span>  | <span data-ttu-id="5438b-113">Возможные значения: `created`, `updated`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="5438b-113">Possible values are: `created`, `updated`, `deleted`.</span></span>      |
| <span data-ttu-id="5438b-114">resource</span><span class="sxs-lookup"><span data-stu-id="5438b-114">resource</span></span>       | <span data-ttu-id="5438b-115">Строка</span><span class="sxs-lookup"><span data-stu-id="5438b-115">String</span></span>  | <span data-ttu-id="5438b-116">URI-идентификатор ресурса, который был изменен.</span><span class="sxs-lookup"><span data-stu-id="5438b-116">URI of the resource that was changed.</span></span>                      |

> <span data-ttu-id="5438b-117">**Примечание:** `resourceData` доступен в качестве дополнительных данных.</span><span class="sxs-lookup"><span data-stu-id="5438b-117">**Note:** `resourceData` is available as additional data.</span></span> <span data-ttu-id="5438b-118">Это объект или Collection(entity) в зависимости от изменений, упакованный в уведомления.</span><span class="sxs-lookup"><span data-stu-id="5438b-118">It is an entity or Collection(entity) depending on the number of changes packaged in the notification.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5438b-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5438b-119">JSON representation</span></span>

<span data-ttu-id="5438b-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5438b-120">The following is a JSON representation of the resource.</span></span>

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
  "description": "commsNotification resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
