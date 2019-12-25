---
title: Тип ресурса Коммснотификатионс
description: Список уведомлений, используемых серверами Communications Server для отправки нескольких уведомлений в один пакет.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 4c41a8657ebc144a7247a5e40984866c71d66154
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871400"
---
# <a name="commsnotifications-resource-type"></a><span data-ttu-id="c3e46-103">Тип ресурса Коммснотификатионс</span><span class="sxs-lookup"><span data-stu-id="c3e46-103">commsNotifications resource type</span></span>

<span data-ttu-id="c3e46-104">Список уведомлений, используемых серверами Communications Server для отправки нескольких уведомлений в один пакет.</span><span class="sxs-lookup"><span data-stu-id="c3e46-104">List of notifications used by the Communications servers for sending multiple notifications in a single batch.</span></span>

## <a name="properties"></a><span data-ttu-id="c3e46-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="c3e46-105">Properties</span></span>

| <span data-ttu-id="c3e46-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="c3e46-106">Property</span></span>       | <span data-ttu-id="c3e46-107">Тип</span><span class="sxs-lookup"><span data-stu-id="c3e46-107">Type</span></span>                                                 | <span data-ttu-id="c3e46-108">Описание</span><span class="sxs-lookup"><span data-stu-id="c3e46-108">Description</span></span>                                   |
|:---------------|:-----------------------------------------------------|:----------------------------------------------|
| <span data-ttu-id="c3e46-109">значение</span><span class="sxs-lookup"><span data-stu-id="c3e46-109">value</span></span>          | <span data-ttu-id="c3e46-110">Коллекция [коммснотификатион](commsnotification.md)</span><span class="sxs-lookup"><span data-stu-id="c3e46-110">[commsNotification](commsnotification.md) collection</span></span> | <span data-ttu-id="c3e46-111">Уведомление об изменении ресурса.</span><span class="sxs-lookup"><span data-stu-id="c3e46-111">The notification of a change in the resource.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c3e46-112">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c3e46-112">JSON representation</span></span>

<span data-ttu-id="c3e46-113">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c3e46-113">The following is a JSON representation of the resource.</span></span>

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
