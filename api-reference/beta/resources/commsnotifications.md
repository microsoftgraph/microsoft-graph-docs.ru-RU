---
title: Тип ресурса Коммснотификатионс
description: Список уведомлений, используемых серверами Communications Server для отправки нескольких уведомлений в один пакет.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 4497e2e1ba28e7f2d0b203f8f982053c5eb8ae1f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341477"
---
# <a name="commsnotifications-resource-type"></a><span data-ttu-id="23907-103">Тип ресурса Коммснотификатионс</span><span class="sxs-lookup"><span data-stu-id="23907-103">commsNotifications resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="23907-104">Список уведомлений, используемых серверами Communications Server для отправки нескольких уведомлений в один пакет.</span><span class="sxs-lookup"><span data-stu-id="23907-104">List of notifications used by the Communications servers for sending multiple notifications in a single batch.</span></span>

## <a name="properties"></a><span data-ttu-id="23907-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="23907-105">Properties</span></span>

| <span data-ttu-id="23907-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="23907-106">Property</span></span>       | <span data-ttu-id="23907-107">Тип</span><span class="sxs-lookup"><span data-stu-id="23907-107">Type</span></span>                                                 | <span data-ttu-id="23907-108">Описание</span><span class="sxs-lookup"><span data-stu-id="23907-108">Description</span></span>                                   |
|:---------------|:-----------------------------------------------------|:----------------------------------------------|
| <span data-ttu-id="23907-109">значение</span><span class="sxs-lookup"><span data-stu-id="23907-109">value</span></span>          | <span data-ttu-id="23907-110">Коллекция [коммснотификатион](commsnotification.md)</span><span class="sxs-lookup"><span data-stu-id="23907-110">[commsNotification](commsnotification.md) collection</span></span> | <span data-ttu-id="23907-111">Уведомление об изменении ресурса.</span><span class="sxs-lookup"><span data-stu-id="23907-111">The notification of a change in the resource.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="23907-112">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="23907-112">JSON representation</span></span>

<span data-ttu-id="23907-113">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="23907-113">The following is a JSON representation of the resource.</span></span>

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
