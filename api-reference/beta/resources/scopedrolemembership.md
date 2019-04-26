---
title: Тип ресурса Scopedrolemembership изменен
description: Членство В роли С областью описывает членство пользователя в роли каталога, для которого применяется административная единица (AU).  Это обеспечивает механизм, позволяющий компании, админсистратор на уровне клиента, делегировать административные привилегии пользователю для управления пользователями и группами в подмножестве Организации (подмножества, определяемого службой автоматического управления).
localization_priority: Normal
ms.openlocfilehash: 56a2514fa65033154b6ab69c497c90fde201c28e
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343474"
---
# <a name="scopedrolemembership-resource-type"></a><span data-ttu-id="d722e-104">Тип ресурса Scopedrolemembership изменен</span><span class="sxs-lookup"><span data-stu-id="d722e-104">scopedRoleMembership resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d722e-105">Членство В роли С областью описывает членство пользователя в роли каталога, для которого применяется административная единица (AU).</span><span class="sxs-lookup"><span data-stu-id="d722e-105">A scoped-role membership describes a user's membership of a directory role, that is further scoped to an Administrative Unit (AU).</span></span>  <span data-ttu-id="d722e-106">Это обеспечивает механизм, позволяющий компании, админсистратор на уровне клиента, делегировать административные привилегии пользователю для управления пользователями и группами в подмножестве Организации (подмножества, определяемого службой автоматического управления).</span><span class="sxs-lookup"><span data-stu-id="d722e-106">This provides a mechanism to allow a tenant-wide company adminsistrator to delegate administrative privileges to a user to manage users and groups in a subset of the organization (the subset being defined by an AU).</span></span>

## <a name="methods"></a><span data-ttu-id="d722e-107">Методы</span><span class="sxs-lookup"><span data-stu-id="d722e-107">Methods</span></span>
<span data-ttu-id="d722e-108">Прямые запросы к этому ресурсу не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="d722e-108">Direct queries to this resource are not supported.</span></span>  <span data-ttu-id="d722e-109">Ознакомьтесь с разделом [админстративе Units](administrativeunit.md) , чтобы узнать, как запрашивать участие в ролях для ролей, а также добавлять и удалять сведения об участии в ролях.</span><span class="sxs-lookup"><span data-stu-id="d722e-109">Please see the [adminstrative units](administrativeunit.md) topic to see information on how to query for scoped-role memberships, as well as adding and removing scoped-role memberships.</span></span> 

## <a name="properties"></a><span data-ttu-id="d722e-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="d722e-110">Properties</span></span>
| <span data-ttu-id="d722e-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="d722e-111">Property</span></span>   | <span data-ttu-id="d722e-112">Тип</span><span class="sxs-lookup"><span data-stu-id="d722e-112">Type</span></span> | <span data-ttu-id="d722e-113">Описание</span><span class="sxs-lookup"><span data-stu-id="d722e-113">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="d722e-114">Административеунитид</span><span class="sxs-lookup"><span data-stu-id="d722e-114">administrativeUnitId</span></span>|<span data-ttu-id="d722e-115">string</span><span class="sxs-lookup"><span data-stu-id="d722e-115">string</span></span>|<span data-ttu-id="d722e-116">Уникальный идентификатор административной единицы, на которую распространяется роль каталога</span><span class="sxs-lookup"><span data-stu-id="d722e-116">Unique identifier for the administrative unit that the directory role is scoped to</span></span>|
|<span data-ttu-id="d722e-117">id</span><span class="sxs-lookup"><span data-stu-id="d722e-117">id</span></span>|<span data-ttu-id="d722e-118">string</span><span class="sxs-lookup"><span data-stu-id="d722e-118">string</span></span>| <span data-ttu-id="d722e-119">Уникальный идентификатор для членства в пределах ролей.</span><span class="sxs-lookup"><span data-stu-id="d722e-119">Unique identifier for the scoped-role membership.</span></span> <span data-ttu-id="d722e-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d722e-120">Read-only.</span></span>|
|<span data-ttu-id="d722e-121">roleId</span><span class="sxs-lookup"><span data-stu-id="d722e-121">roleId</span></span>|<span data-ttu-id="d722e-122">string</span><span class="sxs-lookup"><span data-stu-id="d722e-122">string</span></span>| <span data-ttu-id="d722e-123">Уникальный идентификатор роли каталога, в которой находится член.</span><span class="sxs-lookup"><span data-stu-id="d722e-123">Unique identifier for the directory role that the member is in.</span></span>|
|<span data-ttu-id="d722e-124">roleMemberInfo</span><span class="sxs-lookup"><span data-stu-id="d722e-124">roleMemberInfo</span></span>|[<span data-ttu-id="d722e-125">identity</span><span class="sxs-lookup"><span data-stu-id="d722e-125">identity</span></span>](identity.md)| <span data-ttu-id="d722e-126">Сведения об удостоверении участника роли.</span><span class="sxs-lookup"><span data-stu-id="d722e-126">Role member identity information.</span></span> <span data-ttu-id="d722e-127">Представляет пользователя, который является членом этой области с областью действия.</span><span class="sxs-lookup"><span data-stu-id="d722e-127">Represents the user that is a member of this scoped-role.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d722e-128">Связи</span><span class="sxs-lookup"><span data-stu-id="d722e-128">Relationships</span></span>
<span data-ttu-id="d722e-129">Нет</span><span class="sxs-lookup"><span data-stu-id="d722e-129">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="d722e-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d722e-130">JSON representation</span></span>

<span data-ttu-id="d722e-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d722e-131">Here is a JSON representation of the resource.</span></span>

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
