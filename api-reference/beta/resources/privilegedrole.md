---
title: Тип ресурса privilegedRole
description: 'Представляет роль администратора Azure AD, например: **глобального администратора, администратора выставления счетов, администратор службы, администратор пользователя, пароль администратора**, и т.д.'
ms.openlocfilehash: 0c04ab9de13732e4ac9eecb943a10945bec59d02
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075747"
---
# <a name="privilegedrole-resource-type"></a><span data-ttu-id="15cc0-103">Тип ресурса privilegedRole</span><span class="sxs-lookup"><span data-stu-id="15cc0-103">privilegedRole resource type</span></span>

> <span data-ttu-id="15cc0-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="15cc0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="15cc0-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15cc0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="15cc0-106">Представляет роль администратора Azure AD, например: **глобального администратора, администратора выставления счетов, администратор службы, администратор пользователя, пароль администратора**, и т.д.</span><span class="sxs-lookup"><span data-stu-id="15cc0-106">Represents an Azure AD administrator role, such as: **Global Administrator, Billing Administrator, Service Administrator, User Administrator, Password Administrator**, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="15cc0-107">Методы</span><span class="sxs-lookup"><span data-stu-id="15cc0-107">Methods</span></span>

| <span data-ttu-id="15cc0-108">Метод</span><span class="sxs-lookup"><span data-stu-id="15cc0-108">Method</span></span>           | <span data-ttu-id="15cc0-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="15cc0-109">Return Type</span></span>    |<span data-ttu-id="15cc0-110">Описание</span><span class="sxs-lookup"><span data-stu-id="15cc0-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="15cc0-111">Список объектов privilegedRole</span><span class="sxs-lookup"><span data-stu-id="15cc0-111">List privilegedRole objects</span></span>](../api/privilegedrole-list.md) | <span data-ttu-id="15cc0-112">[privilegedRole](privilegedrole.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="15cc0-112">[privilegedRole](privilegedrole.md) collection</span></span>|<span data-ttu-id="15cc0-113">Получите коллекцию privilegedRole.</span><span class="sxs-lookup"><span data-stu-id="15cc0-113">Get the collection of privilegedRole.</span></span>|
|[<span data-ttu-id="15cc0-114">Получение privilegedRole</span><span class="sxs-lookup"><span data-stu-id="15cc0-114">Get privilegedRole</span></span>](../api/privilegedrole-get.md) | [<span data-ttu-id="15cc0-115">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="15cc0-115">privilegedRole</span></span>](privilegedrole.md) |<span data-ttu-id="15cc0-116">Чтение свойства и связи объекта privilegedRole.</span><span class="sxs-lookup"><span data-stu-id="15cc0-116">Read properties and relationships of privilegedRole object.</span></span>|
|[<span data-ttu-id="15cc0-117">Список назначений</span><span class="sxs-lookup"><span data-stu-id="15cc0-117">List assignments</span></span>](../api/privilegedrole-list-assignments.md) |<span data-ttu-id="15cc0-118">[privilegedRoleAssignment](privilegedroleassignment.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="15cc0-118">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>| <span data-ttu-id="15cc0-119">Получите коллекцию объектов назначения для этой роли.</span><span class="sxs-lookup"><span data-stu-id="15cc0-119">Get a assignment object collection for this role.</span></span>|
|[<span data-ttu-id="15cc0-120">selfActivate</span><span class="sxs-lookup"><span data-stu-id="15cc0-120">selfActivate</span></span>](../api/privilegedrole-selfactivate.md)|[<span data-ttu-id="15cc0-121">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="15cc0-121">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="15cc0-122">Активация назначенной роли.</span><span class="sxs-lookup"><span data-stu-id="15cc0-122">Activate the assigned role.</span></span>|
|[<span data-ttu-id="15cc0-123">selfDeactivate</span><span class="sxs-lookup"><span data-stu-id="15cc0-123">selfDeactivate</span></span>](../api/privilegedrole-selfdeactivate.md)|[<span data-ttu-id="15cc0-124">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="15cc0-124">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="15cc0-125">Деактивируйте, назначенной роли.</span><span class="sxs-lookup"><span data-stu-id="15cc0-125">Deactivate the assigned role.</span></span>|

## <a name="properties"></a><span data-ttu-id="15cc0-126">Свойства</span><span class="sxs-lookup"><span data-stu-id="15cc0-126">Properties</span></span>
| <span data-ttu-id="15cc0-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="15cc0-127">Property</span></span>     | <span data-ttu-id="15cc0-128">Тип</span><span class="sxs-lookup"><span data-stu-id="15cc0-128">Type</span></span>   |<span data-ttu-id="15cc0-129">Описание</span><span class="sxs-lookup"><span data-stu-id="15cc0-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="15cc0-130">id</span><span class="sxs-lookup"><span data-stu-id="15cc0-130">id</span></span>|<span data-ttu-id="15cc0-131">строка</span><span class="sxs-lookup"><span data-stu-id="15cc0-131">string</span></span>|<span data-ttu-id="15cc0-132">Уникальный идентификатор для роли администратора.</span><span class="sxs-lookup"><span data-stu-id="15cc0-132">The unique identifier for administrator role.</span></span> <span data-ttu-id="15cc0-133">Он является строкой GUID, совпадает со значением идентификатора шаблона роли из Azure AD для данной роли.</span><span class="sxs-lookup"><span data-stu-id="15cc0-133">It is a GUID string and has the same value as the role template id from Azure AD for the given role.</span></span> <span data-ttu-id="15cc0-134">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="15cc0-134">Read-only.</span></span>|
|<span data-ttu-id="15cc0-135">name</span><span class="sxs-lookup"><span data-stu-id="15cc0-135">name</span></span>|<span data-ttu-id="15cc0-136">строка</span><span class="sxs-lookup"><span data-stu-id="15cc0-136">string</span></span>|<span data-ttu-id="15cc0-137">Имя роли.</span><span class="sxs-lookup"><span data-stu-id="15cc0-137">Role name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="15cc0-138">Связи</span><span class="sxs-lookup"><span data-stu-id="15cc0-138">Relationships</span></span>
| <span data-ttu-id="15cc0-139">Связь</span><span class="sxs-lookup"><span data-stu-id="15cc0-139">Relationship</span></span> | <span data-ttu-id="15cc0-140">Тип</span><span class="sxs-lookup"><span data-stu-id="15cc0-140">Type</span></span>   |<span data-ttu-id="15cc0-141">Описание</span><span class="sxs-lookup"><span data-stu-id="15cc0-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="15cc0-142">assignments</span><span class="sxs-lookup"><span data-stu-id="15cc0-142">assignments</span></span>|<span data-ttu-id="15cc0-143">[privilegedRoleAssignment](privilegedroleassignment.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="15cc0-143">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>| <span data-ttu-id="15cc0-144">Назначения для этой роли.</span><span class="sxs-lookup"><span data-stu-id="15cc0-144">The assignments for this role.</span></span> <span data-ttu-id="15cc0-145">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="15cc0-145">Read-only.</span></span> <span data-ttu-id="15cc0-146">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="15cc0-146">Nullable.</span></span>|
|<span data-ttu-id="15cc0-147">settings</span><span class="sxs-lookup"><span data-stu-id="15cc0-147">settings</span></span>|[<span data-ttu-id="15cc0-148">privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="15cc0-148">privilegedRoleSettings</span></span>](privilegedrolesettings.md)| <span data-ttu-id="15cc0-149">Параметры для этой роли.</span><span class="sxs-lookup"><span data-stu-id="15cc0-149">The settings for this role.</span></span> <span data-ttu-id="15cc0-150">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="15cc0-150">Read-only.</span></span> <span data-ttu-id="15cc0-151">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="15cc0-151">Nullable.</span></span>|
|<span data-ttu-id="15cc0-152">Сводка</span><span class="sxs-lookup"><span data-stu-id="15cc0-152">summary</span></span>|[<span data-ttu-id="15cc0-153">privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="15cc0-153">privilegedRoleSummary</span></span>](privilegedrolesummary.md)| <span data-ttu-id="15cc0-154">Сводные данные для этой роли.</span><span class="sxs-lookup"><span data-stu-id="15cc0-154">The summary information for this role.</span></span> <span data-ttu-id="15cc0-155">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="15cc0-155">Read-only.</span></span> <span data-ttu-id="15cc0-156">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="15cc0-156">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="15cc0-157">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="15cc0-157">JSON representation</span></span>

<span data-ttu-id="15cc0-158">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="15cc0-158">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "privilegedRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->