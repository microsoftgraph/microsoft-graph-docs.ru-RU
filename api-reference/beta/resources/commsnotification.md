---
title: Тип ресурса Коммснотификатион
description: Базовый тип уведомления о связи, который публикуется серверами Communications Server для уведомления об изменениях.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 20b99493821cfb29898ff0c9517cceecba1d389c
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341379"
---
# <a name="commsnotification-resource-type"></a><span data-ttu-id="4fd1e-103">Тип ресурса Коммснотификатион</span><span class="sxs-lookup"><span data-stu-id="4fd1e-103">commsNotification resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4fd1e-104">Базовый тип уведомления о связи, который публикуется серверами Communications Server для уведомления об изменениях.</span><span class="sxs-lookup"><span data-stu-id="4fd1e-104">Communications notification base type that is published by Communications servers to notify changes.</span></span>

## <a name="properties"></a><span data-ttu-id="4fd1e-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="4fd1e-105">Properties</span></span>
| <span data-ttu-id="4fd1e-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="4fd1e-106">Property</span></span>       | <span data-ttu-id="4fd1e-107">Тип</span><span class="sxs-lookup"><span data-stu-id="4fd1e-107">Type</span></span>    | <span data-ttu-id="4fd1e-108">Описание</span><span class="sxs-lookup"><span data-stu-id="4fd1e-108">Description</span></span>                                                |
|:---------------|:--------|:-----------------------------------------------------------|
| <span data-ttu-id="4fd1e-109">changeType</span><span class="sxs-lookup"><span data-stu-id="4fd1e-109">changeType</span></span>     | <span data-ttu-id="4fd1e-110">String</span><span class="sxs-lookup"><span data-stu-id="4fd1e-110">String</span></span>  | <span data-ttu-id="4fd1e-111">Возможные значения: `created`, `updated`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="4fd1e-111">Possible values are: `created`, `updated`, `deleted`.</span></span>      |
| <span data-ttu-id="4fd1e-112">resource</span><span class="sxs-lookup"><span data-stu-id="4fd1e-112">resource</span></span>       | <span data-ttu-id="4fd1e-113">String</span><span class="sxs-lookup"><span data-stu-id="4fd1e-113">String</span></span>  | <span data-ttu-id="4fd1e-114">URI ресурса, который был изменен.</span><span class="sxs-lookup"><span data-stu-id="4fd1e-114">URI of the resource that was changed.</span></span>                      |

> <span data-ttu-id="4fd1e-115">**Примечание:** `resourceData` доступна в виде дополнительных данных.</span><span class="sxs-lookup"><span data-stu-id="4fd1e-115">**Note:** `resourceData` is available as additional data.</span></span> <span data-ttu-id="4fd1e-116">Это сущность или коллекция (сущность) в зависимости от количества изменений, упакованных в уведомление.</span><span class="sxs-lookup"><span data-stu-id="4fd1e-116">It is an entity or Collection(entity) depending on the number of changes packaged in the notification.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4fd1e-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4fd1e-117">JSON representation</span></span>

<span data-ttu-id="4fd1e-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4fd1e-118">The following is a JSON representation of the resource.</span></span>

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
