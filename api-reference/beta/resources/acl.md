---
title: Тип ресурса ACL
description: Запись управления доступом для элемента, индексируемого Екстерналконнектион поиска Microsoft Search.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 5a26004cf20a5f8c5c032eeade8f657fdf8bd93c
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/19/2019
ms.locfileid: "38703942"
---
# <a name="acl-resource-type"></a><span data-ttu-id="4a267-103">Тип ресурса ACL</span><span class="sxs-lookup"><span data-stu-id="4a267-103">acl resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4a267-104">Запись управления доступом для элемента, индексируемого [Екстерналконнектион](externalconnection.md)поиска Microsoft Search.</span><span class="sxs-lookup"><span data-stu-id="4a267-104">An access control entry for an item indexed by a Microsoft Search [externalConnection](externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="4a267-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="4a267-105">Properties</span></span>

| <span data-ttu-id="4a267-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="4a267-106">Property</span></span>       | <span data-ttu-id="4a267-107">Тип</span><span class="sxs-lookup"><span data-stu-id="4a267-107">Type</span></span>   | <span data-ttu-id="4a267-108">Описание</span><span class="sxs-lookup"><span data-stu-id="4a267-108">Description</span></span>                                        |
|:---------------|:-------|:---------------------------------------------------|
| <span data-ttu-id="4a267-109">акцесстипе</span><span class="sxs-lookup"><span data-stu-id="4a267-109">accessType</span></span>     | <span data-ttu-id="4a267-110">String</span><span class="sxs-lookup"><span data-stu-id="4a267-110">String</span></span> | <span data-ttu-id="4a267-111">Доступ, назначенный удостоверению.</span><span class="sxs-lookup"><span data-stu-id="4a267-111">The access granted to the identity.</span></span> <span data-ttu-id="4a267-112">Возможные значения: `grant`, `deny`.</span><span class="sxs-lookup"><span data-stu-id="4a267-112">Possible values are: `grant`, `deny`.</span></span> |
| <span data-ttu-id="4a267-113">идентитисаурце</span><span class="sxs-lookup"><span data-stu-id="4a267-113">identitySource</span></span> | <span data-ttu-id="4a267-114">String</span><span class="sxs-lookup"><span data-stu-id="4a267-114">String</span></span> | <span data-ttu-id="4a267-115">Необходимо указать значение `Azure Active Directory`.</span><span class="sxs-lookup"><span data-stu-id="4a267-115">Must be set to `Azure Active Directory`.</span></span>           |
| <span data-ttu-id="4a267-116">type</span><span class="sxs-lookup"><span data-stu-id="4a267-116">type</span></span>           | <span data-ttu-id="4a267-117">String</span><span class="sxs-lookup"><span data-stu-id="4a267-117">String</span></span> | <span data-ttu-id="4a267-118">Тип удостоверения.</span><span class="sxs-lookup"><span data-stu-id="4a267-118">The type of identity.</span></span> <span data-ttu-id="4a267-119">Возможные значения: `user`, `group`, `everyone`, `everyoneExceptGuests`.</span><span class="sxs-lookup"><span data-stu-id="4a267-119">Possible values are: `user`, `group`, `everyone`, `everyoneExceptGuests`.</span></span> |
| <span data-ttu-id="4a267-120">value</span><span class="sxs-lookup"><span data-stu-id="4a267-120">value</span></span>          | <span data-ttu-id="4a267-121">String</span><span class="sxs-lookup"><span data-stu-id="4a267-121">String</span></span> | <span data-ttu-id="4a267-122">Идентификатор Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="4a267-122">The Azure Active Directory identifer.</span></span> <span data-ttu-id="4a267-123">Если `type` задано `group`значение `value` `user` или, для пользователя или группы задан идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="4a267-123">If `type` is `user` or `group`, `value` is set to the object identifier for the user or group.</span></span> <span data-ttu-id="4a267-124">Если `type` задано `everyoneExceptGuests`значение `value` `everyone` или, в качестве идентификатора клиента для клиента Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="4a267-124">If `type` is `everyone` or `everyoneExceptGuests`, `value` is set to the tenant identifier for the Azure Active Directory tenant.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4a267-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4a267-125">JSON representation</span></span>

<span data-ttu-id="4a267-126">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4a267-126">The following is a JSON representation of the resource.</span></span>

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
