---
title: Тип ресурса ACL
description: Запись управления доступом для элемента, индексируемого Екстерналконнектион поиска Microsoft Search.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: d0745ab4a04233a654b829da8f93defb855fc0f9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48024558"
---
# <a name="acl-resource-type"></a><span data-ttu-id="59549-103">Тип ресурса ACL</span><span class="sxs-lookup"><span data-stu-id="59549-103">acl resource type</span></span>

<span data-ttu-id="59549-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="59549-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59549-105">Запись управления доступом для элемента, индексируемого [Екстерналконнектион](externalconnection.md)поиска Microsoft Search.</span><span class="sxs-lookup"><span data-stu-id="59549-105">An access control entry for an item indexed by a Microsoft Search [externalConnection](externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="59549-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="59549-106">Properties</span></span>

| <span data-ttu-id="59549-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="59549-107">Property</span></span>       | <span data-ttu-id="59549-108">Тип</span><span class="sxs-lookup"><span data-stu-id="59549-108">Type</span></span>   | <span data-ttu-id="59549-109">Описание</span><span class="sxs-lookup"><span data-stu-id="59549-109">Description</span></span>                                        |
|:---------------|:-------|:---------------------------------------------------|
| <span data-ttu-id="59549-110">акцесстипе</span><span class="sxs-lookup"><span data-stu-id="59549-110">accessType</span></span>     | <span data-ttu-id="59549-111">String</span><span class="sxs-lookup"><span data-stu-id="59549-111">String</span></span> | <span data-ttu-id="59549-112">Доступ, назначенный удостоверению.</span><span class="sxs-lookup"><span data-stu-id="59549-112">The access granted to the identity.</span></span> <span data-ttu-id="59549-113">Возможные значения: `grant`, `deny`.</span><span class="sxs-lookup"><span data-stu-id="59549-113">Possible values are: `grant`, `deny`.</span></span> |
| <span data-ttu-id="59549-114">идентитисаурце</span><span class="sxs-lookup"><span data-stu-id="59549-114">identitySource</span></span> | <span data-ttu-id="59549-115">String</span><span class="sxs-lookup"><span data-stu-id="59549-115">String</span></span> | <span data-ttu-id="59549-116">Необходимо указать значение `Azure Active Directory`.</span><span class="sxs-lookup"><span data-stu-id="59549-116">Must be set to `Azure Active Directory`.</span></span>           |
| <span data-ttu-id="59549-117">type</span><span class="sxs-lookup"><span data-stu-id="59549-117">type</span></span>           | <span data-ttu-id="59549-118">String</span><span class="sxs-lookup"><span data-stu-id="59549-118">String</span></span> | <span data-ttu-id="59549-119">Тип удостоверения.</span><span class="sxs-lookup"><span data-stu-id="59549-119">The type of identity.</span></span> <span data-ttu-id="59549-120">Возможные значения: `user`, `group`, `everyone`, `everyoneExceptGuests`.</span><span class="sxs-lookup"><span data-stu-id="59549-120">Possible values are: `user`, `group`, `everyone`, `everyoneExceptGuests`.</span></span> |
| <span data-ttu-id="59549-121">value</span><span class="sxs-lookup"><span data-stu-id="59549-121">value</span></span>          | <span data-ttu-id="59549-122">String</span><span class="sxs-lookup"><span data-stu-id="59549-122">String</span></span> | <span data-ttu-id="59549-123">Идентификатор Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="59549-123">The Azure Active Directory identifer.</span></span> <span data-ttu-id="59549-124">Если задано значение `type` `user` или `group` , `value` для пользователя или группы задан идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="59549-124">If `type` is `user` or `group`, `value` is set to the object identifier for the user or group.</span></span> <span data-ttu-id="59549-125">Если задано значение `type` `everyone` или `everyoneExceptGuests` , `value` в качестве идентификатора клиента для клиента Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="59549-125">If `type` is `everyone` or `everyoneExceptGuests`, `value` is set to the tenant identifier for the Azure Active Directory tenant.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="59549-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="59549-126">JSON representation</span></span>

<span data-ttu-id="59549-127">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="59549-127">The following is a JSON representation of the resource.</span></span>

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


