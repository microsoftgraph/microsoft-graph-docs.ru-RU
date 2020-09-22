---
title: Тип ресурса conversationMember
description: Представляет пользователя в беседе.
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: e2c888ea55b331762761857c14b4710bf582be3f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48056928"
---
# <a name="conversationmember-resource-type"></a><span data-ttu-id="1ecca-103">Тип ресурса conversationMember</span><span class="sxs-lookup"><span data-stu-id="1ecca-103">conversationMember resource type</span></span>

<span data-ttu-id="1ecca-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1ecca-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1ecca-105">Представляет пользователя в [команде](team.md).</span><span class="sxs-lookup"><span data-stu-id="1ecca-105">Represents a user in a [team](team.md).</span></span>
<span data-ttu-id="1ecca-106">См. также [аадусерконверсатионмембер](aaduserconversationmember.md).</span><span class="sxs-lookup"><span data-stu-id="1ecca-106">See also [aadUserConversationMember](aaduserconversationmember.md).</span></span>

## <a name="properties"></a><span data-ttu-id="1ecca-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="1ecca-107">Properties</span></span>

| <span data-ttu-id="1ecca-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="1ecca-108">Property</span></span>   | <span data-ttu-id="1ecca-109">Тип</span><span class="sxs-lookup"><span data-stu-id="1ecca-109">Type</span></span> |<span data-ttu-id="1ecca-110">Описание</span><span class="sxs-lookup"><span data-stu-id="1ecca-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1ecca-111">id</span><span class="sxs-lookup"><span data-stu-id="1ecca-111">id</span></span>|<span data-ttu-id="1ecca-112">String</span><span class="sxs-lookup"><span data-stu-id="1ecca-112">String</span></span>| <span data-ttu-id="1ecca-113">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1ecca-113">Read-only.</span></span> <span data-ttu-id="1ecca-114">Уникальный идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="1ecca-114">Unique ID of the user.</span></span>|
|<span data-ttu-id="1ecca-115">displayName</span><span class="sxs-lookup"><span data-stu-id="1ecca-115">displayName</span></span>| <span data-ttu-id="1ecca-116">string</span><span class="sxs-lookup"><span data-stu-id="1ecca-116">string</span></span> | <span data-ttu-id="1ecca-117">Отображаемое имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="1ecca-117">The display name of the user.</span></span> |
|<span data-ttu-id="1ecca-118">roles</span><span class="sxs-lookup"><span data-stu-id="1ecca-118">roles</span></span>| <span data-ttu-id="1ecca-119">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="1ecca-119">string collection</span></span> | <span data-ttu-id="1ecca-120">Роли этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="1ecca-120">The roles for that user.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1ecca-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1ecca-121">JSON representation</span></span>

<span data-ttu-id="1ecca-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1ecca-122">The following is a JSON representation of the resource.</span></span>

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

