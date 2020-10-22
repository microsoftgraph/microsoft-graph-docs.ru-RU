---
title: Тип ресурса Емплойиоргдата
description: Представляет данные организации, связанные с пользователем.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: cmmdesai
ms.openlocfilehash: 841d3c7965309721d662475f2cba553c378c49ee
ms.sourcegitcommit: 21481acf54471ff17ab8043b3a96fcb1d2f863d7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/21/2020
ms.locfileid: "48635612"
---
# <a name="employeeorgdata-resource-type"></a><span data-ttu-id="2bb88-103">Тип ресурса Емплойиоргдата</span><span class="sxs-lookup"><span data-stu-id="2bb88-103">employeeOrgData resource type</span></span>

<span data-ttu-id="2bb88-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2bb88-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2bb88-105">Представляет данные организации, связанные с пользователем.</span><span class="sxs-lookup"><span data-stu-id="2bb88-105">Represents organization data associated with a user.</span></span> <span data-ttu-id="2bb88-106">Свойство **емплойиоргдата** объекта [User](user.md) — это коллекция атрибутов Организации.</span><span class="sxs-lookup"><span data-stu-id="2bb88-106">The **employeeOrgData** property of the [user](user.md) entity is a collection of organization attributes.</span></span>

## <a name="properties"></a><span data-ttu-id="2bb88-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="2bb88-107">Properties</span></span>
| <span data-ttu-id="2bb88-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="2bb88-108">Property</span></span>       | <span data-ttu-id="2bb88-109">Тип</span><span class="sxs-lookup"><span data-stu-id="2bb88-109">Type</span></span>    |<span data-ttu-id="2bb88-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2bb88-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2bb88-111">division</span><span class="sxs-lookup"><span data-stu-id="2bb88-111">division</span></span> | <span data-ttu-id="2bb88-112">String</span><span class="sxs-lookup"><span data-stu-id="2bb88-112">String</span></span> | <span data-ttu-id="2bb88-113">Имя подразделения, в котором работает пользователь.</span><span class="sxs-lookup"><span data-stu-id="2bb88-113">The name of the division in which the user works.</span></span> <br><br><span data-ttu-id="2bb88-114">Возвращается только на `$select`.</span><span class="sxs-lookup"><span data-stu-id="2bb88-114">Returned only on `$select`.</span></span> <span data-ttu-id="2bb88-115">Поддерживает `$filter`.</span><span class="sxs-lookup"><span data-stu-id="2bb88-115">Supports `$filter`.</span></span> |
| <span data-ttu-id="2bb88-116">costCenter</span><span class="sxs-lookup"><span data-stu-id="2bb88-116">costCenter</span></span> | <span data-ttu-id="2bb88-117">String</span><span class="sxs-lookup"><span data-stu-id="2bb88-117">String</span></span> | <span data-ttu-id="2bb88-118">Центр затрат, связанный с пользователем.</span><span class="sxs-lookup"><span data-stu-id="2bb88-118">The cost center associated with the user.</span></span> <br><br><span data-ttu-id="2bb88-119">Возвращается только на `$select`.</span><span class="sxs-lookup"><span data-stu-id="2bb88-119">Returned only on `$select`.</span></span> <span data-ttu-id="2bb88-120">Поддерживает `$filter`.</span><span class="sxs-lookup"><span data-stu-id="2bb88-120">Supports `$filter`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2bb88-121">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="2bb88-121">JSON representation</span></span>

<span data-ttu-id="2bb88-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2bb88-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.employeeOrgData"
}-->

```json
{
  "costCenter": "string",
  "division": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2020-10-24 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "employeeOrgData resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
