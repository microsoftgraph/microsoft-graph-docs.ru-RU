---
title: Тип ресурса Коммснотификатион
description: Базовый тип уведомления о связи, который публикуется серверами Communications Server для уведомления об изменениях.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 98b261ab9a640ea23dfb942e8c2bae17b7d92989
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012945"
---
# <a name="commsnotification-resource-type"></a><span data-ttu-id="1ca5f-103">Тип ресурса Коммснотификатион</span><span class="sxs-lookup"><span data-stu-id="1ca5f-103">commsNotification resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1ca5f-104">Базовый тип уведомления о связи, который публикуется серверами Communications Server для уведомления об изменениях.</span><span class="sxs-lookup"><span data-stu-id="1ca5f-104">Communications notification base type that is published by Communications servers to notify changes.</span></span>

## <a name="properties"></a><span data-ttu-id="1ca5f-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="1ca5f-105">Properties</span></span>
| <span data-ttu-id="1ca5f-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="1ca5f-106">Property</span></span>       | <span data-ttu-id="1ca5f-107">Тип</span><span class="sxs-lookup"><span data-stu-id="1ca5f-107">Type</span></span>    | <span data-ttu-id="1ca5f-108">Описание</span><span class="sxs-lookup"><span data-stu-id="1ca5f-108">Description</span></span>                                                |
|:---------------|:--------|:-----------------------------------------------------------|
| <span data-ttu-id="1ca5f-109">changeType</span><span class="sxs-lookup"><span data-stu-id="1ca5f-109">changeType</span></span>     | <span data-ttu-id="1ca5f-110">String</span><span class="sxs-lookup"><span data-stu-id="1ca5f-110">String</span></span>  | <span data-ttu-id="1ca5f-111">Возможные значения: `created`, `updated`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="1ca5f-111">Possible values are: `created`, `updated`, `deleted`.</span></span>      |
| <span data-ttu-id="1ca5f-112">resource</span><span class="sxs-lookup"><span data-stu-id="1ca5f-112">resource</span></span>       | <span data-ttu-id="1ca5f-113">String</span><span class="sxs-lookup"><span data-stu-id="1ca5f-113">String</span></span>  | <span data-ttu-id="1ca5f-114">URI ресурса, который был изменен.</span><span class="sxs-lookup"><span data-stu-id="1ca5f-114">URI of the resource that was changed.</span></span>                      |

> <span data-ttu-id="1ca5f-115">**Примечание:** `resourceData` доступна в виде дополнительных данных.</span><span class="sxs-lookup"><span data-stu-id="1ca5f-115">**Note:** `resourceData` is available as additional data.</span></span> <span data-ttu-id="1ca5f-116">Это сущность или коллекция (сущность) в зависимости от количества изменений, упакованных в уведомление.</span><span class="sxs-lookup"><span data-stu-id="1ca5f-116">It is an entity or Collection(entity) depending on the number of changes packaged in the notification.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1ca5f-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1ca5f-117">JSON representation</span></span>

<span data-ttu-id="1ca5f-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1ca5f-118">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "commsNotification resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
