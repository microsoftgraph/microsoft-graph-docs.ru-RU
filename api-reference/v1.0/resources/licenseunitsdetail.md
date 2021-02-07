---
title: Тип ресурса licenseUnitsDetail
description: Свойство **prepaidUnits** объекта subscribedSku относится к типу **licenseUnitsDetail**.
localization_priority: Normal
author: krbain
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: a942cb72d3830e95f983134a960daa4af1ff1589
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136652"
---
# <a name="licenseunitsdetail-resource-type"></a><span data-ttu-id="3ed62-103">Тип ресурса licenseUnitsDetail</span><span class="sxs-lookup"><span data-stu-id="3ed62-103">licenseUnitsDetail resource type</span></span>

<span data-ttu-id="3ed62-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3ed62-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3ed62-105">Свойство **prepaidUnits** объекта [subscribedSku](subscribedsku.md) относится к типу **licenseUnitsDetail**.</span><span class="sxs-lookup"><span data-stu-id="3ed62-105">The **prepaidUnits** property of the [subscribedSku](subscribedsku.md) entity is of type **licenseUnitsDetail**.</span></span>

## <a name="properties"></a><span data-ttu-id="3ed62-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="3ed62-106">Properties</span></span>
| <span data-ttu-id="3ed62-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="3ed62-107">Property</span></span>     | <span data-ttu-id="3ed62-108">Тип</span><span class="sxs-lookup"><span data-stu-id="3ed62-108">Type</span></span>   |<span data-ttu-id="3ed62-109">Описание</span><span class="sxs-lookup"><span data-stu-id="3ed62-109">Description</span></span>|
|:-------------|:-----|:----------|
|<span data-ttu-id="3ed62-110">enabled</span><span class="sxs-lookup"><span data-stu-id="3ed62-110">enabled</span></span>|<span data-ttu-id="3ed62-111">Int32</span><span class="sxs-lookup"><span data-stu-id="3ed62-111">Int32</span></span>| <span data-ttu-id="3ed62-112">Количество включенных единиц.</span><span class="sxs-lookup"><span data-stu-id="3ed62-112">The number of units that are enabled.</span></span> |
|<span data-ttu-id="3ed62-113">suspended</span><span class="sxs-lookup"><span data-stu-id="3ed62-113">suspended</span></span>|<span data-ttu-id="3ed62-114">Int32</span><span class="sxs-lookup"><span data-stu-id="3ed62-114">Int32</span></span>| <span data-ttu-id="3ed62-115">Количество приостановленных единиц.</span><span class="sxs-lookup"><span data-stu-id="3ed62-115">The number of units that are suspended.</span></span> |
|<span data-ttu-id="3ed62-116">warning</span><span class="sxs-lookup"><span data-stu-id="3ed62-116">warning</span></span>|<span data-ttu-id="3ed62-117">Int32</span><span class="sxs-lookup"><span data-stu-id="3ed62-117">Int32</span></span>| <span data-ttu-id="3ed62-118">Количество единиц, которые находятся в состоянии предупреждения.</span><span class="sxs-lookup"><span data-stu-id="3ed62-118">The number of units that are in warning status.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3ed62-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3ed62-119">JSON representation</span></span>

<span data-ttu-id="3ed62-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3ed62-120">Here is a JSON representation of the resource</span></span>

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

