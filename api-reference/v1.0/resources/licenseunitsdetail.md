---
title: Тип ресурса licenseUnitsDetail
description: Свойство **prepaidUnits** объекта subscribedSku относится к типу **licenseUnitsDetail**.
localization_priority: Normal
ms.openlocfilehash: 8c2a4e995c7e1afa63b7f9daea6b61cbaf974958
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32519909"
---
# <a name="licenseunitsdetail-resource-type"></a><span data-ttu-id="0f8cb-103">Тип ресурса licenseUnitsDetail</span><span class="sxs-lookup"><span data-stu-id="0f8cb-103">licenseUnitsDetail resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0f8cb-104">Свойство **prepaidUnits** объекта [subscribedSku](subscribedsku.md) относится к типу **licenseUnitsDetail**.</span><span class="sxs-lookup"><span data-stu-id="0f8cb-104">The **prepaidUnits** property of the [subscribedSku](subscribedsku.md) entity is of type **licenseUnitsDetail**.</span></span>

## <a name="properties"></a><span data-ttu-id="0f8cb-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="0f8cb-105">Properties</span></span>
| <span data-ttu-id="0f8cb-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="0f8cb-106">Property</span></span>     | <span data-ttu-id="0f8cb-107">Тип</span><span class="sxs-lookup"><span data-stu-id="0f8cb-107">Type</span></span>   |<span data-ttu-id="0f8cb-108">Описание</span><span class="sxs-lookup"><span data-stu-id="0f8cb-108">Description</span></span>|
|:-------------|:-----|:----------|
|<span data-ttu-id="0f8cb-109">enabled</span><span class="sxs-lookup"><span data-stu-id="0f8cb-109">enabled</span></span>|<span data-ttu-id="0f8cb-110">Int32</span><span class="sxs-lookup"><span data-stu-id="0f8cb-110">Int32</span></span>| <span data-ttu-id="0f8cb-111">Количество включенных единиц.</span><span class="sxs-lookup"><span data-stu-id="0f8cb-111">The number of units that are enabled.</span></span> |
|<span data-ttu-id="0f8cb-112">suspended</span><span class="sxs-lookup"><span data-stu-id="0f8cb-112">suspended</span></span>|<span data-ttu-id="0f8cb-113">Int32</span><span class="sxs-lookup"><span data-stu-id="0f8cb-113">Int32</span></span>| <span data-ttu-id="0f8cb-114">Количество приостановленных единиц.</span><span class="sxs-lookup"><span data-stu-id="0f8cb-114">The number of units that are suspended.</span></span> |
|<span data-ttu-id="0f8cb-115">warning</span><span class="sxs-lookup"><span data-stu-id="0f8cb-115">warning</span></span>|<span data-ttu-id="0f8cb-116">Int32</span><span class="sxs-lookup"><span data-stu-id="0f8cb-116">Int32</span></span>| <span data-ttu-id="0f8cb-117">Количество единиц, которые находятся в состоянии предупреждения.</span><span class="sxs-lookup"><span data-stu-id="0f8cb-117">The number of units that are in warning status.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0f8cb-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0f8cb-118">JSON representation</span></span>

<span data-ttu-id="0f8cb-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0f8cb-119">Here is a JSON representation of the resource</span></span>

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
