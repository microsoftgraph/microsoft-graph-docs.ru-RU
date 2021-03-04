---
title: тип ресурса privilegedRole
description: 'Представляет роль администратора Azure AD, например: глобального администратора, администратора биллинга, администратора службы, администратора **пользователей, администратора паролей** и т. д.'
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 4eca2f1a3d9de4fa7f625cd6b559b5a0c9c03916
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444016"
---
# <a name="privilegedrole-resource-type"></a><span data-ttu-id="3e254-103">тип ресурса privilegedRole</span><span class="sxs-lookup"><span data-stu-id="3e254-103">privilegedRole resource type</span></span>

<span data-ttu-id="3e254-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3e254-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3e254-105">Представляет роль администратора Azure AD, например: глобального администратора, администратора биллинга, администратора службы, администратора **пользователей, администратора паролей** и т. д.</span><span class="sxs-lookup"><span data-stu-id="3e254-105">Represents an Azure AD administrator role, such as: **Global Administrator, Billing Administrator, Service Administrator, User Administrator, Password Administrator**, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="3e254-106">Методы</span><span class="sxs-lookup"><span data-stu-id="3e254-106">Methods</span></span>

| <span data-ttu-id="3e254-107">Метод</span><span class="sxs-lookup"><span data-stu-id="3e254-107">Method</span></span>           | <span data-ttu-id="3e254-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="3e254-108">Return Type</span></span>    |<span data-ttu-id="3e254-109">Описание</span><span class="sxs-lookup"><span data-stu-id="3e254-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3e254-110">Список объектов privilegedRole</span><span class="sxs-lookup"><span data-stu-id="3e254-110">List privilegedRole objects</span></span>](../api/privilegedrole-list.md) | <span data-ttu-id="3e254-111">Коллекция [privilegedRole](privilegedrole.md)</span><span class="sxs-lookup"><span data-stu-id="3e254-111">[privilegedRole](privilegedrole.md) collection</span></span>|<span data-ttu-id="3e254-112">Получите коллекцию privilegedRole.</span><span class="sxs-lookup"><span data-stu-id="3e254-112">Get the collection of privilegedRole.</span></span>|
|[<span data-ttu-id="3e254-113">Получение privilegedRole</span><span class="sxs-lookup"><span data-stu-id="3e254-113">Get privilegedRole</span></span>](../api/privilegedrole-get.md) | [<span data-ttu-id="3e254-114">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="3e254-114">privilegedRole</span></span>](privilegedrole.md) |<span data-ttu-id="3e254-115">Чтение свойств и связей объекта privilegedRole.</span><span class="sxs-lookup"><span data-stu-id="3e254-115">Read properties and relationships of privilegedRole object.</span></span>|
|[<span data-ttu-id="3e254-116">Перечисление заданий</span><span class="sxs-lookup"><span data-stu-id="3e254-116">List assignments</span></span>](../api/privilegedrole-list-assignments.md) |<span data-ttu-id="3e254-117">Коллекция [privilegedRoleAssignment](privilegedroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="3e254-117">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>| <span data-ttu-id="3e254-118">Получите коллекцию объектов назначения для этой роли.</span><span class="sxs-lookup"><span data-stu-id="3e254-118">Get a assignment object collection for this role.</span></span>|
|[<span data-ttu-id="3e254-119">selfActivate</span><span class="sxs-lookup"><span data-stu-id="3e254-119">selfActivate</span></span>](../api/privilegedrole-selfactivate.md)|[<span data-ttu-id="3e254-120">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="3e254-120">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="3e254-121">Активируйте назначенную роль.</span><span class="sxs-lookup"><span data-stu-id="3e254-121">Activate the assigned role.</span></span>|
|[<span data-ttu-id="3e254-122">selfDeactivate</span><span class="sxs-lookup"><span data-stu-id="3e254-122">selfDeactivate</span></span>](../api/privilegedrole-selfdeactivate.md)|[<span data-ttu-id="3e254-123">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="3e254-123">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="3e254-124">Деактивировать назначенную роль.</span><span class="sxs-lookup"><span data-stu-id="3e254-124">Deactivate the assigned role.</span></span>|

## <a name="properties"></a><span data-ttu-id="3e254-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="3e254-125">Properties</span></span>
| <span data-ttu-id="3e254-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="3e254-126">Property</span></span>     | <span data-ttu-id="3e254-127">Тип</span><span class="sxs-lookup"><span data-stu-id="3e254-127">Type</span></span>   |<span data-ttu-id="3e254-128">Описание</span><span class="sxs-lookup"><span data-stu-id="3e254-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3e254-129">id</span><span class="sxs-lookup"><span data-stu-id="3e254-129">id</span></span>|<span data-ttu-id="3e254-130">string</span><span class="sxs-lookup"><span data-stu-id="3e254-130">string</span></span>|<span data-ttu-id="3e254-131">Уникальный идентификатор роли администратора.</span><span class="sxs-lookup"><span data-stu-id="3e254-131">The unique identifier for administrator role.</span></span> <span data-ttu-id="3e254-132">Это строка GUID и имеет то же значение, что и id шаблона ролей из Azure AD для данной роли.</span><span class="sxs-lookup"><span data-stu-id="3e254-132">It is a GUID string and has the same value as the role template id from Azure AD for the given role.</span></span> <span data-ttu-id="3e254-133">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3e254-133">Read-only.</span></span>|
|<span data-ttu-id="3e254-134">name</span><span class="sxs-lookup"><span data-stu-id="3e254-134">name</span></span>|<span data-ttu-id="3e254-135">string</span><span class="sxs-lookup"><span data-stu-id="3e254-135">string</span></span>|<span data-ttu-id="3e254-136">Имя роли.</span><span class="sxs-lookup"><span data-stu-id="3e254-136">Role name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3e254-137">Связи</span><span class="sxs-lookup"><span data-stu-id="3e254-137">Relationships</span></span>
| <span data-ttu-id="3e254-138">Связь</span><span class="sxs-lookup"><span data-stu-id="3e254-138">Relationship</span></span> | <span data-ttu-id="3e254-139">Тип</span><span class="sxs-lookup"><span data-stu-id="3e254-139">Type</span></span>   |<span data-ttu-id="3e254-140">Описание</span><span class="sxs-lookup"><span data-stu-id="3e254-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3e254-141">assignments</span><span class="sxs-lookup"><span data-stu-id="3e254-141">assignments</span></span>|<span data-ttu-id="3e254-142">Коллекция [privilegedRoleAssignment](privilegedroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="3e254-142">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>| <span data-ttu-id="3e254-143">Назначения для этой роли.</span><span class="sxs-lookup"><span data-stu-id="3e254-143">The assignments for this role.</span></span> <span data-ttu-id="3e254-144">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3e254-144">Read-only.</span></span> <span data-ttu-id="3e254-145">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="3e254-145">Nullable.</span></span>|
|<span data-ttu-id="3e254-146">параметры</span><span class="sxs-lookup"><span data-stu-id="3e254-146">settings</span></span>|[<span data-ttu-id="3e254-147">privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="3e254-147">privilegedRoleSettings</span></span>](privilegedrolesettings.md)| <span data-ttu-id="3e254-148">Параметры для этой роли.</span><span class="sxs-lookup"><span data-stu-id="3e254-148">The settings for this role.</span></span> <span data-ttu-id="3e254-149">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3e254-149">Read-only.</span></span> <span data-ttu-id="3e254-150">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="3e254-150">Nullable.</span></span>|
|<span data-ttu-id="3e254-151">summary</span><span class="sxs-lookup"><span data-stu-id="3e254-151">summary</span></span>|[<span data-ttu-id="3e254-152">privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="3e254-152">privilegedRoleSummary</span></span>](privilegedrolesummary.md)| <span data-ttu-id="3e254-153">Сводная информация для этой роли.</span><span class="sxs-lookup"><span data-stu-id="3e254-153">The summary information for this role.</span></span> <span data-ttu-id="3e254-154">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3e254-154">Read-only.</span></span> <span data-ttu-id="3e254-155">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="3e254-155">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3e254-156">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3e254-156">JSON representation</span></span>

<span data-ttu-id="3e254-157">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3e254-157">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
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
  "suppressions": []
}
-->


