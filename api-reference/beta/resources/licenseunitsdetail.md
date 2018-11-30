---
title: Тип ресурса licenseUnitsDetail
description: Свойство **prepaidUnits** объекта subscribedSku относится к типу **licenseUnitsDetail**.
ms.openlocfilehash: 5f3d62c39248739746923195945efbc3322d5686
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074874"
---
# <a name="licenseunitsdetail-resource-type"></a><span data-ttu-id="45d56-103">Тип ресурса licenseUnitsDetail</span><span class="sxs-lookup"><span data-stu-id="45d56-103">licenseUnitsDetail resource type</span></span>

> <span data-ttu-id="45d56-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="45d56-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="45d56-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45d56-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="45d56-106">Свойство **prepaidUnits** объекта [subscribedSku](subscribedsku.md) относится к типу **licenseUnitsDetail**.</span><span class="sxs-lookup"><span data-stu-id="45d56-106">The **prepaidUnits** property of the [subscribedSku](subscribedsku.md) entity is of type **licenseUnitsDetail**.</span></span>

## <a name="properties"></a><span data-ttu-id="45d56-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="45d56-107">Properties</span></span>
| <span data-ttu-id="45d56-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="45d56-108">Property</span></span>     | <span data-ttu-id="45d56-109">Тип</span><span class="sxs-lookup"><span data-stu-id="45d56-109">Type</span></span>   |<span data-ttu-id="45d56-110">Описание</span><span class="sxs-lookup"><span data-stu-id="45d56-110">Description</span></span>|
|:-------------|:-----|:----------|
|<span data-ttu-id="45d56-111">enabled</span><span class="sxs-lookup"><span data-stu-id="45d56-111">enabled</span></span>|<span data-ttu-id="45d56-112">Int32</span><span class="sxs-lookup"><span data-stu-id="45d56-112">Int32</span></span>| <span data-ttu-id="45d56-113">Число включенных единиц.</span><span class="sxs-lookup"><span data-stu-id="45d56-113">The number of units that are enabled.</span></span> |
|<span data-ttu-id="45d56-114">suspended</span><span class="sxs-lookup"><span data-stu-id="45d56-114">suspended</span></span>|<span data-ttu-id="45d56-115">Int32</span><span class="sxs-lookup"><span data-stu-id="45d56-115">Int32</span></span>| <span data-ttu-id="45d56-116">Число единиц, действие которых приостановлено.</span><span class="sxs-lookup"><span data-stu-id="45d56-116">The number of units that are suspended.</span></span> |
|<span data-ttu-id="45d56-117">warning</span><span class="sxs-lookup"><span data-stu-id="45d56-117">warning</span></span>|<span data-ttu-id="45d56-118">Int32</span><span class="sxs-lookup"><span data-stu-id="45d56-118">Int32</span></span>| <span data-ttu-id="45d56-119">Число единиц в состоянии предупреждения.</span><span class="sxs-lookup"><span data-stu-id="45d56-119">The number of units that are in warning status.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="45d56-120">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="45d56-120">JSON representation</span></span>

<span data-ttu-id="45d56-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="45d56-121">Here is a JSON representation of the resource</span></span>

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
