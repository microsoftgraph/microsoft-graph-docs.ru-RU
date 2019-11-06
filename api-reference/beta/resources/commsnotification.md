---
title: Тип ресурса Коммснотификатион
description: Базовый тип уведомления о связи, который публикуется серверами Communications Server для уведомления об изменениях.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 9901c1390d1813413cdd95949debea95d54c286b
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006707"
---
# <a name="commsnotification-resource-type"></a><span data-ttu-id="86794-103">Тип ресурса Коммснотификатион</span><span class="sxs-lookup"><span data-stu-id="86794-103">commsNotification resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="86794-104">Базовый тип уведомления о связи, который публикуется серверами Communications Server для уведомления об изменениях.</span><span class="sxs-lookup"><span data-stu-id="86794-104">Communications notification base type that is published by Communications servers to notify changes.</span></span>

## <a name="properties"></a><span data-ttu-id="86794-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="86794-105">Properties</span></span>
| <span data-ttu-id="86794-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="86794-106">Property</span></span>       | <span data-ttu-id="86794-107">Тип</span><span class="sxs-lookup"><span data-stu-id="86794-107">Type</span></span>    | <span data-ttu-id="86794-108">Описание</span><span class="sxs-lookup"><span data-stu-id="86794-108">Description</span></span>                                                |
|:---------------|:--------|:-----------------------------------------------------------|
| <span data-ttu-id="86794-109">changeType</span><span class="sxs-lookup"><span data-stu-id="86794-109">changeType</span></span>     | <span data-ttu-id="86794-110">String</span><span class="sxs-lookup"><span data-stu-id="86794-110">String</span></span>  | <span data-ttu-id="86794-111">Возможные значения: `created`, `updated`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="86794-111">Possible values are: `created`, `updated`, `deleted`.</span></span>      |
| <span data-ttu-id="86794-112">Resourceurl экземпляром</span><span class="sxs-lookup"><span data-stu-id="86794-112">resourceUrl</span></span>       | <span data-ttu-id="86794-113">String</span><span class="sxs-lookup"><span data-stu-id="86794-113">String</span></span>  | <span data-ttu-id="86794-114">URI ресурса, который был изменен.</span><span class="sxs-lookup"><span data-stu-id="86794-114">URI of the resource that was changed.</span></span>                      |

> <span data-ttu-id="86794-115">**Примечание:** `resourceData` доступно в виде дополнительных данных.</span><span class="sxs-lookup"><span data-stu-id="86794-115">**Note:** `resourceData` is available as additional data.</span></span> <span data-ttu-id="86794-116">Это сущность или коллекция (сущность) в зависимости от количества изменений, упакованных в уведомление.</span><span class="sxs-lookup"><span data-stu-id="86794-116">It is an entity or Collection(entity) depending on the number of changes packaged in the notification.</span></span>

## <a name="json-representation"></a><span data-ttu-id="86794-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="86794-117">JSON representation</span></span>

<span data-ttu-id="86794-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="86794-118">The following is a JSON representation of the resource.</span></span>

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
  "@odata.type": "#microsoft.graph.commsNotification",
  "changeType": "created | updated | deleted",
  "resourceUrl": "String"
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
