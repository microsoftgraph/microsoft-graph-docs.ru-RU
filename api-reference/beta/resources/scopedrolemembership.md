---
title: Тип ресурса scopedRoleMembership
description: Членство в пределах роли описывает принадлежности пользователя к роли каталога, с дальнейшей областью действия, чтобы административные единицы (AU).  Это обеспечивает механизм, позволяющий adminsistrator клиента всей компании делегировать административные полномочия для пользователя для управления пользователями и группами в подмножества организации (подмножество, определяемым AU).
localization_priority: Normal
ms.openlocfilehash: 2d51ad696487e7daafb9b0f4fcef0934e4f6d6e2
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521504"
---
# <a name="scopedrolemembership-resource-type"></a><span data-ttu-id="bb4a5-104">Тип ресурса scopedRoleMembership</span><span class="sxs-lookup"><span data-stu-id="bb4a5-104">scopedRoleMembership resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bb4a5-105">Членство в пределах роли описывает принадлежности пользователя к роли каталога, с дальнейшей областью действия, чтобы административные единицы (AU).</span><span class="sxs-lookup"><span data-stu-id="bb4a5-105">A scoped-role membership describes a user's membership of a directory role, that is further scoped to an Administrative Unit (AU).</span></span>  <span data-ttu-id="bb4a5-106">Это обеспечивает механизм, позволяющий adminsistrator клиента всей компании делегировать административные полномочия для пользователя для управления пользователями и группами в подмножества организации (подмножество, определяемым AU).</span><span class="sxs-lookup"><span data-stu-id="bb4a5-106">This provides a mechanism to allow a tenant-wide company adminsistrator to delegate administrative privileges to a user to manage users and groups in a subset of the organization (the subset being defined by an AU).</span></span>

## <a name="methods"></a><span data-ttu-id="bb4a5-107">Методы</span><span class="sxs-lookup"><span data-stu-id="bb4a5-107">Methods</span></span>
<span data-ttu-id="bb4a5-108">Прямые запросы для этого ресурса не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="bb4a5-108">Direct queries to this resource are not supported.</span></span>  <span data-ttu-id="bb4a5-109">Ознакомьтесь с [единицы администрирования](administrativeunit.md) раздел для просмотра сведений о том, как для запроса областью действия роли участие в группах, а также добавление и удаление членство областью действия роли.</span><span class="sxs-lookup"><span data-stu-id="bb4a5-109">Please see the [adminstrative units](administrativeunit.md) topic to see information on how to query for scoped-role memberships, as well as adding and removing scoped-role memberships.</span></span> 

## <a name="properties"></a><span data-ttu-id="bb4a5-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="bb4a5-110">Properties</span></span>
| <span data-ttu-id="bb4a5-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="bb4a5-111">Property</span></span>   | <span data-ttu-id="bb4a5-112">Тип</span><span class="sxs-lookup"><span data-stu-id="bb4a5-112">Type</span></span> | <span data-ttu-id="bb4a5-113">Описание</span><span class="sxs-lookup"><span data-stu-id="bb4a5-113">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="bb4a5-114">administrativeUnitId</span><span class="sxs-lookup"><span data-stu-id="bb4a5-114">administrativeUnitId</span></span>|<span data-ttu-id="bb4a5-115">string</span><span class="sxs-lookup"><span data-stu-id="bb4a5-115">string</span></span>|<span data-ttu-id="bb4a5-116">Уникальный идентификатор административного подразделения, пределах роли каталога</span><span class="sxs-lookup"><span data-stu-id="bb4a5-116">Unique identifier for the administrative unit that the directory role is scoped to</span></span>|
|<span data-ttu-id="bb4a5-117">id</span><span class="sxs-lookup"><span data-stu-id="bb4a5-117">id</span></span>|<span data-ttu-id="bb4a5-118">string</span><span class="sxs-lookup"><span data-stu-id="bb4a5-118">string</span></span>| <span data-ttu-id="bb4a5-119">Уникальный идентификатор для членство в области определения роли.</span><span class="sxs-lookup"><span data-stu-id="bb4a5-119">Unique identifier for the scoped-role membership.</span></span> <span data-ttu-id="bb4a5-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bb4a5-120">Read-only.</span></span>|
|<span data-ttu-id="bb4a5-121">roleId</span><span class="sxs-lookup"><span data-stu-id="bb4a5-121">roleId</span></span>|<span data-ttu-id="bb4a5-122">string</span><span class="sxs-lookup"><span data-stu-id="bb4a5-122">string</span></span>| <span data-ttu-id="bb4a5-123">Уникальный идентификатор для роли каталога, элемент.</span><span class="sxs-lookup"><span data-stu-id="bb4a5-123">Unique identifier for the directory role that the member is in.</span></span>|
|<span data-ttu-id="bb4a5-124">roleMemberInfo</span><span class="sxs-lookup"><span data-stu-id="bb4a5-124">roleMemberInfo</span></span>|[<span data-ttu-id="bb4a5-125">identity</span><span class="sxs-lookup"><span data-stu-id="bb4a5-125">identity</span></span>](identity.md)| <span data-ttu-id="bb4a5-126">Сведения о удостоверение члена роли.</span><span class="sxs-lookup"><span data-stu-id="bb4a5-126">Role member identity information.</span></span> <span data-ttu-id="bb4a5-127">Представляет пользователя, который является членом этой области определения роли.</span><span class="sxs-lookup"><span data-stu-id="bb4a5-127">Represents the user that is a member of this scoped-role.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bb4a5-128">Отношения</span><span class="sxs-lookup"><span data-stu-id="bb4a5-128">Relationships</span></span>
<span data-ttu-id="bb4a5-129">Нет</span><span class="sxs-lookup"><span data-stu-id="bb4a5-129">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="bb4a5-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bb4a5-130">JSON representation</span></span>

<span data-ttu-id="bb4a5-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bb4a5-131">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "scopedRoleMembership resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/scopedrolemembership.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
