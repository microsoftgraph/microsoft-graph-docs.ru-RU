---
title: Тип ресурса scopedRoleMembership
description: Членство в пределах роли описывает принадлежности пользователя к роли каталога, с дальнейшей областью действия, чтобы административные единицы (AU).  Это обеспечивает механизм, позволяющий adminsistrator клиента всей компании делегировать административные полномочия для пользователя для управления пользователями и группами в подмножества организации (подмножество, определяемым AU).
ms.openlocfilehash: bd635a5b1b06b98657ba24c397e2f67afb76fa8f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078130"
---
# <a name="scopedrolemembership-resource-type"></a><span data-ttu-id="c4123-104">Тип ресурса scopedRoleMembership</span><span class="sxs-lookup"><span data-stu-id="c4123-104">scopedRoleMembership resource type</span></span>

> <span data-ttu-id="c4123-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c4123-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c4123-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4123-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c4123-107">Членство в пределах роли описывает принадлежности пользователя к роли каталога, с дальнейшей областью действия, чтобы административные единицы (AU).</span><span class="sxs-lookup"><span data-stu-id="c4123-107">A scoped-role membership describes a user's membership of a directory role, that is further scoped to an Administrative Unit (AU).</span></span>  <span data-ttu-id="c4123-108">Это обеспечивает механизм, позволяющий adminsistrator клиента всей компании делегировать административные полномочия для пользователя для управления пользователями и группами в подмножества организации (подмножество, определяемым AU).</span><span class="sxs-lookup"><span data-stu-id="c4123-108">This provides a mechanism to allow a tenant-wide company adminsistrator to delegate administrative privileges to a user to manage users and groups in a subset of the organization (the subset being defined by an AU).</span></span>

## <a name="methods"></a><span data-ttu-id="c4123-109">Methods</span><span class="sxs-lookup"><span data-stu-id="c4123-109">Methods</span></span>
<span data-ttu-id="c4123-110">Прямые запросы для этого ресурса не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="c4123-110">Direct queries to this resource are not supported.</span></span>  <span data-ttu-id="c4123-111">Ознакомьтесь с [единицы администрирования](administrativeunit.md) раздел для просмотра сведений о том, как для запроса областью действия роли участие в группах, а также добавление и удаление членство областью действия роли.</span><span class="sxs-lookup"><span data-stu-id="c4123-111">Please see the [adminstrative units](administrativeunit.md) topic to see information on how to query for scoped-role memberships, as well as adding and removing scoped-role memberships.</span></span> 

## <a name="properties"></a><span data-ttu-id="c4123-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="c4123-112">Properties</span></span>
| <span data-ttu-id="c4123-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="c4123-113">Property</span></span>   | <span data-ttu-id="c4123-114">Тип</span><span class="sxs-lookup"><span data-stu-id="c4123-114">Type</span></span> | <span data-ttu-id="c4123-115">Description</span><span class="sxs-lookup"><span data-stu-id="c4123-115">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="c4123-116">administrativeUnitId</span><span class="sxs-lookup"><span data-stu-id="c4123-116">administrativeUnitId</span></span>|<span data-ttu-id="c4123-117">string</span><span class="sxs-lookup"><span data-stu-id="c4123-117">string</span></span>|<span data-ttu-id="c4123-118">Уникальный идентификатор административного подразделения, пределах роли каталога</span><span class="sxs-lookup"><span data-stu-id="c4123-118">Unique identifier for the administrative unit that the directory role is scoped to</span></span>|
|<span data-ttu-id="c4123-119">id</span><span class="sxs-lookup"><span data-stu-id="c4123-119">id</span></span>|<span data-ttu-id="c4123-120">строка</span><span class="sxs-lookup"><span data-stu-id="c4123-120">string</span></span>| <span data-ttu-id="c4123-121">Уникальный идентификатор для членство в области определения роли.</span><span class="sxs-lookup"><span data-stu-id="c4123-121">Unique identifier for the scoped-role membership.</span></span> <span data-ttu-id="c4123-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c4123-122">Read-only.</span></span>|
|<span data-ttu-id="c4123-123">roleId</span><span class="sxs-lookup"><span data-stu-id="c4123-123">roleId</span></span>|<span data-ttu-id="c4123-124">string</span><span class="sxs-lookup"><span data-stu-id="c4123-124">string</span></span>| <span data-ttu-id="c4123-125">Уникальный идентификатор для роли каталога, элемент.</span><span class="sxs-lookup"><span data-stu-id="c4123-125">Unique identifier for the directory role that the member is in.</span></span>|
|<span data-ttu-id="c4123-126">roleMemberInfo</span><span class="sxs-lookup"><span data-stu-id="c4123-126">roleMemberInfo</span></span>|[<span data-ttu-id="c4123-127">identity</span><span class="sxs-lookup"><span data-stu-id="c4123-127">identity</span></span>](identity.md)| <span data-ttu-id="c4123-128">Сведения о удостоверение члена роли.</span><span class="sxs-lookup"><span data-stu-id="c4123-128">Role member identity information.</span></span> <span data-ttu-id="c4123-129">Представляет пользователя, который является членом этой области определения роли.</span><span class="sxs-lookup"><span data-stu-id="c4123-129">Represents the user that is a member of this scoped-role.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c4123-130">Связи</span><span class="sxs-lookup"><span data-stu-id="c4123-130">Relationships</span></span>
<span data-ttu-id="c4123-131">Нет</span><span class="sxs-lookup"><span data-stu-id="c4123-131">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="c4123-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c4123-132">JSON representation</span></span>

<span data-ttu-id="c4123-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c4123-133">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.scopedrolemembership"
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
<!-- {
  "type": "#page.annotation",
  "description": "scopedRoleMembership resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->