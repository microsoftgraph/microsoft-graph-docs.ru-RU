---
title: Тип ресурса licenseUnitsDetail
description: Свойство **prepaidUnits** объекта subscribedSku относится к типу **licenseUnitsDetail**.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 4482f9661b41981717422c7c874319fbca7be23d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966979"
---
# <a name="licenseunitsdetail-resource-type"></a><span data-ttu-id="f9d70-103">Тип ресурса licenseUnitsDetail</span><span class="sxs-lookup"><span data-stu-id="f9d70-103">licenseUnitsDetail resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f9d70-104">Свойство **prepaidUnits** объекта [subscribedSku](subscribedsku.md) относится к типу **licenseUnitsDetail**.</span><span class="sxs-lookup"><span data-stu-id="f9d70-104">The **prepaidUnits** property of the [subscribedSku](subscribedsku.md) entity is of type **licenseUnitsDetail**.</span></span>

## <a name="properties"></a><span data-ttu-id="f9d70-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="f9d70-105">Properties</span></span>
| <span data-ttu-id="f9d70-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="f9d70-106">Property</span></span>     | <span data-ttu-id="f9d70-107">Тип</span><span class="sxs-lookup"><span data-stu-id="f9d70-107">Type</span></span>   |<span data-ttu-id="f9d70-108">Описание</span><span class="sxs-lookup"><span data-stu-id="f9d70-108">Description</span></span>|
|:-------------|:-----|:----------|
|<span data-ttu-id="f9d70-109">enabled</span><span class="sxs-lookup"><span data-stu-id="f9d70-109">enabled</span></span>|<span data-ttu-id="f9d70-110">Int32</span><span class="sxs-lookup"><span data-stu-id="f9d70-110">Int32</span></span>| <span data-ttu-id="f9d70-111">Количество включенных единиц.</span><span class="sxs-lookup"><span data-stu-id="f9d70-111">The number of units that are enabled.</span></span> |
|<span data-ttu-id="f9d70-112">suspended</span><span class="sxs-lookup"><span data-stu-id="f9d70-112">suspended</span></span>|<span data-ttu-id="f9d70-113">Int32</span><span class="sxs-lookup"><span data-stu-id="f9d70-113">Int32</span></span>| <span data-ttu-id="f9d70-114">Количество приостановленных единиц.</span><span class="sxs-lookup"><span data-stu-id="f9d70-114">The number of units that are suspended.</span></span> |
|<span data-ttu-id="f9d70-115">warning</span><span class="sxs-lookup"><span data-stu-id="f9d70-115">warning</span></span>|<span data-ttu-id="f9d70-116">Int32</span><span class="sxs-lookup"><span data-stu-id="f9d70-116">Int32</span></span>| <span data-ttu-id="f9d70-117">Количество единиц, которые находятся в состоянии предупреждения.</span><span class="sxs-lookup"><span data-stu-id="f9d70-117">The number of units that are in warning status.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f9d70-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f9d70-118">JSON representation</span></span>

<span data-ttu-id="f9d70-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f9d70-119">Here is a JSON representation of the resource</span></span>

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
