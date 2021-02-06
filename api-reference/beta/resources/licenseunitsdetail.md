---
title: Тип ресурса licenseUnitsDetail
description: Свойство **prepaidUnits** объекта subscribedSku относится к типу **licenseUnitsDetail**.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: directory-management
author: krbain
ms.openlocfilehash: 3d4925c2acea0216e16283eaa8f779cb556e0857
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132435"
---
# <a name="licenseunitsdetail-resource-type"></a><span data-ttu-id="bea6b-103">Тип ресурса licenseUnitsDetail</span><span class="sxs-lookup"><span data-stu-id="bea6b-103">licenseUnitsDetail resource type</span></span>

<span data-ttu-id="bea6b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bea6b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bea6b-105">Свойство **prepaidUnits** объекта [subscribedSku](subscribedsku.md) относится к типу **licenseUnitsDetail**.</span><span class="sxs-lookup"><span data-stu-id="bea6b-105">The **prepaidUnits** property of the [subscribedSku](subscribedsku.md) entity is of type **licenseUnitsDetail**.</span></span>

## <a name="properties"></a><span data-ttu-id="bea6b-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="bea6b-106">Properties</span></span>
| <span data-ttu-id="bea6b-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="bea6b-107">Property</span></span>     | <span data-ttu-id="bea6b-108">Тип</span><span class="sxs-lookup"><span data-stu-id="bea6b-108">Type</span></span>   |<span data-ttu-id="bea6b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="bea6b-109">Description</span></span>|
|:-------------|:-----|:----------|
|<span data-ttu-id="bea6b-110">enabled</span><span class="sxs-lookup"><span data-stu-id="bea6b-110">enabled</span></span>|<span data-ttu-id="bea6b-111">Int32</span><span class="sxs-lookup"><span data-stu-id="bea6b-111">Int32</span></span>| <span data-ttu-id="bea6b-112">Количество включенных единиц.</span><span class="sxs-lookup"><span data-stu-id="bea6b-112">The number of units that are enabled.</span></span> |
|<span data-ttu-id="bea6b-113">suspended</span><span class="sxs-lookup"><span data-stu-id="bea6b-113">suspended</span></span>|<span data-ttu-id="bea6b-114">Int32</span><span class="sxs-lookup"><span data-stu-id="bea6b-114">Int32</span></span>| <span data-ttu-id="bea6b-115">Количество приостановленных единиц.</span><span class="sxs-lookup"><span data-stu-id="bea6b-115">The number of units that are suspended.</span></span> |
|<span data-ttu-id="bea6b-116">warning</span><span class="sxs-lookup"><span data-stu-id="bea6b-116">warning</span></span>|<span data-ttu-id="bea6b-117">Int32</span><span class="sxs-lookup"><span data-stu-id="bea6b-117">Int32</span></span>| <span data-ttu-id="bea6b-118">Количество единиц, которые находятся в состоянии предупреждения.</span><span class="sxs-lookup"><span data-stu-id="bea6b-118">The number of units that are in warning status.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="bea6b-119">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="bea6b-119">JSON representation</span></span>

<span data-ttu-id="bea6b-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bea6b-120">Here is a JSON representation of the resource</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "licenseUnitsDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


