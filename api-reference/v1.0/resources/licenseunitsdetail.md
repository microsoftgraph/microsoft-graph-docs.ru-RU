---
title: Тип ресурса licenseUnitsDetail
description: Свойство **prepaidUnits** объекта subscribedSku относится к типу **licenseUnitsDetail**.
localization_priority: Normal
author: krbain
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 2133119f037e04d66dceb2b99f933d2caafc381c
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46811303"
---
# <a name="licenseunitsdetail-resource-type"></a><span data-ttu-id="74474-103">Тип ресурса licenseUnitsDetail</span><span class="sxs-lookup"><span data-stu-id="74474-103">licenseUnitsDetail resource type</span></span>

<span data-ttu-id="74474-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="74474-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="74474-105">Свойство **prepaidUnits** объекта [subscribedSku](subscribedsku.md) относится к типу **licenseUnitsDetail**.</span><span class="sxs-lookup"><span data-stu-id="74474-105">The **prepaidUnits** property of the [subscribedSku](subscribedsku.md) entity is of type **licenseUnitsDetail**.</span></span>

## <a name="properties"></a><span data-ttu-id="74474-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="74474-106">Properties</span></span>
| <span data-ttu-id="74474-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="74474-107">Property</span></span>     | <span data-ttu-id="74474-108">Тип</span><span class="sxs-lookup"><span data-stu-id="74474-108">Type</span></span>   |<span data-ttu-id="74474-109">Описание</span><span class="sxs-lookup"><span data-stu-id="74474-109">Description</span></span>|
|:-------------|:-----|:----------|
|<span data-ttu-id="74474-110">enabled</span><span class="sxs-lookup"><span data-stu-id="74474-110">enabled</span></span>|<span data-ttu-id="74474-111">Int32</span><span class="sxs-lookup"><span data-stu-id="74474-111">Int32</span></span>| <span data-ttu-id="74474-112">Количество включенных единиц.</span><span class="sxs-lookup"><span data-stu-id="74474-112">The number of units that are enabled.</span></span> |
|<span data-ttu-id="74474-113">suspended</span><span class="sxs-lookup"><span data-stu-id="74474-113">suspended</span></span>|<span data-ttu-id="74474-114">Int32</span><span class="sxs-lookup"><span data-stu-id="74474-114">Int32</span></span>| <span data-ttu-id="74474-115">Количество приостановленных единиц.</span><span class="sxs-lookup"><span data-stu-id="74474-115">The number of units that are suspended.</span></span> |
|<span data-ttu-id="74474-116">warning</span><span class="sxs-lookup"><span data-stu-id="74474-116">warning</span></span>|<span data-ttu-id="74474-117">Int32</span><span class="sxs-lookup"><span data-stu-id="74474-117">Int32</span></span>| <span data-ttu-id="74474-118">Количество единиц, которые находятся в состоянии предупреждения.</span><span class="sxs-lookup"><span data-stu-id="74474-118">The number of units that are in warning status.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="74474-119">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="74474-119">JSON representation</span></span>

<span data-ttu-id="74474-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="74474-120">Here is a JSON representation of the resource</span></span>

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
