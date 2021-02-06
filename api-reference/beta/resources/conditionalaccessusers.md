---
title: Тип ресурса conditionalAccessUsers
description: Представляет пользователей, группы и роли, включенные в область политики и исключенные из нее.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 6214c3daacf580aaffa01a93be2b2c785c03f4fd
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128584"
---
# <a name="conditionalaccessusers-resource-type"></a><span data-ttu-id="a2477-103">Тип ресурса conditionalAccessUsers</span><span class="sxs-lookup"><span data-stu-id="a2477-103">conditionalAccessUsers resource type</span></span>

<span data-ttu-id="a2477-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2477-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a2477-105">Представляет пользователей, группы и роли, включенные в область политики и исключенные из нее.</span><span class="sxs-lookup"><span data-stu-id="a2477-105">Represents users, groups, and roles included in and excluded from the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="a2477-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="a2477-106">Properties</span></span>

| <span data-ttu-id="a2477-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="a2477-107">Property</span></span>     | <span data-ttu-id="a2477-108">Тип</span><span class="sxs-lookup"><span data-stu-id="a2477-108">Type</span></span>        | <span data-ttu-id="a2477-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a2477-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="a2477-110">includeUsers</span><span class="sxs-lookup"><span data-stu-id="a2477-110">includeUsers</span></span> | <span data-ttu-id="a2477-111">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="a2477-111">String collection</span></span> | <span data-ttu-id="a2477-112">User IDs in scope of policy unless explicitly excluded, or `None` or `All` or `GuestsOrExternalUsers` .</span><span class="sxs-lookup"><span data-stu-id="a2477-112">User IDs in scope of policy unless explicitly excluded, or `None` or `All` or `GuestsOrExternalUsers`.</span></span> |
| <span data-ttu-id="a2477-113">excludeUsers</span><span class="sxs-lookup"><span data-stu-id="a2477-113">excludeUsers</span></span> | <span data-ttu-id="a2477-114">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="a2477-114">String collection</span></span> | <span data-ttu-id="a2477-115">User IDs excluded from scope of policy and/or `GuestsOrExternalUsers` .</span><span class="sxs-lookup"><span data-stu-id="a2477-115">User IDs excluded from scope of policy and/or `GuestsOrExternalUsers`.</span></span> |
| <span data-ttu-id="a2477-116">includeGroups</span><span class="sxs-lookup"><span data-stu-id="a2477-116">includeGroups</span></span> | <span data-ttu-id="a2477-117">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="a2477-117">String collection</span></span> | <span data-ttu-id="a2477-118">Групповые ИД в области политики, если явно не исключены, или `All` .</span><span class="sxs-lookup"><span data-stu-id="a2477-118">Group IDs in scope of policy unless explicitly excluded, or `All`.</span></span> |
| <span data-ttu-id="a2477-119">excludeGroups</span><span class="sxs-lookup"><span data-stu-id="a2477-119">excludeGroups</span></span> | <span data-ttu-id="a2477-120">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="a2477-120">String collection</span></span> | <span data-ttu-id="a2477-121">ИД группы, исключенные из области действия политики.</span><span class="sxs-lookup"><span data-stu-id="a2477-121">Group IDs excluded from scope of policy.</span></span> |
| <span data-ttu-id="a2477-122">includeRoles</span><span class="sxs-lookup"><span data-stu-id="a2477-122">includeRoles</span></span> | <span data-ttu-id="a2477-123">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="a2477-123">String collection</span></span> | <span data-ttu-id="a2477-124">ИД ролей в области политики, если явно не исключено, или `All` .</span><span class="sxs-lookup"><span data-stu-id="a2477-124">Role IDs in scope of policy unless explicitly excluded, or `All`.</span></span> |
| <span data-ttu-id="a2477-125">excludeRoles</span><span class="sxs-lookup"><span data-stu-id="a2477-125">excludeRoles</span></span> | <span data-ttu-id="a2477-126">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="a2477-126">String collection</span></span> | <span data-ttu-id="a2477-127">ИД ролей, исключенные из области действия политики.</span><span class="sxs-lookup"><span data-stu-id="a2477-127">Role IDs excluded from scope of policy.</span></span> |

## <a name="relationships"></a><span data-ttu-id="a2477-128">Связи</span><span class="sxs-lookup"><span data-stu-id="a2477-128">Relationships</span></span>

<span data-ttu-id="a2477-129">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="a2477-129">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a2477-130">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="a2477-130">JSON representation</span></span>

<span data-ttu-id="a2477-131">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a2477-131">The following is a JSON representation of the resource.</span></span>

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

