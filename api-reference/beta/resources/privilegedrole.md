---
title: Тип ресурса privilegedRole
description: 'Представляет роль администратора Azure AD, например: **глобального администратора, администратора выставления счетов, администратор службы, администратор пользователя, пароль администратора**, и т.д.'
localization_priority: Normal
ms.openlocfilehash: 131999f52a583400b018e98d2319118f69ca87e8
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513748"
---
# <a name="privilegedrole-resource-type"></a><span data-ttu-id="55844-103">Тип ресурса privilegedRole</span><span class="sxs-lookup"><span data-stu-id="55844-103">privilegedRole resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="55844-104">Представляет роль администратора Azure AD, например: **глобального администратора, администратора выставления счетов, администратор службы, администратор пользователя, пароль администратора**, и т.д.</span><span class="sxs-lookup"><span data-stu-id="55844-104">Represents an Azure AD administrator role, such as: **Global Administrator, Billing Administrator, Service Administrator, User Administrator, Password Administrator**, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="55844-105">Методы</span><span class="sxs-lookup"><span data-stu-id="55844-105">Methods</span></span>

| <span data-ttu-id="55844-106">Метод</span><span class="sxs-lookup"><span data-stu-id="55844-106">Method</span></span>           | <span data-ttu-id="55844-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="55844-107">Return Type</span></span>    |<span data-ttu-id="55844-108">Описание</span><span class="sxs-lookup"><span data-stu-id="55844-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="55844-109">Список объектов privilegedRole</span><span class="sxs-lookup"><span data-stu-id="55844-109">List privilegedRole objects</span></span>](../api/privilegedrole-list.md) | <span data-ttu-id="55844-110">[privilegedRole](privilegedrole.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="55844-110">[privilegedRole](privilegedrole.md) collection</span></span>|<span data-ttu-id="55844-111">Получите коллекцию privilegedRole.</span><span class="sxs-lookup"><span data-stu-id="55844-111">Get the collection of privilegedRole.</span></span>|
|[<span data-ttu-id="55844-112">Получение privilegedRole</span><span class="sxs-lookup"><span data-stu-id="55844-112">Get privilegedRole</span></span>](../api/privilegedrole-get.md) | [<span data-ttu-id="55844-113">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="55844-113">privilegedRole</span></span>](privilegedrole.md) |<span data-ttu-id="55844-114">Чтение свойства и связи объекта privilegedRole.</span><span class="sxs-lookup"><span data-stu-id="55844-114">Read properties and relationships of privilegedRole object.</span></span>|
|[<span data-ttu-id="55844-115">Список назначений</span><span class="sxs-lookup"><span data-stu-id="55844-115">List assignments</span></span>](../api/privilegedrole-list-assignments.md) |<span data-ttu-id="55844-116">[privilegedRoleAssignment](privilegedroleassignment.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="55844-116">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>| <span data-ttu-id="55844-117">Получите коллекцию объектов назначения для этой роли.</span><span class="sxs-lookup"><span data-stu-id="55844-117">Get a assignment object collection for this role.</span></span>|
|[<span data-ttu-id="55844-118">selfActivate</span><span class="sxs-lookup"><span data-stu-id="55844-118">selfActivate</span></span>](../api/privilegedrole-selfactivate.md)|[<span data-ttu-id="55844-119">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="55844-119">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="55844-120">Активация назначенной роли.</span><span class="sxs-lookup"><span data-stu-id="55844-120">Activate the assigned role.</span></span>|
|[<span data-ttu-id="55844-121">selfDeactivate</span><span class="sxs-lookup"><span data-stu-id="55844-121">selfDeactivate</span></span>](../api/privilegedrole-selfdeactivate.md)|[<span data-ttu-id="55844-122">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="55844-122">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="55844-123">Деактивируйте, назначенной роли.</span><span class="sxs-lookup"><span data-stu-id="55844-123">Deactivate the assigned role.</span></span>|

## <a name="properties"></a><span data-ttu-id="55844-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="55844-124">Properties</span></span>
| <span data-ttu-id="55844-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="55844-125">Property</span></span>     | <span data-ttu-id="55844-126">Тип</span><span class="sxs-lookup"><span data-stu-id="55844-126">Type</span></span>   |<span data-ttu-id="55844-127">Описание</span><span class="sxs-lookup"><span data-stu-id="55844-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="55844-128">id</span><span class="sxs-lookup"><span data-stu-id="55844-128">id</span></span>|<span data-ttu-id="55844-129">string</span><span class="sxs-lookup"><span data-stu-id="55844-129">string</span></span>|<span data-ttu-id="55844-130">Уникальный идентификатор для роли администратора.</span><span class="sxs-lookup"><span data-stu-id="55844-130">The unique identifier for administrator role.</span></span> <span data-ttu-id="55844-131">Он является строкой GUID, совпадает со значением идентификатора шаблона роли из Azure AD для данной роли.</span><span class="sxs-lookup"><span data-stu-id="55844-131">It is a GUID string and has the same value as the role template id from Azure AD for the given role.</span></span> <span data-ttu-id="55844-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="55844-132">Read-only.</span></span>|
|<span data-ttu-id="55844-133">name</span><span class="sxs-lookup"><span data-stu-id="55844-133">name</span></span>|<span data-ttu-id="55844-134">строка</span><span class="sxs-lookup"><span data-stu-id="55844-134">string</span></span>|<span data-ttu-id="55844-135">Имя роли.</span><span class="sxs-lookup"><span data-stu-id="55844-135">Role name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="55844-136">Отношения</span><span class="sxs-lookup"><span data-stu-id="55844-136">Relationships</span></span>
| <span data-ttu-id="55844-137">Связь</span><span class="sxs-lookup"><span data-stu-id="55844-137">Relationship</span></span> | <span data-ttu-id="55844-138">Тип</span><span class="sxs-lookup"><span data-stu-id="55844-138">Type</span></span>   |<span data-ttu-id="55844-139">Описание</span><span class="sxs-lookup"><span data-stu-id="55844-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="55844-140">assignments</span><span class="sxs-lookup"><span data-stu-id="55844-140">assignments</span></span>|<span data-ttu-id="55844-141">[privilegedRoleAssignment](privilegedroleassignment.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="55844-141">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>| <span data-ttu-id="55844-142">Назначения для этой роли.</span><span class="sxs-lookup"><span data-stu-id="55844-142">The assignments for this role.</span></span> <span data-ttu-id="55844-143">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="55844-143">Read-only.</span></span> <span data-ttu-id="55844-144">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="55844-144">Nullable.</span></span>|
|<span data-ttu-id="55844-145">settings</span><span class="sxs-lookup"><span data-stu-id="55844-145">settings</span></span>|[<span data-ttu-id="55844-146">privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="55844-146">privilegedRoleSettings</span></span>](privilegedrolesettings.md)| <span data-ttu-id="55844-147">Параметры для этой роли.</span><span class="sxs-lookup"><span data-stu-id="55844-147">The settings for this role.</span></span> <span data-ttu-id="55844-148">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="55844-148">Read-only.</span></span> <span data-ttu-id="55844-149">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="55844-149">Nullable.</span></span>|
|<span data-ttu-id="55844-150">Summary</span><span class="sxs-lookup"><span data-stu-id="55844-150">summary</span></span>|[<span data-ttu-id="55844-151">privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="55844-151">privilegedRoleSummary</span></span>](privilegedrolesummary.md)| <span data-ttu-id="55844-152">Сводные данные для этой роли.</span><span class="sxs-lookup"><span data-stu-id="55844-152">The summary information for this role.</span></span> <span data-ttu-id="55844-153">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="55844-153">Read-only.</span></span> <span data-ttu-id="55844-154">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="55844-154">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="55844-155">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="55844-155">JSON representation</span></span>

<span data-ttu-id="55844-156">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="55844-156">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.privilegedRole"
}-->

```json
{
  "id": "string (identifier)",
  "name": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/privilegedrole.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
