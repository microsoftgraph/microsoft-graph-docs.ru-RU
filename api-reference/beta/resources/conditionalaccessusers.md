---
title: Тип ресурса Кондитионалакцессусерс
description: Представляет пользователей, группы и роли, включенные в область политики и исключенные из нее.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 99fa682b787a164896cb638060798cddee07b255
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43467938"
---
# <a name="conditionalaccessusers-resource-type"></a><span data-ttu-id="3f3fc-103">Тип ресурса Кондитионалакцессусерс</span><span class="sxs-lookup"><span data-stu-id="3f3fc-103">conditionalAccessUsers resource type</span></span>

<span data-ttu-id="3f3fc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3f3fc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3f3fc-105">Представляет пользователей, группы и роли, включенные в область политики и исключенные из нее.</span><span class="sxs-lookup"><span data-stu-id="3f3fc-105">Represents users, groups, and roles included in and excluded from the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="3f3fc-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="3f3fc-106">Properties</span></span>

| <span data-ttu-id="3f3fc-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="3f3fc-107">Property</span></span>     | <span data-ttu-id="3f3fc-108">Тип</span><span class="sxs-lookup"><span data-stu-id="3f3fc-108">Type</span></span>        | <span data-ttu-id="3f3fc-109">Описание</span><span class="sxs-lookup"><span data-stu-id="3f3fc-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="3f3fc-110">инклудеусерс</span><span class="sxs-lookup"><span data-stu-id="3f3fc-110">includeUsers</span></span> | <span data-ttu-id="3f3fc-111">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3f3fc-111">String collection</span></span> | <span data-ttu-id="3f3fc-112">Идентификаторы пользователей в области применения политики, если явно не `None` исключены, `All` или или `GuestsOrExternalUsers`.</span><span class="sxs-lookup"><span data-stu-id="3f3fc-112">User IDs in scope of policy unless explicitly excluded, or `None` or `All` or `GuestsOrExternalUsers`.</span></span> |
| <span data-ttu-id="3f3fc-113">ексклудеусерс</span><span class="sxs-lookup"><span data-stu-id="3f3fc-113">excludeUsers</span></span> | <span data-ttu-id="3f3fc-114">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3f3fc-114">String collection</span></span> | <span data-ttu-id="3f3fc-115">Идентификаторы пользователей, исключенные из области применения политики `GuestsOrExternalUsers`и/или.</span><span class="sxs-lookup"><span data-stu-id="3f3fc-115">User IDs excluded from scope of policy and/or `GuestsOrExternalUsers`.</span></span> |
| <span data-ttu-id="3f3fc-116">инклудеграупс</span><span class="sxs-lookup"><span data-stu-id="3f3fc-116">includeGroups</span></span> | <span data-ttu-id="3f3fc-117">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3f3fc-117">String collection</span></span> | <span data-ttu-id="3f3fc-118">Идентификаторы групп в области политики, если явно не исключены, или `All`.</span><span class="sxs-lookup"><span data-stu-id="3f3fc-118">Group IDs in scope of policy unless explicitly excluded, or `All`.</span></span> |
| <span data-ttu-id="3f3fc-119">ексклудеграупс</span><span class="sxs-lookup"><span data-stu-id="3f3fc-119">excludeGroups</span></span> | <span data-ttu-id="3f3fc-120">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3f3fc-120">String collection</span></span> | <span data-ttu-id="3f3fc-121">Идентификаторы групп, исключенные из области применения политики.</span><span class="sxs-lookup"><span data-stu-id="3f3fc-121">Group IDs excluded from scope of policy.</span></span> |
| <span data-ttu-id="3f3fc-122">инклудеролес</span><span class="sxs-lookup"><span data-stu-id="3f3fc-122">includeRoles</span></span> | <span data-ttu-id="3f3fc-123">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3f3fc-123">String collection</span></span> | <span data-ttu-id="3f3fc-124">Идентификаторы ролей в области применения политики, если они явно `All`не исключены, или.</span><span class="sxs-lookup"><span data-stu-id="3f3fc-124">Role IDs in scope of policy unless explicitly excluded, or `All`.</span></span> |
| <span data-ttu-id="3f3fc-125">ексклудеролес</span><span class="sxs-lookup"><span data-stu-id="3f3fc-125">excludeRoles</span></span> | <span data-ttu-id="3f3fc-126">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3f3fc-126">String collection</span></span> | <span data-ttu-id="3f3fc-127">Идентификаторы ролей, исключенные из области применения политики.</span><span class="sxs-lookup"><span data-stu-id="3f3fc-127">Role IDs excluded from scope of policy.</span></span> |

## <a name="relationships"></a><span data-ttu-id="3f3fc-128">Отношения</span><span class="sxs-lookup"><span data-stu-id="3f3fc-128">Relationships</span></span>

<span data-ttu-id="3f3fc-129">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="3f3fc-129">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3f3fc-130">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="3f3fc-130">JSON representation</span></span>

<span data-ttu-id="3f3fc-131">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3f3fc-131">The following is a JSON representation of the resource.</span></span>

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