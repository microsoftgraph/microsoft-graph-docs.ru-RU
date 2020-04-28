---
title: Тип ресурса Scopedrolemembership изменен
description: Членство в роли с областью описывает членство пользователя в роли каталога, для которого применяется административная единица (AU).  Это обеспечивает механизм, позволяющий компании, админсистратор на уровне клиента, делегировать административные привилегии пользователю для управления пользователями и группами в подмножестве Организации (подмножества, определяемого службой автоматического управления).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: d5448db2bb73146b3f3e435376ea7b5d708f0474
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520944"
---
# <a name="scopedrolemembership-resource-type"></a><span data-ttu-id="0add6-104">Тип ресурса Scopedrolemembership изменен</span><span class="sxs-lookup"><span data-stu-id="0add6-104">scopedRoleMembership resource type</span></span>

<span data-ttu-id="0add6-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0add6-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0add6-106">Членство в роли с областью описывает членство пользователя в роли каталога, для которого применяется административная единица (AU).</span><span class="sxs-lookup"><span data-stu-id="0add6-106">A scoped-role membership describes a user's membership of a directory role, that is further scoped to an Administrative Unit (AU).</span></span>  <span data-ttu-id="0add6-107">Это обеспечивает механизм, позволяющий компании, админсистратор на уровне клиента, делегировать административные привилегии пользователю для управления пользователями и группами в подмножестве Организации (подмножества, определяемого службой автоматического управления).</span><span class="sxs-lookup"><span data-stu-id="0add6-107">This provides a mechanism to allow a tenant-wide company adminsistrator to delegate administrative privileges to a user to manage users and groups in a subset of the organization (the subset being defined by an AU).</span></span>

## <a name="methods"></a><span data-ttu-id="0add6-108">Methods</span><span class="sxs-lookup"><span data-stu-id="0add6-108">Methods</span></span>
<span data-ttu-id="0add6-109">Прямые запросы к этому ресурсу не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="0add6-109">Direct queries to this resource are not supported.</span></span>  <span data-ttu-id="0add6-110">Ознакомьтесь с разделом [админстративе Units](administrativeunit.md) , чтобы узнать, как запрашивать участие в ролях для ролей, а также добавлять и удалять сведения об участии в ролях.</span><span class="sxs-lookup"><span data-stu-id="0add6-110">Please see the [adminstrative units](administrativeunit.md) topic to see information on how to query for scoped-role memberships, as well as adding and removing scoped-role memberships.</span></span> 

## <a name="properties"></a><span data-ttu-id="0add6-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="0add6-111">Properties</span></span>
| <span data-ttu-id="0add6-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="0add6-112">Property</span></span>   | <span data-ttu-id="0add6-113">Тип</span><span class="sxs-lookup"><span data-stu-id="0add6-113">Type</span></span> | <span data-ttu-id="0add6-114">Описание</span><span class="sxs-lookup"><span data-stu-id="0add6-114">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="0add6-115">административеунитид</span><span class="sxs-lookup"><span data-stu-id="0add6-115">administrativeUnitId</span></span>|<span data-ttu-id="0add6-116">string</span><span class="sxs-lookup"><span data-stu-id="0add6-116">string</span></span>|<span data-ttu-id="0add6-117">Уникальный идентификатор административной единицы, на которую распространяется роль каталога</span><span class="sxs-lookup"><span data-stu-id="0add6-117">Unique identifier for the administrative unit that the directory role is scoped to</span></span>|
|<span data-ttu-id="0add6-118">id</span><span class="sxs-lookup"><span data-stu-id="0add6-118">id</span></span>|<span data-ttu-id="0add6-119">string</span><span class="sxs-lookup"><span data-stu-id="0add6-119">string</span></span>| <span data-ttu-id="0add6-120">Уникальный идентификатор для членства в пределах ролей.</span><span class="sxs-lookup"><span data-stu-id="0add6-120">Unique identifier for the scoped-role membership.</span></span> <span data-ttu-id="0add6-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0add6-121">Read-only.</span></span>|
|<span data-ttu-id="0add6-122">roleId</span><span class="sxs-lookup"><span data-stu-id="0add6-122">roleId</span></span>|<span data-ttu-id="0add6-123">string</span><span class="sxs-lookup"><span data-stu-id="0add6-123">string</span></span>| <span data-ttu-id="0add6-124">Уникальный идентификатор роли каталога, в которой находится член.</span><span class="sxs-lookup"><span data-stu-id="0add6-124">Unique identifier for the directory role that the member is in.</span></span>|
|<span data-ttu-id="0add6-125">roleMemberInfo</span><span class="sxs-lookup"><span data-stu-id="0add6-125">roleMemberInfo</span></span>|[<span data-ttu-id="0add6-126">identity</span><span class="sxs-lookup"><span data-stu-id="0add6-126">identity</span></span>](identity.md)| <span data-ttu-id="0add6-127">Сведения об удостоверении участника роли.</span><span class="sxs-lookup"><span data-stu-id="0add6-127">Role member identity information.</span></span> <span data-ttu-id="0add6-128">Представляет пользователя, который является членом этой области с областью действия.</span><span class="sxs-lookup"><span data-stu-id="0add6-128">Represents the user that is a member of this scoped-role.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0add6-129">Связи</span><span class="sxs-lookup"><span data-stu-id="0add6-129">Relationships</span></span>
<span data-ttu-id="0add6-130">Нет</span><span class="sxs-lookup"><span data-stu-id="0add6-130">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="0add6-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0add6-131">JSON representation</span></span>

<span data-ttu-id="0add6-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0add6-132">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.scopedRoleMembership"
}-->

```json
{
  "administrativeUnitId": "string",
  "id": "string (identifier)",
  "roleId": "string",
  "roleMemberInfo": {"@odata.type": "microsoft.graph.identity"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "scopedRoleMembership resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
