---
title: Тип ресурса licenseUnitsDetail
description: Свойство **prepaidUnits** объекта subscribedSku относится к типу **licenseUnitsDetail**.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 4de4d89b5abec06abc6d2f8bfa4f78c22abe4ca0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447579"
---
# <a name="licenseunitsdetail-resource-type"></a><span data-ttu-id="490a8-103">Тип ресурса licenseUnitsDetail</span><span class="sxs-lookup"><span data-stu-id="490a8-103">licenseUnitsDetail resource type</span></span>

<span data-ttu-id="490a8-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="490a8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="490a8-105">Свойство **prepaidUnits** объекта [subscribedSku](subscribedsku.md) относится к типу **licenseUnitsDetail**.</span><span class="sxs-lookup"><span data-stu-id="490a8-105">The **prepaidUnits** property of the [subscribedSku](subscribedsku.md) entity is of type **licenseUnitsDetail**.</span></span>

## <a name="properties"></a><span data-ttu-id="490a8-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="490a8-106">Properties</span></span>
| <span data-ttu-id="490a8-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="490a8-107">Property</span></span>     | <span data-ttu-id="490a8-108">Тип</span><span class="sxs-lookup"><span data-stu-id="490a8-108">Type</span></span>   |<span data-ttu-id="490a8-109">Описание</span><span class="sxs-lookup"><span data-stu-id="490a8-109">Description</span></span>|
|:-------------|:-----|:----------|
|<span data-ttu-id="490a8-110">enabled</span><span class="sxs-lookup"><span data-stu-id="490a8-110">enabled</span></span>|<span data-ttu-id="490a8-111">Int32</span><span class="sxs-lookup"><span data-stu-id="490a8-111">Int32</span></span>| <span data-ttu-id="490a8-112">Количество включенных единиц.</span><span class="sxs-lookup"><span data-stu-id="490a8-112">The number of units that are enabled.</span></span> |
|<span data-ttu-id="490a8-113">suspended</span><span class="sxs-lookup"><span data-stu-id="490a8-113">suspended</span></span>|<span data-ttu-id="490a8-114">Int32</span><span class="sxs-lookup"><span data-stu-id="490a8-114">Int32</span></span>| <span data-ttu-id="490a8-115">Количество приостановленных единиц.</span><span class="sxs-lookup"><span data-stu-id="490a8-115">The number of units that are suspended.</span></span> |
|<span data-ttu-id="490a8-116">warning</span><span class="sxs-lookup"><span data-stu-id="490a8-116">warning</span></span>|<span data-ttu-id="490a8-117">Int32</span><span class="sxs-lookup"><span data-stu-id="490a8-117">Int32</span></span>| <span data-ttu-id="490a8-118">Количество единиц, которые находятся в состоянии предупреждения.</span><span class="sxs-lookup"><span data-stu-id="490a8-118">The number of units that are in warning status.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="490a8-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="490a8-119">JSON representation</span></span>

<span data-ttu-id="490a8-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="490a8-120">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.licenseUnitsDetail"
}-->

```json
{
  "enabled": 1024,
  "suspended": 1024,
  "warning": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "licenseUnitsDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
