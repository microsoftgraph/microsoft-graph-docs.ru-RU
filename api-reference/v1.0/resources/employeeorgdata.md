---
title: тип ресурса employeeOrgData
description: Представляет данные организации, связанные с пользователем.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: users
author: cmmdesai
ms.openlocfilehash: 5e3ea0401730ffc8b15cae8c371d9352995c6f28
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50961995"
---
# <a name="employeeorgdata-resource-type"></a><span data-ttu-id="38754-103">тип ресурса employeeOrgData</span><span class="sxs-lookup"><span data-stu-id="38754-103">employeeOrgData resource type</span></span>

<span data-ttu-id="38754-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="38754-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="38754-105">Представляет данные организации, связанные с пользователем.</span><span class="sxs-lookup"><span data-stu-id="38754-105">Represents organization data associated with a user.</span></span> <span data-ttu-id="38754-106">Свойство **employeeOrgData** сущности [пользователя](user.md) — это коллекция атрибутов организации.</span><span class="sxs-lookup"><span data-stu-id="38754-106">The **employeeOrgData** property of the [user](user.md) entity is a collection of organization attributes.</span></span>

## <a name="properties"></a><span data-ttu-id="38754-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="38754-107">Properties</span></span>
| <span data-ttu-id="38754-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="38754-108">Property</span></span>       | <span data-ttu-id="38754-109">Тип</span><span class="sxs-lookup"><span data-stu-id="38754-109">Type</span></span>    |<span data-ttu-id="38754-110">Описание</span><span class="sxs-lookup"><span data-stu-id="38754-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="38754-111">division</span><span class="sxs-lookup"><span data-stu-id="38754-111">division</span></span> | <span data-ttu-id="38754-112">String</span><span class="sxs-lookup"><span data-stu-id="38754-112">String</span></span> | <span data-ttu-id="38754-113">Имя подразделения, в котором работает пользователь.</span><span class="sxs-lookup"><span data-stu-id="38754-113">The name of the division in which the user works.</span></span> <br><br><span data-ttu-id="38754-114">Возвращается только с помощью оператора `$select`.</span><span class="sxs-lookup"><span data-stu-id="38754-114">Returned only on `$select`.</span></span> <span data-ttu-id="38754-115">Поддерживает `$filter`.</span><span class="sxs-lookup"><span data-stu-id="38754-115">Supports `$filter`.</span></span> |
| <span data-ttu-id="38754-116">costCenter</span><span class="sxs-lookup"><span data-stu-id="38754-116">costCenter</span></span> | <span data-ttu-id="38754-117">String</span><span class="sxs-lookup"><span data-stu-id="38754-117">String</span></span> | <span data-ttu-id="38754-118">Центр затрат, связанный с пользователем.</span><span class="sxs-lookup"><span data-stu-id="38754-118">The cost center associated with the user.</span></span> <br><br><span data-ttu-id="38754-119">Возвращается только с помощью оператора `$select`.</span><span class="sxs-lookup"><span data-stu-id="38754-119">Returned only on `$select`.</span></span> <span data-ttu-id="38754-120">Поддерживает `$filter`.</span><span class="sxs-lookup"><span data-stu-id="38754-120">Supports `$filter`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="38754-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="38754-121">JSON representation</span></span>

<span data-ttu-id="38754-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="38754-122">The following is a JSON representation of the resource.</span></span>

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
