---
title: тип ресурса acl
description: Запись элемента управления доступом для элемента, индексного Поиск (Майкрософт) externalConnection.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 339b5ab51fd604cae2dd42e2ec853ede8d27ef5b
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467832"
---
# <a name="acl-resource-type"></a><span data-ttu-id="503be-103">тип ресурса acl</span><span class="sxs-lookup"><span data-stu-id="503be-103">acl resource type</span></span>

<span data-ttu-id="503be-104">Пространство имен: microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="503be-104">Namespace: microsoft.graph.externalConnectors</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="503be-105">Запись элемента управления доступом для элемента, индексного Поиск (Майкрософт) [externalConnection.](externalconnectors-externalconnection.md)</span><span class="sxs-lookup"><span data-stu-id="503be-105">An access control entry for an item indexed by a Microsoft Search [externalConnection](externalconnectors-externalconnection.md).</span></span>

## <a name="properties"></a><span data-ttu-id="503be-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="503be-106">Properties</span></span>

| <span data-ttu-id="503be-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="503be-107">Property</span></span>       | <span data-ttu-id="503be-108">Тип</span><span class="sxs-lookup"><span data-stu-id="503be-108">Type</span></span>   | <span data-ttu-id="503be-109">Описание</span><span class="sxs-lookup"><span data-stu-id="503be-109">Description</span></span>                                        |
|:---------------|:-------|:---------------------------------------------------|
| <span data-ttu-id="503be-110">accessType</span><span class="sxs-lookup"><span data-stu-id="503be-110">accessType</span></span>     | <span data-ttu-id="503be-111">String</span><span class="sxs-lookup"><span data-stu-id="503be-111">String</span></span> | <span data-ttu-id="503be-112">Доступ, предоставленный удостоверению.</span><span class="sxs-lookup"><span data-stu-id="503be-112">The access granted to the identity.</span></span> <span data-ttu-id="503be-113">Возможные значения: `grant`, `deny`.</span><span class="sxs-lookup"><span data-stu-id="503be-113">Possible values are: `grant`, `deny`.</span></span> |
| <span data-ttu-id="503be-114">identitySource</span><span class="sxs-lookup"><span data-stu-id="503be-114">identitySource</span></span> | <span data-ttu-id="503be-115">String</span><span class="sxs-lookup"><span data-stu-id="503be-115">String</span></span> | <span data-ttu-id="503be-116">Источник удостоверений.</span><span class="sxs-lookup"><span data-stu-id="503be-116">The source of identity.</span></span> <span data-ttu-id="503be-117">Возможные значения: `azureActiveDirectory` или `external`.</span><span class="sxs-lookup"><span data-stu-id="503be-117">Possible values are `azureActiveDirectory` or `external`.</span></span>           |
| <span data-ttu-id="503be-118">type</span><span class="sxs-lookup"><span data-stu-id="503be-118">type</span></span>           | <span data-ttu-id="503be-119">String</span><span class="sxs-lookup"><span data-stu-id="503be-119">String</span></span> | <span data-ttu-id="503be-120">Тип удостоверения.</span><span class="sxs-lookup"><span data-stu-id="503be-120">The type of identity.</span></span> <span data-ttu-id="503be-121">Возможные значения: , , если identitySource есть и только `user` если `group` `everyone` `everyoneExceptGuests` `azureActiveDirectory` `group` identitySource `external` является .</span><span class="sxs-lookup"><span data-stu-id="503be-121">Possible values are: `user`, `group`, `everyone`, `everyoneExceptGuests` if the identitySource is `azureActiveDirectory` and just `group` if the identitySource is `external`.</span></span> |
| <span data-ttu-id="503be-122">value</span><span class="sxs-lookup"><span data-stu-id="503be-122">value</span></span>          | <span data-ttu-id="503be-123">String</span><span class="sxs-lookup"><span data-stu-id="503be-123">String</span></span> | <span data-ttu-id="503be-124">Уникальный идентификатор удостоверения.</span><span class="sxs-lookup"><span data-stu-id="503be-124">The unique identifer of the identity.</span></span> <span data-ttu-id="503be-125">В случае Azure Active Directory удостоверений устанавливается идентификатор объекта пользователя, группы или клиента для пользователей, групп и всех `value` (и всех пользователейExceptGuests) соответственно.</span><span class="sxs-lookup"><span data-stu-id="503be-125">In case of Azure Active Directory identities, `value` is set to the object identifier of the user, group or tenant for types user, group and everyone (and everyoneExceptGuests) respectively.</span></span> <span data-ttu-id="503be-126">В случае внешних `value` групп задают ID [externalGroup](externalconnectors-externalgroup.md).</span><span class="sxs-lookup"><span data-stu-id="503be-126">In case of external groups `value` is set to the ID of the [externalGroup](externalconnectors-externalgroup.md).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="503be-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="503be-127">JSON representation</span></span>

<span data-ttu-id="503be-128">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="503be-128">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalConnectors.acl",
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
