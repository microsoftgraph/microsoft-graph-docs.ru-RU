---
title: Тип ресурса Scopedrolemembership изменен
description: Членство в роли с областью описывает членство пользователя в роли каталога, для которого применяется административная единица (AU).  Это обеспечивает механизм, позволяющий компании, админсистратор на уровне клиента, делегировать административные привилегии пользователю для управления пользователями и группами в подмножестве Организации (подмножества, определяемого службой автоматического управления).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: abhijeetsinha
ms.openlocfilehash: 27eae463ab0f5fe0718a6d97602e366d32b11b86
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812465"
---
# <a name="scopedrolemembership-resource-type"></a><span data-ttu-id="1ae1c-104">Тип ресурса Scopedrolemembership изменен</span><span class="sxs-lookup"><span data-stu-id="1ae1c-104">scopedRoleMembership resource type</span></span>

<span data-ttu-id="1ae1c-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1ae1c-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1ae1c-106">Членство в роли с областью описывает членство пользователя в роли каталога, для которого применяется административная единица (AU).</span><span class="sxs-lookup"><span data-stu-id="1ae1c-106">A scoped-role membership describes a user's membership of a directory role, that is further scoped to an Administrative Unit (AU).</span></span>  <span data-ttu-id="1ae1c-107">Это предоставляет механизм, позволяющий администратору компании на уровне клиента делегировать административные права пользователю для управления пользователями и группами в подмножестве Организации (подмножества, определяемого службой автоматического управления).</span><span class="sxs-lookup"><span data-stu-id="1ae1c-107">This provides a mechanism to allow a tenant-wide company administrator to delegate administrative privileges to a user to manage users and groups in a subset of the organization (the subset being defined by an AU).</span></span>

## <a name="methods"></a><span data-ttu-id="1ae1c-108">Методы</span><span class="sxs-lookup"><span data-stu-id="1ae1c-108">Methods</span></span>
<span data-ttu-id="1ae1c-109">Прямые запросы к этому ресурсу не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="1ae1c-109">Direct queries to this resource are not supported.</span></span>  <span data-ttu-id="1ae1c-110">В разделе " [административные единицы](administrativeunit.md) " представлены сведения о том, как запрашивать сведения о членстве в пределах ролей, а также добавлять и удалять членство в ролях.</span><span class="sxs-lookup"><span data-stu-id="1ae1c-110">Please see the [administrative units](administrativeunit.md) topic to see information on how to query for scoped-role memberships, as well as adding and removing scoped-role memberships.</span></span>

## <a name="properties"></a><span data-ttu-id="1ae1c-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="1ae1c-111">Properties</span></span>
| <span data-ttu-id="1ae1c-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="1ae1c-112">Property</span></span>   | <span data-ttu-id="1ae1c-113">Тип</span><span class="sxs-lookup"><span data-stu-id="1ae1c-113">Type</span></span> | <span data-ttu-id="1ae1c-114">Описание</span><span class="sxs-lookup"><span data-stu-id="1ae1c-114">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="1ae1c-115">административеунитид</span><span class="sxs-lookup"><span data-stu-id="1ae1c-115">administrativeUnitId</span></span>|<span data-ttu-id="1ae1c-116">string</span><span class="sxs-lookup"><span data-stu-id="1ae1c-116">string</span></span>|<span data-ttu-id="1ae1c-117">Уникальный идентификатор административной единицы, на которую распространяется роль каталога</span><span class="sxs-lookup"><span data-stu-id="1ae1c-117">Unique identifier for the administrative unit that the directory role is scoped to</span></span>|
|<span data-ttu-id="1ae1c-118">id</span><span class="sxs-lookup"><span data-stu-id="1ae1c-118">id</span></span>|<span data-ttu-id="1ae1c-119">string</span><span class="sxs-lookup"><span data-stu-id="1ae1c-119">string</span></span>| <span data-ttu-id="1ae1c-120">Уникальный идентификатор для членства в пределах ролей.</span><span class="sxs-lookup"><span data-stu-id="1ae1c-120">Unique identifier for the scoped-role membership.</span></span> <span data-ttu-id="1ae1c-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1ae1c-121">Read-only.</span></span>|
|<span data-ttu-id="1ae1c-122">roleId</span><span class="sxs-lookup"><span data-stu-id="1ae1c-122">roleId</span></span>|<span data-ttu-id="1ae1c-123">string</span><span class="sxs-lookup"><span data-stu-id="1ae1c-123">string</span></span>| <span data-ttu-id="1ae1c-124">Уникальный идентификатор роли каталога, в которой находится член.</span><span class="sxs-lookup"><span data-stu-id="1ae1c-124">Unique identifier for the directory role that the member is in.</span></span>|
|<span data-ttu-id="1ae1c-125">roleMemberInfo</span><span class="sxs-lookup"><span data-stu-id="1ae1c-125">roleMemberInfo</span></span>|[<span data-ttu-id="1ae1c-126">identity</span><span class="sxs-lookup"><span data-stu-id="1ae1c-126">identity</span></span>](identity.md)| <span data-ttu-id="1ae1c-127">Сведения об удостоверении участника роли.</span><span class="sxs-lookup"><span data-stu-id="1ae1c-127">Role member identity information.</span></span> <span data-ttu-id="1ae1c-128">Представляет пользователя, который является членом этой области с областью действия.</span><span class="sxs-lookup"><span data-stu-id="1ae1c-128">Represents the user that is a member of this scoped-role.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1ae1c-129">Отношения</span><span class="sxs-lookup"><span data-stu-id="1ae1c-129">Relationships</span></span>
<span data-ttu-id="1ae1c-130">Нет</span><span class="sxs-lookup"><span data-stu-id="1ae1c-130">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="1ae1c-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1ae1c-131">JSON representation</span></span>

<span data-ttu-id="1ae1c-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1ae1c-132">Here is a JSON representation of the resource.</span></span>

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
