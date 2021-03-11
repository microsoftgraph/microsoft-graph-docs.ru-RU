---
title: Тип ресурса licenseUnitsDetail
description: Свойство **prepaidUnits** объекта subscribedSku относится к типу **licenseUnitsDetail**.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: directory-management
author: jpettere
ms.openlocfilehash: 3cc2ba98b0d221774ea1700c279a115a68494580
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720517"
---
# <a name="licenseunitsdetail-resource-type"></a><span data-ttu-id="30134-103">Тип ресурса licenseUnitsDetail</span><span class="sxs-lookup"><span data-stu-id="30134-103">licenseUnitsDetail resource type</span></span>

<span data-ttu-id="30134-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="30134-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="30134-105">Свойство **prepaidUnits** объекта [subscribedSku](subscribedsku.md) относится к типу **licenseUnitsDetail**.</span><span class="sxs-lookup"><span data-stu-id="30134-105">The **prepaidUnits** property of the [subscribedSku](subscribedsku.md) entity is of type **licenseUnitsDetail**.</span></span>

## <a name="properties"></a><span data-ttu-id="30134-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="30134-106">Properties</span></span>
| <span data-ttu-id="30134-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="30134-107">Property</span></span>     | <span data-ttu-id="30134-108">Тип</span><span class="sxs-lookup"><span data-stu-id="30134-108">Type</span></span>   |<span data-ttu-id="30134-109">Описание</span><span class="sxs-lookup"><span data-stu-id="30134-109">Description</span></span>|
|:-------------|:-----|:----------|
|<span data-ttu-id="30134-110">enabled</span><span class="sxs-lookup"><span data-stu-id="30134-110">enabled</span></span>|<span data-ttu-id="30134-111">Int32</span><span class="sxs-lookup"><span data-stu-id="30134-111">Int32</span></span>| <span data-ttu-id="30134-112">Количество включенных единиц.</span><span class="sxs-lookup"><span data-stu-id="30134-112">The number of units that are enabled.</span></span> |
|<span data-ttu-id="30134-113">suspended</span><span class="sxs-lookup"><span data-stu-id="30134-113">suspended</span></span>|<span data-ttu-id="30134-114">Int32</span><span class="sxs-lookup"><span data-stu-id="30134-114">Int32</span></span>| <span data-ttu-id="30134-115">Количество приостановленных единиц.</span><span class="sxs-lookup"><span data-stu-id="30134-115">The number of units that are suspended.</span></span> |
|<span data-ttu-id="30134-116">warning</span><span class="sxs-lookup"><span data-stu-id="30134-116">warning</span></span>|<span data-ttu-id="30134-117">Int32</span><span class="sxs-lookup"><span data-stu-id="30134-117">Int32</span></span>| <span data-ttu-id="30134-118">Количество единиц, которые находятся в состоянии предупреждения.</span><span class="sxs-lookup"><span data-stu-id="30134-118">The number of units that are in warning status.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="30134-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="30134-119">JSON representation</span></span>

<span data-ttu-id="30134-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="30134-120">Here is a JSON representation of the resource</span></span>

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


