---
title: Тип ресурса Кондитионалакцессусерс
description: Представляет пользователей, группы и роли, включенные в область политики и исключенные из нее.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 7e54c5b018331952776b36a0ab3c07be88c2be7c
ms.sourcegitcommit: 3ee6a3a949be7f0a9028bde90092a10a42e0f1fc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/23/2019
ms.locfileid: "37638479"
---
# <a name="conditionalaccessusers-resource-type"></a><span data-ttu-id="bd037-103">Тип ресурса Кондитионалакцессусерс</span><span class="sxs-lookup"><span data-stu-id="bd037-103">conditionalAccessUsers resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bd037-104">Представляет пользователей, группы и роли, включенные в область политики и исключенные из нее.</span><span class="sxs-lookup"><span data-stu-id="bd037-104">Represents users, groups, and roles included in and excluded from the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="bd037-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="bd037-105">Properties</span></span>

| <span data-ttu-id="bd037-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="bd037-106">Property</span></span>     | <span data-ttu-id="bd037-107">Тип</span><span class="sxs-lookup"><span data-stu-id="bd037-107">Type</span></span>        | <span data-ttu-id="bd037-108">Описание</span><span class="sxs-lookup"><span data-stu-id="bd037-108">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="bd037-109">инклудеусерс</span><span class="sxs-lookup"><span data-stu-id="bd037-109">includeUsers</span></span> | <span data-ttu-id="bd037-110">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="bd037-110">String collection</span></span> | <span data-ttu-id="bd037-111">Идентификаторы пользователей в области применения политики, если явно не `None` исключены, `All` или или `GuestsOrExternalUsers`.</span><span class="sxs-lookup"><span data-stu-id="bd037-111">User IDs in scope of policy unless explicitly excluded, or `None` or `All` or `GuestsOrExternalUsers`.</span></span> |
| <span data-ttu-id="bd037-112">ексклудеусерс</span><span class="sxs-lookup"><span data-stu-id="bd037-112">excludeUsers</span></span> | <span data-ttu-id="bd037-113">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="bd037-113">String collection</span></span> | <span data-ttu-id="bd037-114">Идентификаторы пользователей, исключенные из области применения политики `GuestsOrExternalUsers`и/или.</span><span class="sxs-lookup"><span data-stu-id="bd037-114">User IDs excluded from scope of policy and/or `GuestsOrExternalUsers`.</span></span> |
| <span data-ttu-id="bd037-115">инклудеграупс</span><span class="sxs-lookup"><span data-stu-id="bd037-115">includeGroups</span></span> | <span data-ttu-id="bd037-116">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="bd037-116">String collection</span></span> | <span data-ttu-id="bd037-117">Идентификаторы групп в области политики, если явно не исключены, или `All`.</span><span class="sxs-lookup"><span data-stu-id="bd037-117">Group IDs in scope of policy unless explicitly excluded, or `All`.</span></span> |
| <span data-ttu-id="bd037-118">ексклудеграупс</span><span class="sxs-lookup"><span data-stu-id="bd037-118">excludeGroups</span></span> | <span data-ttu-id="bd037-119">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="bd037-119">String collection</span></span> | <span data-ttu-id="bd037-120">Идентификаторы групп, исключенные из области применения политики.</span><span class="sxs-lookup"><span data-stu-id="bd037-120">Group IDs excluded from scope of policy.</span></span> |
| <span data-ttu-id="bd037-121">инклудеролес</span><span class="sxs-lookup"><span data-stu-id="bd037-121">includeRoles</span></span> | <span data-ttu-id="bd037-122">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="bd037-122">String collection</span></span> | <span data-ttu-id="bd037-123">Идентификаторы ролей в области применения политики, если они явно `All`не исключены, или.</span><span class="sxs-lookup"><span data-stu-id="bd037-123">Role IDs in scope of policy unless explicitly excluded, or `All`.</span></span> |
| <span data-ttu-id="bd037-124">ексклудеролес</span><span class="sxs-lookup"><span data-stu-id="bd037-124">excludeRoles</span></span> | <span data-ttu-id="bd037-125">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="bd037-125">String collection</span></span> | <span data-ttu-id="bd037-126">Идентификаторы ролей, исключенные из области применения политики.</span><span class="sxs-lookup"><span data-stu-id="bd037-126">Role IDs excluded from scope of policy.</span></span> |

## <a name="relationships"></a><span data-ttu-id="bd037-127">Связи</span><span class="sxs-lookup"><span data-stu-id="bd037-127">Relationships</span></span>

<span data-ttu-id="bd037-128">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="bd037-128">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="bd037-129">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="bd037-129">JSON representation</span></span>

<span data-ttu-id="bd037-130">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bd037-130">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "includeUsers",
    "excludeUsers",
    "includeGroups",
    "excludeGroups",
    "includeRoles",
    "excludeRoles"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessUsers",
  "baseType": null
}-->

```json
{
  "excludeGroups": ["String"],
  "excludeRoles": ["String"],
  "excludeUsers": ["String"],
  "includeGroups": ["String"],
  "includeRoles": ["String"],
  "includeUsers": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessUsers resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->