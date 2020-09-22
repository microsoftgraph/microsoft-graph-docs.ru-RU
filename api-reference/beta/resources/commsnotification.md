---
title: Тип ресурса Коммснотификатион
description: Базовый тип уведомления о связи, который публикуется серверами Communications Server для уведомления об изменениях.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: c87c12aee367a6520485a222702f827ae833aa98
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48033967"
---
# <a name="commsnotification-resource-type"></a><span data-ttu-id="5d7fa-103">Тип ресурса Коммснотификатион</span><span class="sxs-lookup"><span data-stu-id="5d7fa-103">commsNotification resource type</span></span>

<span data-ttu-id="5d7fa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5d7fa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5d7fa-105">Базовый тип уведомления о связи, который публикуется серверами Communications Server для уведомления об изменениях.</span><span class="sxs-lookup"><span data-stu-id="5d7fa-105">Communications notification base type that is published by Communications servers to notify changes.</span></span>

## <a name="properties"></a><span data-ttu-id="5d7fa-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="5d7fa-106">Properties</span></span>
| <span data-ttu-id="5d7fa-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="5d7fa-107">Property</span></span>       | <span data-ttu-id="5d7fa-108">Тип</span><span class="sxs-lookup"><span data-stu-id="5d7fa-108">Type</span></span>    | <span data-ttu-id="5d7fa-109">Описание</span><span class="sxs-lookup"><span data-stu-id="5d7fa-109">Description</span></span>                                                |
|:---------------|:--------|:-----------------------------------------------------------|
| <span data-ttu-id="5d7fa-110">changeType</span><span class="sxs-lookup"><span data-stu-id="5d7fa-110">changeType</span></span>     | <span data-ttu-id="5d7fa-111">String</span><span class="sxs-lookup"><span data-stu-id="5d7fa-111">String</span></span>  | <span data-ttu-id="5d7fa-112">Возможные значения: `created`, `updated`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="5d7fa-112">Possible values are: `created`, `updated`, `deleted`.</span></span>      |
| <span data-ttu-id="5d7fa-113">Resourceurl экземпляром</span><span class="sxs-lookup"><span data-stu-id="5d7fa-113">resourceUrl</span></span>       | <span data-ttu-id="5d7fa-114">String</span><span class="sxs-lookup"><span data-stu-id="5d7fa-114">String</span></span>  | <span data-ttu-id="5d7fa-115">URI ресурса, который был изменен.</span><span class="sxs-lookup"><span data-stu-id="5d7fa-115">URI of the resource that was changed.</span></span>                      |

> <span data-ttu-id="5d7fa-116">**Примечание:** `resourceData` доступна в виде дополнительных данных.</span><span class="sxs-lookup"><span data-stu-id="5d7fa-116">**Note:** `resourceData` is available as additional data.</span></span> <span data-ttu-id="5d7fa-117">Это либо сущность, либо коллекция сущностей в зависимости от количества изменений, упакованных в уведомление.</span><span class="sxs-lookup"><span data-stu-id="5d7fa-117">It is either an entity or a collection of entities depending on the number of changes packaged in the notification.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5d7fa-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5d7fa-118">JSON representation</span></span>

<span data-ttu-id="5d7fa-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5d7fa-119">The following is a JSON representation of the resource.</span></span>

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


