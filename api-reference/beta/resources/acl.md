---
title: тип ресурса acl
description: Запись элемента управления доступом для элемента, индексного Поиск (Майкрософт) externalConnection.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: d4c3f3cc72c7fde56665c33561fa435e76842eb1
ms.sourcegitcommit: 3873c85f53e026073addca92d31d234af244444c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/10/2021
ms.locfileid: "53366599"
---
# <a name="acl-resource-type"></a><span data-ttu-id="e9caa-103">тип ресурса acl</span><span class="sxs-lookup"><span data-stu-id="e9caa-103">acl resource type</span></span>

<span data-ttu-id="e9caa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e9caa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e9caa-105">Запись элемента управления доступом для элемента, индексного Поиск (Майкрософт) [externalConnection.](externalconnection.md)</span><span class="sxs-lookup"><span data-stu-id="e9caa-105">An access control entry for an item indexed by a Microsoft Search [externalConnection](externalconnection.md).</span></span>

## <a name="properties"></a><span data-ttu-id="e9caa-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="e9caa-106">Properties</span></span>

| <span data-ttu-id="e9caa-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="e9caa-107">Property</span></span>       | <span data-ttu-id="e9caa-108">Тип</span><span class="sxs-lookup"><span data-stu-id="e9caa-108">Type</span></span>   | <span data-ttu-id="e9caa-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e9caa-109">Description</span></span>                                        |
|:---------------|:-------|:---------------------------------------------------|
| <span data-ttu-id="e9caa-110">accessType</span><span class="sxs-lookup"><span data-stu-id="e9caa-110">accessType</span></span>     | <span data-ttu-id="e9caa-111">String</span><span class="sxs-lookup"><span data-stu-id="e9caa-111">String</span></span> | <span data-ttu-id="e9caa-112">Доступ, предоставленный удостоверению.</span><span class="sxs-lookup"><span data-stu-id="e9caa-112">The access granted to the identity.</span></span> <span data-ttu-id="e9caa-113">Возможные значения: `grant`, `deny`.</span><span class="sxs-lookup"><span data-stu-id="e9caa-113">Possible values are: `grant`, `deny`.</span></span> |
| <span data-ttu-id="e9caa-114">identitySource</span><span class="sxs-lookup"><span data-stu-id="e9caa-114">identitySource</span></span> | <span data-ttu-id="e9caa-115">String</span><span class="sxs-lookup"><span data-stu-id="e9caa-115">String</span></span> | <span data-ttu-id="e9caa-116">Источник удостоверений.</span><span class="sxs-lookup"><span data-stu-id="e9caa-116">The source of identity.</span></span> <span data-ttu-id="e9caa-117">Возможные значения: `azureActiveDirectory` или `external`.</span><span class="sxs-lookup"><span data-stu-id="e9caa-117">Possible values are `azureActiveDirectory` or `external`.</span></span>           |
| <span data-ttu-id="e9caa-118">type</span><span class="sxs-lookup"><span data-stu-id="e9caa-118">type</span></span>           | <span data-ttu-id="e9caa-119">String</span><span class="sxs-lookup"><span data-stu-id="e9caa-119">String</span></span> | <span data-ttu-id="e9caa-120">Тип удостоверения.</span><span class="sxs-lookup"><span data-stu-id="e9caa-120">The type of identity.</span></span> <span data-ttu-id="e9caa-121">Возможные значения: , , если identitySource есть и только `user` если `group` `everyone` `everyoneExceptGuests` `azureActiveDirectory` `group` identitySource `external` является .</span><span class="sxs-lookup"><span data-stu-id="e9caa-121">Possible values are: `user`, `group`, `everyone`, `everyoneExceptGuests` if the identitySource is `azureActiveDirectory` and just `group` if the identitySource is `external`.</span></span> |
| <span data-ttu-id="e9caa-122">value</span><span class="sxs-lookup"><span data-stu-id="e9caa-122">value</span></span>          | <span data-ttu-id="e9caa-123">String</span><span class="sxs-lookup"><span data-stu-id="e9caa-123">String</span></span> | <span data-ttu-id="e9caa-124">Уникальный идентификатор удостоверения.</span><span class="sxs-lookup"><span data-stu-id="e9caa-124">The unique identifer of the identity.</span></span> <span data-ttu-id="e9caa-125">В случае Azure Active Directory удостоверений устанавливается идентификатор объекта пользователя, группы или клиента для пользователей, групп и всех `value` (и всех пользователейExceptGuests) соответственно.</span><span class="sxs-lookup"><span data-stu-id="e9caa-125">In case of Azure Active Directory identities, `value` is set to the object identifier of the user, group or tenant for types user, group and everyone (and everyoneExceptGuests) respectively.</span></span> <span data-ttu-id="e9caa-126">В случае внешних `value` групп задают ID [externalGroup](externalgroup.md).</span><span class="sxs-lookup"><span data-stu-id="e9caa-126">In case of external groups `value` is set to the ID of the [externalGroup](externalgroup.md).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e9caa-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e9caa-127">JSON representation</span></span>

<span data-ttu-id="e9caa-128">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e9caa-128">The following is a JSON representation of the resource.</span></span>

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
