---
title: Тип ресурса conditionalAccessUsers
description: Представляет пользователей, группы и роли, включенные в область политики и исключенные из нее.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 8f75eb86ab9627b2cb9d507de9321743524203b3
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50129774"
---
# <a name="conditionalaccessusers-resource-type"></a><span data-ttu-id="b22fa-103">Тип ресурса conditionalAccessUsers</span><span class="sxs-lookup"><span data-stu-id="b22fa-103">conditionalAccessUsers resource type</span></span>

<span data-ttu-id="b22fa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b22fa-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b22fa-105">Представляет пользователей, группы и роли, включенные в область политики и исключенные из нее.</span><span class="sxs-lookup"><span data-stu-id="b22fa-105">Represents users, groups, and roles included in and excluded from the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="b22fa-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="b22fa-106">Properties</span></span>

| <span data-ttu-id="b22fa-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="b22fa-107">Property</span></span>     | <span data-ttu-id="b22fa-108">Тип</span><span class="sxs-lookup"><span data-stu-id="b22fa-108">Type</span></span>        | <span data-ttu-id="b22fa-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b22fa-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="b22fa-110">includeUsers</span><span class="sxs-lookup"><span data-stu-id="b22fa-110">includeUsers</span></span> | <span data-ttu-id="b22fa-111">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="b22fa-111">String collection</span></span> | <span data-ttu-id="b22fa-112">User IDs in scope of policy unless explicitly excluded, or `None` `All` or or `GuestsOrExternalUsers` .</span><span class="sxs-lookup"><span data-stu-id="b22fa-112">User IDs in scope of policy unless explicitly excluded, or `None` or `All` or `GuestsOrExternalUsers`.</span></span> |
| <span data-ttu-id="b22fa-113">excludeUsers</span><span class="sxs-lookup"><span data-stu-id="b22fa-113">excludeUsers</span></span> | <span data-ttu-id="b22fa-114">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="b22fa-114">String collection</span></span> | <span data-ttu-id="b22fa-115">ИД пользователей, исключенных из области действия политики и/или `GuestsOrExternalUsers` .</span><span class="sxs-lookup"><span data-stu-id="b22fa-115">User IDs excluded from scope of policy and/or `GuestsOrExternalUsers`.</span></span> |
| <span data-ttu-id="b22fa-116">includeGroups</span><span class="sxs-lookup"><span data-stu-id="b22fa-116">includeGroups</span></span> | <span data-ttu-id="b22fa-117">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="b22fa-117">String collection</span></span> | <span data-ttu-id="b22fa-118">Групповые ИД в области политики, если явно не исключены, или `All` .</span><span class="sxs-lookup"><span data-stu-id="b22fa-118">Group IDs in scope of policy unless explicitly excluded, or `All`.</span></span> |
| <span data-ttu-id="b22fa-119">excludeGroups</span><span class="sxs-lookup"><span data-stu-id="b22fa-119">excludeGroups</span></span> | <span data-ttu-id="b22fa-120">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="b22fa-120">String collection</span></span> | <span data-ttu-id="b22fa-121">ИД группы, исключенные из области действия политики.</span><span class="sxs-lookup"><span data-stu-id="b22fa-121">Group IDs excluded from scope of policy.</span></span> |
| <span data-ttu-id="b22fa-122">includeRoles</span><span class="sxs-lookup"><span data-stu-id="b22fa-122">includeRoles</span></span> | <span data-ttu-id="b22fa-123">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="b22fa-123">String collection</span></span> | <span data-ttu-id="b22fa-124">ИД ролей в области политики, если явно не исключено, или `All` .</span><span class="sxs-lookup"><span data-stu-id="b22fa-124">Role IDs in scope of policy unless explicitly excluded, or `All`.</span></span> |
| <span data-ttu-id="b22fa-125">excludeRoles</span><span class="sxs-lookup"><span data-stu-id="b22fa-125">excludeRoles</span></span> | <span data-ttu-id="b22fa-126">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="b22fa-126">String collection</span></span> | <span data-ttu-id="b22fa-127">ИД ролей, исключенные из области действия политики.</span><span class="sxs-lookup"><span data-stu-id="b22fa-127">Role IDs excluded from scope of policy.</span></span> |

## <a name="relationships"></a><span data-ttu-id="b22fa-128">Связи</span><span class="sxs-lookup"><span data-stu-id="b22fa-128">Relationships</span></span>

<span data-ttu-id="b22fa-129">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="b22fa-129">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b22fa-130">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="b22fa-130">JSON representation</span></span>

<span data-ttu-id="b22fa-131">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b22fa-131">The following is a JSON representation of the resource.</span></span>

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

