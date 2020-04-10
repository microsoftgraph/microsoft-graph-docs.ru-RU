---
title: Тип ресурса Привилежедроле
description: 'Представляет роль администратора Azure AD, например: **глобальному администратору, администратору выставления счетов, администратору служб, администратору пользователей, администратору паролей**и т. д.'
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 51114eea797d27886f48c664d06d0b88d4a35a2d
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/10/2020
ms.locfileid: "43217913"
---
# <a name="privilegedrole-resource-type"></a><span data-ttu-id="c740c-103">Тип ресурса Привилежедроле</span><span class="sxs-lookup"><span data-stu-id="c740c-103">privilegedRole resource type</span></span>

<span data-ttu-id="c740c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c740c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c740c-105">Представляет роль администратора Azure AD, например: **глобальному администратору, администратору выставления счетов, администратору служб, администратору пользователей, администратору паролей**и т. д.</span><span class="sxs-lookup"><span data-stu-id="c740c-105">Represents an Azure AD administrator role, such as: **Global Administrator, Billing Administrator, Service Administrator, User Administrator, Password Administrator**, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="c740c-106">Методы</span><span class="sxs-lookup"><span data-stu-id="c740c-106">Methods</span></span>

| <span data-ttu-id="c740c-107">Метод</span><span class="sxs-lookup"><span data-stu-id="c740c-107">Method</span></span>           | <span data-ttu-id="c740c-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c740c-108">Return Type</span></span>    |<span data-ttu-id="c740c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="c740c-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c740c-110">Список объектов Привилежедроле</span><span class="sxs-lookup"><span data-stu-id="c740c-110">List privilegedRole objects</span></span>](../api/privilegedrole-list.md) | <span data-ttu-id="c740c-111">Коллекция [privilegedRole](privilegedrole.md)</span><span class="sxs-lookup"><span data-stu-id="c740c-111">[privilegedRole](privilegedrole.md) collection</span></span>|<span data-ttu-id="c740c-112">Получение коллекции Привилежедроле.</span><span class="sxs-lookup"><span data-stu-id="c740c-112">Get the collection of privilegedRole.</span></span>|
|[<span data-ttu-id="c740c-113">Получение privilegedRole</span><span class="sxs-lookup"><span data-stu-id="c740c-113">Get privilegedRole</span></span>](../api/privilegedrole-get.md) | [<span data-ttu-id="c740c-114">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="c740c-114">privilegedRole</span></span>](privilegedrole.md) |<span data-ttu-id="c740c-115">Чтение свойств и связей объекта Привилежедроле.</span><span class="sxs-lookup"><span data-stu-id="c740c-115">Read properties and relationships of privilegedRole object.</span></span>|
|[<span data-ttu-id="c740c-116">Перечисление заданий</span><span class="sxs-lookup"><span data-stu-id="c740c-116">List assignments</span></span>](../api/privilegedrole-list-assignments.md) |<span data-ttu-id="c740c-117">Коллекция [privilegedRoleAssignment](privilegedroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="c740c-117">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>| <span data-ttu-id="c740c-118">Получение коллекции объектов назначений для этой роли.</span><span class="sxs-lookup"><span data-stu-id="c740c-118">Get a assignment object collection for this role.</span></span>|
|[<span data-ttu-id="c740c-119">selfActivate</span><span class="sxs-lookup"><span data-stu-id="c740c-119">selfActivate</span></span>](../api/privilegedrole-selfactivate.md)|[<span data-ttu-id="c740c-120">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="c740c-120">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="c740c-121">Активируйте назначенную роль.</span><span class="sxs-lookup"><span data-stu-id="c740c-121">Activate the assigned role.</span></span>|
|[<span data-ttu-id="c740c-122">selfDeactivate</span><span class="sxs-lookup"><span data-stu-id="c740c-122">selfDeactivate</span></span>](../api/privilegedrole-selfdeactivate.md)|[<span data-ttu-id="c740c-123">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="c740c-123">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="c740c-124">Деактивация назначенной роли.</span><span class="sxs-lookup"><span data-stu-id="c740c-124">Deactivate the assigned role.</span></span>|

## <a name="properties"></a><span data-ttu-id="c740c-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="c740c-125">Properties</span></span>
| <span data-ttu-id="c740c-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="c740c-126">Property</span></span>     | <span data-ttu-id="c740c-127">Тип</span><span class="sxs-lookup"><span data-stu-id="c740c-127">Type</span></span>   |<span data-ttu-id="c740c-128">Описание</span><span class="sxs-lookup"><span data-stu-id="c740c-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c740c-129">id</span><span class="sxs-lookup"><span data-stu-id="c740c-129">id</span></span>|<span data-ttu-id="c740c-130">строка</span><span class="sxs-lookup"><span data-stu-id="c740c-130">string</span></span>|<span data-ttu-id="c740c-131">Уникальный идентификатор для роли администратора.</span><span class="sxs-lookup"><span data-stu-id="c740c-131">The unique identifier for administrator role.</span></span> <span data-ttu-id="c740c-132">Это строка GUID, имеющая то же значение, что и идентификатор шаблона роли из Azure AD для заданной роли.</span><span class="sxs-lookup"><span data-stu-id="c740c-132">It is a GUID string and has the same value as the role template id from Azure AD for the given role.</span></span> <span data-ttu-id="c740c-133">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c740c-133">Read-only.</span></span>|
|<span data-ttu-id="c740c-134">name</span><span class="sxs-lookup"><span data-stu-id="c740c-134">name</span></span>|<span data-ttu-id="c740c-135">string</span><span class="sxs-lookup"><span data-stu-id="c740c-135">string</span></span>|<span data-ttu-id="c740c-136">Имя роли.</span><span class="sxs-lookup"><span data-stu-id="c740c-136">Role name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c740c-137">Отношения</span><span class="sxs-lookup"><span data-stu-id="c740c-137">Relationships</span></span>
| <span data-ttu-id="c740c-138">Связь</span><span class="sxs-lookup"><span data-stu-id="c740c-138">Relationship</span></span> | <span data-ttu-id="c740c-139">Тип</span><span class="sxs-lookup"><span data-stu-id="c740c-139">Type</span></span>   |<span data-ttu-id="c740c-140">Описание</span><span class="sxs-lookup"><span data-stu-id="c740c-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c740c-141">assignments</span><span class="sxs-lookup"><span data-stu-id="c740c-141">assignments</span></span>|<span data-ttu-id="c740c-142">Коллекция [privilegedRoleAssignment](privilegedroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="c740c-142">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>| <span data-ttu-id="c740c-143">Назначения для этой роли.</span><span class="sxs-lookup"><span data-stu-id="c740c-143">The assignments for this role.</span></span> <span data-ttu-id="c740c-144">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c740c-144">Read-only.</span></span> <span data-ttu-id="c740c-145">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="c740c-145">Nullable.</span></span>|
|<span data-ttu-id="c740c-146">settings</span><span class="sxs-lookup"><span data-stu-id="c740c-146">settings</span></span>|[<span data-ttu-id="c740c-147">privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="c740c-147">privilegedRoleSettings</span></span>](privilegedrolesettings.md)| <span data-ttu-id="c740c-148">Параметры для этой роли.</span><span class="sxs-lookup"><span data-stu-id="c740c-148">The settings for this role.</span></span> <span data-ttu-id="c740c-149">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c740c-149">Read-only.</span></span> <span data-ttu-id="c740c-150">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="c740c-150">Nullable.</span></span>|
|<span data-ttu-id="c740c-151">summary</span><span class="sxs-lookup"><span data-stu-id="c740c-151">summary</span></span>|[<span data-ttu-id="c740c-152">privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="c740c-152">privilegedRoleSummary</span></span>](privilegedrolesummary.md)| <span data-ttu-id="c740c-153">Сводные данные для этой роли.</span><span class="sxs-lookup"><span data-stu-id="c740c-153">The summary information for this role.</span></span> <span data-ttu-id="c740c-154">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c740c-154">Read-only.</span></span> <span data-ttu-id="c740c-155">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="c740c-155">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c740c-156">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c740c-156">JSON representation</span></span>

<span data-ttu-id="c740c-157">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c740c-157">Here is a JSON representation of the resource.</span></span>

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
