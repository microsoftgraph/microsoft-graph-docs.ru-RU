---
title: Тип ресурса Коммснотификатионс
description: Список уведомлений, используемых серверами Communications Server для отправки нескольких уведомлений в один пакет.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 750c0d0a19e4ec8bbf99a95235573d67d87701ed
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48033961"
---
# <a name="commsnotifications-resource-type"></a><span data-ttu-id="c9fec-103">Тип ресурса Коммснотификатионс</span><span class="sxs-lookup"><span data-stu-id="c9fec-103">commsNotifications resource type</span></span>

<span data-ttu-id="c9fec-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c9fec-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c9fec-105">Список уведомлений, используемых серверами Communications Server для отправки нескольких уведомлений в один пакет.</span><span class="sxs-lookup"><span data-stu-id="c9fec-105">List of notifications used by the Communications servers for sending multiple notifications in a single batch.</span></span>

## <a name="properties"></a><span data-ttu-id="c9fec-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="c9fec-106">Properties</span></span>

| <span data-ttu-id="c9fec-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="c9fec-107">Property</span></span>       | <span data-ttu-id="c9fec-108">Тип</span><span class="sxs-lookup"><span data-stu-id="c9fec-108">Type</span></span>                                                 | <span data-ttu-id="c9fec-109">Описание</span><span class="sxs-lookup"><span data-stu-id="c9fec-109">Description</span></span>                                   |
|:---------------|:-----------------------------------------------------|:----------------------------------------------|
| <span data-ttu-id="c9fec-110">значение</span><span class="sxs-lookup"><span data-stu-id="c9fec-110">value</span></span>          | <span data-ttu-id="c9fec-111">Коллекция [коммснотификатион](commsnotification.md)</span><span class="sxs-lookup"><span data-stu-id="c9fec-111">[commsNotification](commsnotification.md) collection</span></span> | <span data-ttu-id="c9fec-112">Уведомление об изменении ресурса.</span><span class="sxs-lookup"><span data-stu-id="c9fec-112">The notification of a change in the resource.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c9fec-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c9fec-113">JSON representation</span></span>

<span data-ttu-id="c9fec-114">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c9fec-114">The following is a JSON representation of the resource.</span></span>

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


