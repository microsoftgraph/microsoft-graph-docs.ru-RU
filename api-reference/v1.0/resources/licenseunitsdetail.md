---
title: Тип ресурса licenseUnitsDetail
description: Свойство **prepaidUnits** объекта subscribedSku относится к типу **licenseUnitsDetail**.
ms.openlocfilehash: e8cf5253676dab8a4b31c3ab33faa0af3ddfd527
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024575"
---
# <a name="licenseunitsdetail-resource-type"></a><span data-ttu-id="f9844-103">Тип ресурса licenseUnitsDetail</span><span class="sxs-lookup"><span data-stu-id="f9844-103">licenseUnitsDetail resource type</span></span>

<span data-ttu-id="f9844-104">Свойство **prepaidUnits** объекта [subscribedSku](subscribedsku.md) относится к типу **licenseUnitsDetail**.</span><span class="sxs-lookup"><span data-stu-id="f9844-104">The **prepaidUnits** property of the [subscribedSku](subscribedsku.md) entity is of type **licenseUnitsDetail**.</span></span>

## <a name="properties"></a><span data-ttu-id="f9844-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="f9844-105">Properties</span></span>
| <span data-ttu-id="f9844-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="f9844-106">Property</span></span>     | <span data-ttu-id="f9844-107">Тип</span><span class="sxs-lookup"><span data-stu-id="f9844-107">Type</span></span>   |<span data-ttu-id="f9844-108">Описание</span><span class="sxs-lookup"><span data-stu-id="f9844-108">Description</span></span>|
|:-------------|:-----|:----------|
|<span data-ttu-id="f9844-109">enabled</span><span class="sxs-lookup"><span data-stu-id="f9844-109">enabled</span></span>|<span data-ttu-id="f9844-110">Int32</span><span class="sxs-lookup"><span data-stu-id="f9844-110">Int32</span></span>| <span data-ttu-id="f9844-111">Число включенных единиц.</span><span class="sxs-lookup"><span data-stu-id="f9844-111">The number of units that are enabled.</span></span> |
|<span data-ttu-id="f9844-112">suspended</span><span class="sxs-lookup"><span data-stu-id="f9844-112">suspended</span></span>|<span data-ttu-id="f9844-113">Int32</span><span class="sxs-lookup"><span data-stu-id="f9844-113">Int32</span></span>| <span data-ttu-id="f9844-114">Число единиц, действие которых приостановлено.</span><span class="sxs-lookup"><span data-stu-id="f9844-114">The number of units that are suspended.</span></span> |
|<span data-ttu-id="f9844-115">warning</span><span class="sxs-lookup"><span data-stu-id="f9844-115">warning</span></span>|<span data-ttu-id="f9844-116">Int32</span><span class="sxs-lookup"><span data-stu-id="f9844-116">Int32</span></span>| <span data-ttu-id="f9844-117">Число единиц в состоянии предупреждения.</span><span class="sxs-lookup"><span data-stu-id="f9844-117">The number of units that are in warning status.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f9844-118">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="f9844-118">JSON representation</span></span>

<span data-ttu-id="f9844-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f9844-119">Here is a JSON representation of the resource</span></span>

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
