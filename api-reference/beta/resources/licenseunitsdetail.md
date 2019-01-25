---
title: Тип ресурса licenseUnitsDetail
description: Свойство prepaidUnits объекта subscribedSku относится к типу licenseUnitsDetail.
localization_priority: Normal
ms.openlocfilehash: a5eacb79dfca97b992e2f8584761aaa45beccd76
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511319"
---
# <a name="licenseunitsdetail-resource-type"></a><span data-ttu-id="e22fa-103">Тип ресурса licenseUnitsDetail</span><span class="sxs-lookup"><span data-stu-id="e22fa-103">licenseUnitsDetail resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e22fa-104">Свойство **prepaidUnits** объекта [subscribedSku](subscribedsku.md) относится к типу **licenseUnitsDetail**.</span><span class="sxs-lookup"><span data-stu-id="e22fa-104">The **prepaidUnits** property of the [subscribedSku](subscribedsku.md) entity is of type **licenseUnitsDetail**.</span></span>

## <a name="properties"></a><span data-ttu-id="e22fa-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="e22fa-105">Properties</span></span>
| <span data-ttu-id="e22fa-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="e22fa-106">Property</span></span>     | <span data-ttu-id="e22fa-107">Тип</span><span class="sxs-lookup"><span data-stu-id="e22fa-107">Type</span></span>   |<span data-ttu-id="e22fa-108">Описание</span><span class="sxs-lookup"><span data-stu-id="e22fa-108">Description</span></span>|
|:-------------|:-----|:----------|
|<span data-ttu-id="e22fa-109">enabled</span><span class="sxs-lookup"><span data-stu-id="e22fa-109">enabled</span></span>|<span data-ttu-id="e22fa-110">Int32</span><span class="sxs-lookup"><span data-stu-id="e22fa-110">Int32</span></span>| <span data-ttu-id="e22fa-111">Число включенных единиц.</span><span class="sxs-lookup"><span data-stu-id="e22fa-111">The number of units that are enabled.</span></span> |
|<span data-ttu-id="e22fa-112">suspended</span><span class="sxs-lookup"><span data-stu-id="e22fa-112">suspended</span></span>|<span data-ttu-id="e22fa-113">Int32</span><span class="sxs-lookup"><span data-stu-id="e22fa-113">Int32</span></span>| <span data-ttu-id="e22fa-114">Число единиц, действие которых приостановлено.</span><span class="sxs-lookup"><span data-stu-id="e22fa-114">The number of units that are suspended.</span></span> |
|<span data-ttu-id="e22fa-115">warning</span><span class="sxs-lookup"><span data-stu-id="e22fa-115">warning</span></span>|<span data-ttu-id="e22fa-116">Int32</span><span class="sxs-lookup"><span data-stu-id="e22fa-116">Int32</span></span>| <span data-ttu-id="e22fa-117">Число единиц в состоянии предупреждения.</span><span class="sxs-lookup"><span data-stu-id="e22fa-117">The number of units that are in warning status.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e22fa-118">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e22fa-118">JSON representation</span></span>

<span data-ttu-id="e22fa-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e22fa-119">Here is a JSON representation of the resource</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/licenseunitsdetail.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
