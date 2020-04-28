---
title: Тип ресурса Кондитионалакцессусерс
description: Представляет пользователей, группы и роли, включенные в область политики и исключенные из нее.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ad9c41e91a71fa00af71c05bc5c9d0591f81826b
ms.sourcegitcommit: 79988a42d91cc25bdd1c531b5f3261901d720a9a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2020
ms.locfileid: "43916678"
---
# <a name="conditionalaccessusers-resource-type"></a><span data-ttu-id="a463c-103">Тип ресурса Кондитионалакцессусерс</span><span class="sxs-lookup"><span data-stu-id="a463c-103">conditionalAccessUsers resource type</span></span>

<span data-ttu-id="a463c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a463c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a463c-105">Представляет пользователей, группы и роли, включенные в область политики и исключенные из нее.</span><span class="sxs-lookup"><span data-stu-id="a463c-105">Represents users, groups, and roles included in and excluded from the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="a463c-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="a463c-106">Properties</span></span>

| <span data-ttu-id="a463c-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="a463c-107">Property</span></span>     | <span data-ttu-id="a463c-108">Тип</span><span class="sxs-lookup"><span data-stu-id="a463c-108">Type</span></span>        | <span data-ttu-id="a463c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a463c-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="a463c-110">инклудеусерс</span><span class="sxs-lookup"><span data-stu-id="a463c-110">includeUsers</span></span> | <span data-ttu-id="a463c-111">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="a463c-111">String collection</span></span> | <span data-ttu-id="a463c-112">Идентификаторы пользователей в области применения политики, если явно не `None` исключены, `All` или или `GuestsOrExternalUsers`.</span><span class="sxs-lookup"><span data-stu-id="a463c-112">User IDs in scope of policy unless explicitly excluded, or `None` or `All` or `GuestsOrExternalUsers`.</span></span> |
| <span data-ttu-id="a463c-113">ексклудеусерс</span><span class="sxs-lookup"><span data-stu-id="a463c-113">excludeUsers</span></span> | <span data-ttu-id="a463c-114">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="a463c-114">String collection</span></span> | <span data-ttu-id="a463c-115">Идентификаторы пользователей, исключенные из области применения политики `GuestsOrExternalUsers`и/или.</span><span class="sxs-lookup"><span data-stu-id="a463c-115">User IDs excluded from scope of policy and/or `GuestsOrExternalUsers`.</span></span> |
| <span data-ttu-id="a463c-116">инклудеграупс</span><span class="sxs-lookup"><span data-stu-id="a463c-116">includeGroups</span></span> | <span data-ttu-id="a463c-117">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="a463c-117">String collection</span></span> | <span data-ttu-id="a463c-118">Идентификаторы групп в области политики, если явно не исключены, или `All`.</span><span class="sxs-lookup"><span data-stu-id="a463c-118">Group IDs in scope of policy unless explicitly excluded, or `All`.</span></span> |
| <span data-ttu-id="a463c-119">ексклудеграупс</span><span class="sxs-lookup"><span data-stu-id="a463c-119">excludeGroups</span></span> | <span data-ttu-id="a463c-120">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="a463c-120">String collection</span></span> | <span data-ttu-id="a463c-121">Идентификаторы групп, исключенные из области применения политики.</span><span class="sxs-lookup"><span data-stu-id="a463c-121">Group IDs excluded from scope of policy.</span></span> |
| <span data-ttu-id="a463c-122">инклудеролес</span><span class="sxs-lookup"><span data-stu-id="a463c-122">includeRoles</span></span> | <span data-ttu-id="a463c-123">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="a463c-123">String collection</span></span> | <span data-ttu-id="a463c-124">Идентификаторы ролей в области применения политики, если они явно `All`не исключены, или.</span><span class="sxs-lookup"><span data-stu-id="a463c-124">Role IDs in scope of policy unless explicitly excluded, or `All`.</span></span> |
| <span data-ttu-id="a463c-125">ексклудеролес</span><span class="sxs-lookup"><span data-stu-id="a463c-125">excludeRoles</span></span> | <span data-ttu-id="a463c-126">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="a463c-126">String collection</span></span> | <span data-ttu-id="a463c-127">Идентификаторы ролей, исключенные из области применения политики.</span><span class="sxs-lookup"><span data-stu-id="a463c-127">Role IDs excluded from scope of policy.</span></span> |

## <a name="relationships"></a><span data-ttu-id="a463c-128">Связи</span><span class="sxs-lookup"><span data-stu-id="a463c-128">Relationships</span></span>

<span data-ttu-id="a463c-129">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="a463c-129">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a463c-130">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="a463c-130">JSON representation</span></span>

<span data-ttu-id="a463c-131">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a463c-131">The following is a JSON representation of the resource.</span></span>

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