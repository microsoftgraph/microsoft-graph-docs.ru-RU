---
title: Тип ресурса conversationMember
description: Представляет пользователя в беседе.
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 17fee8985e2383f0ede652cc1e1a6d8e9dc3304c
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/25/2020
ms.locfileid: "46873458"
---
# <a name="conversationmember-resource-type"></a><span data-ttu-id="db3fd-103">Тип ресурса conversationMember</span><span class="sxs-lookup"><span data-stu-id="db3fd-103">conversationMember resource type</span></span>

<span data-ttu-id="db3fd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="db3fd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db3fd-105">Представляет пользователя в [команде](team.md).</span><span class="sxs-lookup"><span data-stu-id="db3fd-105">Represents a user in a [team](team.md).</span></span>
<span data-ttu-id="db3fd-106">См. также [аадусерконверсатионмембер](aaduserconversationmember.md).</span><span class="sxs-lookup"><span data-stu-id="db3fd-106">See also [aadUserConversationMember](aaduserconversationmember.md).</span></span>

## <a name="properties"></a><span data-ttu-id="db3fd-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="db3fd-107">Properties</span></span>

| <span data-ttu-id="db3fd-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="db3fd-108">Property</span></span>   | <span data-ttu-id="db3fd-109">Тип</span><span class="sxs-lookup"><span data-stu-id="db3fd-109">Type</span></span> |<span data-ttu-id="db3fd-110">Описание</span><span class="sxs-lookup"><span data-stu-id="db3fd-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="db3fd-111">id</span><span class="sxs-lookup"><span data-stu-id="db3fd-111">id</span></span>|<span data-ttu-id="db3fd-112">String</span><span class="sxs-lookup"><span data-stu-id="db3fd-112">String</span></span>| <span data-ttu-id="db3fd-113">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="db3fd-113">Read-only.</span></span> <span data-ttu-id="db3fd-114">Уникальный идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="db3fd-114">Unique ID of the user.</span></span>|
|<span data-ttu-id="db3fd-115">displayName</span><span class="sxs-lookup"><span data-stu-id="db3fd-115">displayName</span></span>| <span data-ttu-id="db3fd-116">string</span><span class="sxs-lookup"><span data-stu-id="db3fd-116">string</span></span> | <span data-ttu-id="db3fd-117">Отображаемое имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="db3fd-117">The display name of the user.</span></span> |
|<span data-ttu-id="db3fd-118">roles</span><span class="sxs-lookup"><span data-stu-id="db3fd-118">roles</span></span>| <span data-ttu-id="db3fd-119">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="db3fd-119">string collection</span></span> | <span data-ttu-id="db3fd-120">Роли этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="db3fd-120">The roles for that user.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="db3fd-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="db3fd-121">JSON representation</span></span>

<span data-ttu-id="db3fd-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="db3fd-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.conversationMember",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "displayName": "String",
  "id": "String (identifier)",
  "roles": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conversationMember resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
