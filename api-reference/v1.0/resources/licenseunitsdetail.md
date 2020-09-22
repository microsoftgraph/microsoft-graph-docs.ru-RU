---
title: Тип ресурса licenseUnitsDetail
description: Свойство **prepaidUnits** объекта subscribedSku относится к типу **licenseUnitsDetail**.
localization_priority: Normal
author: krbain
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: af761aea94f21d3543bcaa8032d4120e3d1ad502
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48048332"
---
# <a name="licenseunitsdetail-resource-type"></a><span data-ttu-id="51b37-103">Тип ресурса licenseUnitsDetail</span><span class="sxs-lookup"><span data-stu-id="51b37-103">licenseUnitsDetail resource type</span></span>

<span data-ttu-id="51b37-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="51b37-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="51b37-105">Свойство **prepaidUnits** объекта [subscribedSku](subscribedsku.md) относится к типу **licenseUnitsDetail**.</span><span class="sxs-lookup"><span data-stu-id="51b37-105">The **prepaidUnits** property of the [subscribedSku](subscribedsku.md) entity is of type **licenseUnitsDetail**.</span></span>

## <a name="properties"></a><span data-ttu-id="51b37-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="51b37-106">Properties</span></span>
| <span data-ttu-id="51b37-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="51b37-107">Property</span></span>     | <span data-ttu-id="51b37-108">Тип</span><span class="sxs-lookup"><span data-stu-id="51b37-108">Type</span></span>   |<span data-ttu-id="51b37-109">Описание</span><span class="sxs-lookup"><span data-stu-id="51b37-109">Description</span></span>|
|:-------------|:-----|:----------|
|<span data-ttu-id="51b37-110">enabled</span><span class="sxs-lookup"><span data-stu-id="51b37-110">enabled</span></span>|<span data-ttu-id="51b37-111">Int32</span><span class="sxs-lookup"><span data-stu-id="51b37-111">Int32</span></span>| <span data-ttu-id="51b37-112">Количество включенных единиц.</span><span class="sxs-lookup"><span data-stu-id="51b37-112">The number of units that are enabled.</span></span> |
|<span data-ttu-id="51b37-113">suspended</span><span class="sxs-lookup"><span data-stu-id="51b37-113">suspended</span></span>|<span data-ttu-id="51b37-114">Int32</span><span class="sxs-lookup"><span data-stu-id="51b37-114">Int32</span></span>| <span data-ttu-id="51b37-115">Количество приостановленных единиц.</span><span class="sxs-lookup"><span data-stu-id="51b37-115">The number of units that are suspended.</span></span> |
|<span data-ttu-id="51b37-116">warning</span><span class="sxs-lookup"><span data-stu-id="51b37-116">warning</span></span>|<span data-ttu-id="51b37-117">Int32</span><span class="sxs-lookup"><span data-stu-id="51b37-117">Int32</span></span>| <span data-ttu-id="51b37-118">Количество единиц, которые находятся в состоянии предупреждения.</span><span class="sxs-lookup"><span data-stu-id="51b37-118">The number of units that are in warning status.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="51b37-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="51b37-119">JSON representation</span></span>

<span data-ttu-id="51b37-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="51b37-120">Here is a JSON representation of the resource</span></span>

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

