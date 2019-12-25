---
title: Тип ресурса Коммснотификатион
description: Базовый тип уведомления о связи, который публикуется серверами Communications Server для уведомления об изменениях.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 1752bbe46ee7795bd71df2089dadf6a975ccae26
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870927"
---
# <a name="commsnotification-resource-type"></a><span data-ttu-id="e7600-103">Тип ресурса Коммснотификатион</span><span class="sxs-lookup"><span data-stu-id="e7600-103">commsNotification resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e7600-104">Базовый тип уведомления о связи, который публикуется серверами Communications Server для уведомления об изменениях.</span><span class="sxs-lookup"><span data-stu-id="e7600-104">Communications notification base type that is published by Communications servers to notify changes.</span></span>

## <a name="properties"></a><span data-ttu-id="e7600-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="e7600-105">Properties</span></span>
| <span data-ttu-id="e7600-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="e7600-106">Property</span></span>       | <span data-ttu-id="e7600-107">Тип</span><span class="sxs-lookup"><span data-stu-id="e7600-107">Type</span></span>    | <span data-ttu-id="e7600-108">Описание</span><span class="sxs-lookup"><span data-stu-id="e7600-108">Description</span></span>                                                |
|:---------------|:--------|:-----------------------------------------------------------|
| <span data-ttu-id="e7600-109">changeType</span><span class="sxs-lookup"><span data-stu-id="e7600-109">changeType</span></span>     | <span data-ttu-id="e7600-110">String</span><span class="sxs-lookup"><span data-stu-id="e7600-110">String</span></span>  | <span data-ttu-id="e7600-111">Возможные значения: `created`, `updated`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="e7600-111">Possible values are: `created`, `updated`, `deleted`.</span></span>      |
| <span data-ttu-id="e7600-112">Resourceurl экземпляром</span><span class="sxs-lookup"><span data-stu-id="e7600-112">resourceUrl</span></span>       | <span data-ttu-id="e7600-113">String</span><span class="sxs-lookup"><span data-stu-id="e7600-113">String</span></span>  | <span data-ttu-id="e7600-114">URI ресурса, который был изменен.</span><span class="sxs-lookup"><span data-stu-id="e7600-114">URI of the resource that was changed.</span></span>                      |

> <span data-ttu-id="e7600-115">**Примечание:** `resourceData` доступно в виде дополнительных данных.</span><span class="sxs-lookup"><span data-stu-id="e7600-115">**Note:** `resourceData` is available as additional data.</span></span> <span data-ttu-id="e7600-116">Это либо сущность, либо коллекция сущностей в зависимости от количества изменений, упакованных в уведомление.</span><span class="sxs-lookup"><span data-stu-id="e7600-116">It is either an entity or a collection of entities depending on the number of changes packaged in the notification.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e7600-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e7600-117">JSON representation</span></span>

<span data-ttu-id="e7600-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e7600-118">The following is a JSON representation of the resource.</span></span>

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
