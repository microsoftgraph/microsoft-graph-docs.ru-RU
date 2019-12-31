---
title: Тип ресурса Коммснотификатионс
description: Список уведомлений, используемых серверами Communications Server для отправки нескольких уведомлений в один пакет.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: ede69277c904df28c81f7b4b7ed33393df771cf6
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913354"
---
# <a name="commsnotifications-resource-type"></a><span data-ttu-id="c5343-103">Тип ресурса Коммснотификатионс</span><span class="sxs-lookup"><span data-stu-id="c5343-103">commsNotifications resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c5343-104">Список уведомлений, используемых серверами Communications Server для отправки нескольких уведомлений в один пакет.</span><span class="sxs-lookup"><span data-stu-id="c5343-104">List of notifications used by the Communications servers for sending multiple notifications in a single batch.</span></span>

## <a name="properties"></a><span data-ttu-id="c5343-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="c5343-105">Properties</span></span>

| <span data-ttu-id="c5343-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="c5343-106">Property</span></span>       | <span data-ttu-id="c5343-107">Тип</span><span class="sxs-lookup"><span data-stu-id="c5343-107">Type</span></span>                                                 | <span data-ttu-id="c5343-108">Описание</span><span class="sxs-lookup"><span data-stu-id="c5343-108">Description</span></span>                                   |
|:---------------|:-----------------------------------------------------|:----------------------------------------------|
| <span data-ttu-id="c5343-109">значение</span><span class="sxs-lookup"><span data-stu-id="c5343-109">value</span></span>          | <span data-ttu-id="c5343-110">Коллекция [коммснотификатион](commsnotification.md)</span><span class="sxs-lookup"><span data-stu-id="c5343-110">[commsNotification](commsnotification.md) collection</span></span> | <span data-ttu-id="c5343-111">Уведомление об изменении ресурса.</span><span class="sxs-lookup"><span data-stu-id="c5343-111">The notification of a change in the resource.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c5343-112">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c5343-112">JSON representation</span></span>

<span data-ttu-id="c5343-113">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c5343-113">The following is a JSON representation of the resource.</span></span>

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
