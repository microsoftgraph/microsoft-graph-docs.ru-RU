---
title: Тип ресурса Коммснотификатионс
description: Список уведомлений, используемых серверами Communications Server для отправки нескольких уведомлений в один пакет.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: d9e77c95c4303e02be7ac6ef91caf02e9c2d3ce6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531795"
---
# <a name="commsnotifications-resource-type"></a><span data-ttu-id="5f1e0-103">Тип ресурса Коммснотификатионс</span><span class="sxs-lookup"><span data-stu-id="5f1e0-103">commsNotifications resource type</span></span>

<span data-ttu-id="5f1e0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5f1e0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5f1e0-105">Список уведомлений, используемых серверами Communications Server для отправки нескольких уведомлений в один пакет.</span><span class="sxs-lookup"><span data-stu-id="5f1e0-105">List of notifications used by the Communications servers for sending multiple notifications in a single batch.</span></span>

## <a name="properties"></a><span data-ttu-id="5f1e0-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="5f1e0-106">Properties</span></span>

| <span data-ttu-id="5f1e0-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="5f1e0-107">Property</span></span>       | <span data-ttu-id="5f1e0-108">Тип</span><span class="sxs-lookup"><span data-stu-id="5f1e0-108">Type</span></span>                                                 | <span data-ttu-id="5f1e0-109">Описание</span><span class="sxs-lookup"><span data-stu-id="5f1e0-109">Description</span></span>                                   |
|:---------------|:-----------------------------------------------------|:----------------------------------------------|
| <span data-ttu-id="5f1e0-110">значение</span><span class="sxs-lookup"><span data-stu-id="5f1e0-110">value</span></span>          | <span data-ttu-id="5f1e0-111">Коллекция [коммснотификатион](commsnotification.md)</span><span class="sxs-lookup"><span data-stu-id="5f1e0-111">[commsNotification](commsnotification.md) collection</span></span> | <span data-ttu-id="5f1e0-112">Уведомление об изменении ресурса.</span><span class="sxs-lookup"><span data-stu-id="5f1e0-112">The notification of a change in the resource.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5f1e0-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5f1e0-113">JSON representation</span></span>

<span data-ttu-id="5f1e0-114">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5f1e0-114">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "commsNotifications resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
