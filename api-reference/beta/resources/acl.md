---
title: Тип ресурса ACL
description: Запись управления доступом для элемента, индексируемого Екстерналконнектион поиска Microsoft Search.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: a957feaffe36e76a36958ef7855376bcfe58484e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508452"
---
# <a name="acl-resource-type"></a><span data-ttu-id="e6afa-103">Тип ресурса ACL</span><span class="sxs-lookup"><span data-stu-id="e6afa-103">acl resource type</span></span>

<span data-ttu-id="e6afa-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="e6afa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e6afa-105">Запись управления доступом для элемента, индексируемого [Екстерналконнектион](externalconnection.md)поиска Microsoft Search.</span><span class="sxs-lookup"><span data-stu-id="e6afa-105">An access control entry for an item indexed by a Microsoft Search [externalConnection](externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="e6afa-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="e6afa-106">Properties</span></span>

| <span data-ttu-id="e6afa-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="e6afa-107">Property</span></span>       | <span data-ttu-id="e6afa-108">Тип</span><span class="sxs-lookup"><span data-stu-id="e6afa-108">Type</span></span>   | <span data-ttu-id="e6afa-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e6afa-109">Description</span></span>                                        |
|:---------------|:-------|:---------------------------------------------------|
| <span data-ttu-id="e6afa-110">акцесстипе</span><span class="sxs-lookup"><span data-stu-id="e6afa-110">accessType</span></span>     | <span data-ttu-id="e6afa-111">String</span><span class="sxs-lookup"><span data-stu-id="e6afa-111">String</span></span> | <span data-ttu-id="e6afa-112">Доступ, назначенный удостоверению.</span><span class="sxs-lookup"><span data-stu-id="e6afa-112">The access granted to the identity.</span></span> <span data-ttu-id="e6afa-113">Возможные значения: `grant`, `deny`.</span><span class="sxs-lookup"><span data-stu-id="e6afa-113">Possible values are: `grant`, `deny`.</span></span> |
| <span data-ttu-id="e6afa-114">идентитисаурце</span><span class="sxs-lookup"><span data-stu-id="e6afa-114">identitySource</span></span> | <span data-ttu-id="e6afa-115">String</span><span class="sxs-lookup"><span data-stu-id="e6afa-115">String</span></span> | <span data-ttu-id="e6afa-116">Необходимо указать значение `Azure Active Directory`.</span><span class="sxs-lookup"><span data-stu-id="e6afa-116">Must be set to `Azure Active Directory`.</span></span>           |
| <span data-ttu-id="e6afa-117">type</span><span class="sxs-lookup"><span data-stu-id="e6afa-117">type</span></span>           | <span data-ttu-id="e6afa-118">String</span><span class="sxs-lookup"><span data-stu-id="e6afa-118">String</span></span> | <span data-ttu-id="e6afa-119">Тип удостоверения.</span><span class="sxs-lookup"><span data-stu-id="e6afa-119">The type of identity.</span></span> <span data-ttu-id="e6afa-120">Возможные значения: `user`, `group`, `everyone`, `everyoneExceptGuests`.</span><span class="sxs-lookup"><span data-stu-id="e6afa-120">Possible values are: `user`, `group`, `everyone`, `everyoneExceptGuests`.</span></span> |
| <span data-ttu-id="e6afa-121">value</span><span class="sxs-lookup"><span data-stu-id="e6afa-121">value</span></span>          | <span data-ttu-id="e6afa-122">String</span><span class="sxs-lookup"><span data-stu-id="e6afa-122">String</span></span> | <span data-ttu-id="e6afa-123">Идентификатор Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="e6afa-123">The Azure Active Directory identifer.</span></span> <span data-ttu-id="e6afa-124">Если `type` задано `group`значение `value` `user` или, для пользователя или группы задан идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="e6afa-124">If `type` is `user` or `group`, `value` is set to the object identifier for the user or group.</span></span> <span data-ttu-id="e6afa-125">Если `type` задано `everyoneExceptGuests`значение `value` `everyone` или, в качестве идентификатора клиента для клиента Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="e6afa-125">If `type` is `everyone` or `everyoneExceptGuests`, `value` is set to the tenant identifier for the Azure Active Directory tenant.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e6afa-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e6afa-126">JSON representation</span></span>

<span data-ttu-id="e6afa-127">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e6afa-127">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.acl",
  "baseType": null
}-->

```json
{
  "accessType": "String",
  "identitySource": "String",
  "type": "String",
  "value": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "acl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
