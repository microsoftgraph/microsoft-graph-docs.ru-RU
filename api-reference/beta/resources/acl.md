---
title: Тип ресурса ACL
description: Запись управления доступом для элемента, индексируемого Екстерналконнектион поиска Microsoft Search.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 6d390ac0fee3063bd8f0d292d14e04b2616c1d00
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193535"
---
# <a name="acl-resource-type"></a><span data-ttu-id="47595-103">Тип ресурса ACL</span><span class="sxs-lookup"><span data-stu-id="47595-103">acl resource type</span></span>

<span data-ttu-id="47595-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="47595-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="47595-105">Запись управления доступом для элемента, индексируемого [Екстерналконнектион](externalconnection.md)поиска Microsoft Search.</span><span class="sxs-lookup"><span data-stu-id="47595-105">An access control entry for an item indexed by a Microsoft Search [externalConnection](externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="47595-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="47595-106">Properties</span></span>

| <span data-ttu-id="47595-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="47595-107">Property</span></span>       | <span data-ttu-id="47595-108">Тип</span><span class="sxs-lookup"><span data-stu-id="47595-108">Type</span></span>   | <span data-ttu-id="47595-109">Описание</span><span class="sxs-lookup"><span data-stu-id="47595-109">Description</span></span>                                        |
|:---------------|:-------|:---------------------------------------------------|
| <span data-ttu-id="47595-110">акцесстипе</span><span class="sxs-lookup"><span data-stu-id="47595-110">accessType</span></span>     | <span data-ttu-id="47595-111">String</span><span class="sxs-lookup"><span data-stu-id="47595-111">String</span></span> | <span data-ttu-id="47595-112">Доступ, назначенный удостоверению.</span><span class="sxs-lookup"><span data-stu-id="47595-112">The access granted to the identity.</span></span> <span data-ttu-id="47595-113">Возможные значения: `grant`, `deny`.</span><span class="sxs-lookup"><span data-stu-id="47595-113">Possible values are: `grant`, `deny`.</span></span> |
| <span data-ttu-id="47595-114">идентитисаурце</span><span class="sxs-lookup"><span data-stu-id="47595-114">identitySource</span></span> | <span data-ttu-id="47595-115">String</span><span class="sxs-lookup"><span data-stu-id="47595-115">String</span></span> | <span data-ttu-id="47595-116">Источник удостоверения.</span><span class="sxs-lookup"><span data-stu-id="47595-116">The source of identity.</span></span> <span data-ttu-id="47595-117">Возможные значения: `azureActiveDirectory` или `external` .</span><span class="sxs-lookup"><span data-stu-id="47595-117">Possible values are `azureActiveDirectory` or `external`.</span></span>           |
| <span data-ttu-id="47595-118">type</span><span class="sxs-lookup"><span data-stu-id="47595-118">type</span></span>           | <span data-ttu-id="47595-119">String</span><span class="sxs-lookup"><span data-stu-id="47595-119">String</span></span> | <span data-ttu-id="47595-120">Тип удостоверения.</span><span class="sxs-lookup"><span data-stu-id="47595-120">The type of identity.</span></span> <span data-ttu-id="47595-121">Возможные значения: `user` , `group` ,, `everyone` `everyoneExceptGuests` Если идентитисаурце, `azureActiveDirectory` и только в том `group` случае, если идентитисаурце `external` .</span><span class="sxs-lookup"><span data-stu-id="47595-121">Possible values are: `user`, `group`, `everyone`, `everyoneExceptGuests` if the identitySource is `azureActiveDirectory` and just `group` if the identitySource is `external`.</span></span> |
| <span data-ttu-id="47595-122">value</span><span class="sxs-lookup"><span data-stu-id="47595-122">value</span></span>          | <span data-ttu-id="47595-123">String</span><span class="sxs-lookup"><span data-stu-id="47595-123">String</span></span> | <span data-ttu-id="47595-124">Уникальный идентификатор удостоверения.</span><span class="sxs-lookup"><span data-stu-id="47595-124">The unique identifer of the identity.</span></span> <span data-ttu-id="47595-125">В случае удостоверений Azure Active Directory `value` для этого параметра задается идентификатор объекта пользователя, группы или клиента для типов User, Group и Everyone (and еверйониксцептгуестс) соответственно.</span><span class="sxs-lookup"><span data-stu-id="47595-125">In case of Azure Active Directory identities, `value` is set to the object identifier of the user, group or tenant for types user, group and everyone (and everyoneExceptGuests) respectively.</span></span> <span data-ttu-id="47595-126">В случае внешних групп `value` задается идентификатор [екстерналграуп](externalgroup.md).</span><span class="sxs-lookup"><span data-stu-id="47595-126">In case of external groups `value` is set to the ID of the [externalGroup](externalgroup.md).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="47595-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="47595-127">JSON representation</span></span>

<span data-ttu-id="47595-128">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="47595-128">The following is a JSON representation of the resource.</span></span>

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
