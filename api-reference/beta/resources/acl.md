---
title: Тип ресурса ACL
description: Запись управления доступом для элемента, индексируемого Екстерналконнектион поиска Microsoft Search.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 0e94f0442f1c2f7f1a1118f07a4e7a86407eee94
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939118"
---
# <a name="acl-resource-type"></a><span data-ttu-id="df348-103">Тип ресурса ACL</span><span class="sxs-lookup"><span data-stu-id="df348-103">acl resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="df348-104">Запись управления доступом для элемента, индексируемого [Екстерналконнектион](externalconnection.md)поиска Microsoft Search.</span><span class="sxs-lookup"><span data-stu-id="df348-104">An access control entry for an item indexed by a Microsoft Search [externalConnection](externalconnection.md).</span></span>

## <a name="properties"></a><span data-ttu-id="df348-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="df348-105">Properties</span></span>

| <span data-ttu-id="df348-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="df348-106">Property</span></span>       | <span data-ttu-id="df348-107">Тип</span><span class="sxs-lookup"><span data-stu-id="df348-107">Type</span></span>   | <span data-ttu-id="df348-108">Описание</span><span class="sxs-lookup"><span data-stu-id="df348-108">Description</span></span>                                        |
|:---------------|:-------|:---------------------------------------------------|
| <span data-ttu-id="df348-109">акцесстипе</span><span class="sxs-lookup"><span data-stu-id="df348-109">accessType</span></span>     | <span data-ttu-id="df348-110">Строка</span><span class="sxs-lookup"><span data-stu-id="df348-110">String</span></span> | <span data-ttu-id="df348-111">Доступ, назначенный удостоверению.</span><span class="sxs-lookup"><span data-stu-id="df348-111">The access granted to the identity.</span></span> <span data-ttu-id="df348-112">Возможные значения: `grant`, `deny`.</span><span class="sxs-lookup"><span data-stu-id="df348-112">Possible values are: `grant`, `deny`.</span></span> |
| <span data-ttu-id="df348-113">идентитисаурце</span><span class="sxs-lookup"><span data-stu-id="df348-113">identitySource</span></span> | <span data-ttu-id="df348-114">Строка</span><span class="sxs-lookup"><span data-stu-id="df348-114">String</span></span> | <span data-ttu-id="df348-115">Необходимо указать значение `Azure Active Directory`.</span><span class="sxs-lookup"><span data-stu-id="df348-115">Must be set to `Azure Active Directory`.</span></span>           |
| <span data-ttu-id="df348-116">type</span><span class="sxs-lookup"><span data-stu-id="df348-116">type</span></span>           | <span data-ttu-id="df348-117">String</span><span class="sxs-lookup"><span data-stu-id="df348-117">String</span></span> | <span data-ttu-id="df348-118">Тип удостоверения.</span><span class="sxs-lookup"><span data-stu-id="df348-118">The type of identity.</span></span> <span data-ttu-id="df348-119">Возможные значения: `user`, `group`, `everyone`, `everyoneExceptGuests`.</span><span class="sxs-lookup"><span data-stu-id="df348-119">Possible values are: `user`, `group`, `everyone`, `everyoneExceptGuests`.</span></span> |
| <span data-ttu-id="df348-120">value</span><span class="sxs-lookup"><span data-stu-id="df348-120">value</span></span>          | <span data-ttu-id="df348-121">String</span><span class="sxs-lookup"><span data-stu-id="df348-121">String</span></span> | <span data-ttu-id="df348-122">Идентификатор Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="df348-122">The Azure Active Directory identifer.</span></span> <span data-ttu-id="df348-123">Если `type` задано `group`значение `value` `user` или, для пользователя или группы задан идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="df348-123">If `type` is `user` or `group`, `value` is set to the object identifier for the user or group.</span></span> <span data-ttu-id="df348-124">Если `type` задано `everyoneExceptGuests`значение `value` `everyone` или, в качестве идентификатора клиента для клиента Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="df348-124">If `type` is `everyone` or `everyoneExceptGuests`, `value` is set to the tenant identifier for the Azure Active Directory tenant.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="df348-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="df348-125">JSON representation</span></span>

<span data-ttu-id="df348-126">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="df348-126">The following is a JSON representation of the resource.</span></span>

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
