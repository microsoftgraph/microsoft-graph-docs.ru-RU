---
title: Тип ресурса scopedRoleMembership
description: Членство с ролью с областью действия описывает членство пользователя в роли каталога, которая дополнительно имеет область действия административной единицы (AU).  Это предоставляет механизм, позволяющий администратору компании на клиенте делегировать права администратора пользователю для управления пользователями и группами в подмножестве организаций (подмножество определяется au).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: directory-management
author: abhijeetsinha
ms.openlocfilehash: ffd1e616d94ccf959b8535f46f79a2c7c57e00c2
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134710"
---
# <a name="scopedrolemembership-resource-type"></a><span data-ttu-id="c69fb-104">Тип ресурса scopedRoleMembership</span><span class="sxs-lookup"><span data-stu-id="c69fb-104">scopedRoleMembership resource type</span></span>

<span data-ttu-id="c69fb-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c69fb-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c69fb-106">Членство с ролью с областью действия описывает членство пользователя в роли каталога, которая дополнительно имеет область действия административной единицы (AU).</span><span class="sxs-lookup"><span data-stu-id="c69fb-106">A scoped-role membership describes a user's membership of a directory role, that is further scoped to an Administrative Unit (AU).</span></span>  <span data-ttu-id="c69fb-107">Это предоставляет механизм, позволяющий администратору компании на клиенте делегировать права администратора пользователю для управления пользователями и группами в подмножество организации (подмножество, определяемого au).</span><span class="sxs-lookup"><span data-stu-id="c69fb-107">This provides a mechanism to allow a tenant-wide company administrator to delegate administrative privileges to a user to manage users and groups in a subset of the organization (the subset being defined by an AU).</span></span>

## <a name="methods"></a><span data-ttu-id="c69fb-108">Методы</span><span class="sxs-lookup"><span data-stu-id="c69fb-108">Methods</span></span>
<span data-ttu-id="c69fb-109">Прямые запросы к этому ресурсу не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="c69fb-109">Direct queries to this resource are not supported.</span></span>  <span data-ttu-id="c69fb-110">См. [раздел](administrativeunit.md) об административных единицах, чтобы узнать, как запрашивать участие в роли с заданной областью, а также добавлять и удалять членство с ролью с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="c69fb-110">Please see the [administrative units](administrativeunit.md) topic to see information on how to query for scoped-role memberships, as well as adding and removing scoped-role memberships.</span></span>

## <a name="properties"></a><span data-ttu-id="c69fb-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="c69fb-111">Properties</span></span>
| <span data-ttu-id="c69fb-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="c69fb-112">Property</span></span>   | <span data-ttu-id="c69fb-113">Тип</span><span class="sxs-lookup"><span data-stu-id="c69fb-113">Type</span></span> | <span data-ttu-id="c69fb-114">Описание</span><span class="sxs-lookup"><span data-stu-id="c69fb-114">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="c69fb-115">administrativeUnitId</span><span class="sxs-lookup"><span data-stu-id="c69fb-115">administrativeUnitId</span></span>|<span data-ttu-id="c69fb-116">string</span><span class="sxs-lookup"><span data-stu-id="c69fb-116">string</span></span>|<span data-ttu-id="c69fb-117">Уникальный идентификатор административной единицы, областью действия роли каталога</span><span class="sxs-lookup"><span data-stu-id="c69fb-117">Unique identifier for the administrative unit that the directory role is scoped to</span></span>|
|<span data-ttu-id="c69fb-118">id</span><span class="sxs-lookup"><span data-stu-id="c69fb-118">id</span></span>|<span data-ttu-id="c69fb-119">string</span><span class="sxs-lookup"><span data-stu-id="c69fb-119">string</span></span>| <span data-ttu-id="c69fb-120">Уникальный идентификатор членства с ролью с за областью действия.</span><span class="sxs-lookup"><span data-stu-id="c69fb-120">Unique identifier for the scoped-role membership.</span></span> <span data-ttu-id="c69fb-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c69fb-121">Read-only.</span></span>|
|<span data-ttu-id="c69fb-122">roleId</span><span class="sxs-lookup"><span data-stu-id="c69fb-122">roleId</span></span>|<span data-ttu-id="c69fb-123">string</span><span class="sxs-lookup"><span data-stu-id="c69fb-123">string</span></span>| <span data-ttu-id="c69fb-124">Уникальный идентификатор роли каталога, в котором находится участник.</span><span class="sxs-lookup"><span data-stu-id="c69fb-124">Unique identifier for the directory role that the member is in.</span></span>|
|<span data-ttu-id="c69fb-125">roleMemberInfo</span><span class="sxs-lookup"><span data-stu-id="c69fb-125">roleMemberInfo</span></span>|[<span data-ttu-id="c69fb-126">identity</span><span class="sxs-lookup"><span data-stu-id="c69fb-126">identity</span></span>](identity.md)| <span data-ttu-id="c69fb-127">Сведения об удостоверении участника роли.</span><span class="sxs-lookup"><span data-stu-id="c69fb-127">Role member identity information.</span></span> <span data-ttu-id="c69fb-128">Представляет пользователя, который является членом этой роли с заданной областью действия.</span><span class="sxs-lookup"><span data-stu-id="c69fb-128">Represents the user that is a member of this scoped-role.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c69fb-129">Связи</span><span class="sxs-lookup"><span data-stu-id="c69fb-129">Relationships</span></span>
<span data-ttu-id="c69fb-130">Нет</span><span class="sxs-lookup"><span data-stu-id="c69fb-130">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="c69fb-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c69fb-131">JSON representation</span></span>

<span data-ttu-id="c69fb-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c69fb-132">Here is a JSON representation of the resource.</span></span>

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


