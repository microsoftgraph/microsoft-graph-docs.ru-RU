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
# <a name="privilegedrole-resource-type"></a><span data-ttu-id="3815d-103">Тип ресурса Привилежедроле</span><span class="sxs-lookup"><span data-stu-id="3815d-103">privilegedRole resource type</span></span>

<span data-ttu-id="3815d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3815d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3815d-105">Представляет роль администратора Azure AD, например: **глобальному администратору, администратору выставления счетов, администратору служб, администратору пользователей, администратору паролей**и т. д.</span><span class="sxs-lookup"><span data-stu-id="3815d-105">Represents an Azure AD administrator role, such as: **Global Administrator, Billing Administrator, Service Administrator, User Administrator, Password Administrator**, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="3815d-106">Методы</span><span class="sxs-lookup"><span data-stu-id="3815d-106">Methods</span></span>

| <span data-ttu-id="3815d-107">Метод</span><span class="sxs-lookup"><span data-stu-id="3815d-107">Method</span></span>           | <span data-ttu-id="3815d-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="3815d-108">Return Type</span></span>    |<span data-ttu-id="3815d-109">Описание</span><span class="sxs-lookup"><span data-stu-id="3815d-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3815d-110">Список объектов Привилежедроле</span><span class="sxs-lookup"><span data-stu-id="3815d-110">List privilegedRole objects</span></span>](../api/privilegedrole-list.md) | <span data-ttu-id="3815d-111">Коллекция [privilegedRole](privilegedrole.md)</span><span class="sxs-lookup"><span data-stu-id="3815d-111">[privilegedRole](privilegedrole.md) collection</span></span>|<span data-ttu-id="3815d-112">Получение коллекции Привилежедроле.</span><span class="sxs-lookup"><span data-stu-id="3815d-112">Get the collection of privilegedRole.</span></span>|
|[<span data-ttu-id="3815d-113">Получение privilegedRole</span><span class="sxs-lookup"><span data-stu-id="3815d-113">Get privilegedRole</span></span>](../api/privilegedrole-get.md) | [<span data-ttu-id="3815d-114">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="3815d-114">privilegedRole</span></span>](privilegedrole.md) |<span data-ttu-id="3815d-115">Чтение свойств и связей объекта Привилежедроле.</span><span class="sxs-lookup"><span data-stu-id="3815d-115">Read properties and relationships of privilegedRole object.</span></span>|
|[<span data-ttu-id="3815d-116">Перечисление заданий</span><span class="sxs-lookup"><span data-stu-id="3815d-116">List assignments</span></span>](../api/privilegedrole-list-assignments.md) |<span data-ttu-id="3815d-117">Коллекция [privilegedRoleAssignment](privilegedroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="3815d-117">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>| <span data-ttu-id="3815d-118">Получение коллекции объектов назначений для этой роли.</span><span class="sxs-lookup"><span data-stu-id="3815d-118">Get a assignment object collection for this role.</span></span>|
|[<span data-ttu-id="3815d-119">selfActivate</span><span class="sxs-lookup"><span data-stu-id="3815d-119">selfActivate</span></span>](../api/privilegedrole-selfactivate.md)|[<span data-ttu-id="3815d-120">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="3815d-120">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="3815d-121">Активируйте назначенную роль.</span><span class="sxs-lookup"><span data-stu-id="3815d-121">Activate the assigned role.</span></span>|
|[<span data-ttu-id="3815d-122">selfDeactivate</span><span class="sxs-lookup"><span data-stu-id="3815d-122">selfDeactivate</span></span>](../api/privilegedrole-selfdeactivate.md)|[<span data-ttu-id="3815d-123">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="3815d-123">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="3815d-124">Деактивация назначенной роли.</span><span class="sxs-lookup"><span data-stu-id="3815d-124">Deactivate the assigned role.</span></span>|

## <a name="properties"></a><span data-ttu-id="3815d-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="3815d-125">Properties</span></span>
| <span data-ttu-id="3815d-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="3815d-126">Property</span></span>     | <span data-ttu-id="3815d-127">Тип</span><span class="sxs-lookup"><span data-stu-id="3815d-127">Type</span></span>   |<span data-ttu-id="3815d-128">Описание</span><span class="sxs-lookup"><span data-stu-id="3815d-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3815d-129">id</span><span class="sxs-lookup"><span data-stu-id="3815d-129">id</span></span>|<span data-ttu-id="3815d-130">строка</span><span class="sxs-lookup"><span data-stu-id="3815d-130">string</span></span>|<span data-ttu-id="3815d-131">Уникальный идентификатор для роли администратора.</span><span class="sxs-lookup"><span data-stu-id="3815d-131">The unique identifier for administrator role.</span></span> <span data-ttu-id="3815d-132">Это строка GUID, имеющая то же значение, что и идентификатор шаблона роли из Azure AD для заданной роли.</span><span class="sxs-lookup"><span data-stu-id="3815d-132">It is a GUID string and has the same value as the role template id from Azure AD for the given role.</span></span> <span data-ttu-id="3815d-133">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3815d-133">Read-only.</span></span>|
|<span data-ttu-id="3815d-134">name</span><span class="sxs-lookup"><span data-stu-id="3815d-134">name</span></span>|<span data-ttu-id="3815d-135">string</span><span class="sxs-lookup"><span data-stu-id="3815d-135">string</span></span>|<span data-ttu-id="3815d-136">Имя роли.</span><span class="sxs-lookup"><span data-stu-id="3815d-136">Role name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3815d-137">Связи</span><span class="sxs-lookup"><span data-stu-id="3815d-137">Relationships</span></span>
| <span data-ttu-id="3815d-138">Связь</span><span class="sxs-lookup"><span data-stu-id="3815d-138">Relationship</span></span> | <span data-ttu-id="3815d-139">Тип</span><span class="sxs-lookup"><span data-stu-id="3815d-139">Type</span></span>   |<span data-ttu-id="3815d-140">Описание</span><span class="sxs-lookup"><span data-stu-id="3815d-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3815d-141">assignments</span><span class="sxs-lookup"><span data-stu-id="3815d-141">assignments</span></span>|<span data-ttu-id="3815d-142">Коллекция [privilegedRoleAssignment](privilegedroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="3815d-142">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>| <span data-ttu-id="3815d-143">Назначения для этой роли.</span><span class="sxs-lookup"><span data-stu-id="3815d-143">The assignments for this role.</span></span> <span data-ttu-id="3815d-144">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3815d-144">Read-only.</span></span> <span data-ttu-id="3815d-145">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="3815d-145">Nullable.</span></span>|
|<span data-ttu-id="3815d-146">settings</span><span class="sxs-lookup"><span data-stu-id="3815d-146">settings</span></span>|[<span data-ttu-id="3815d-147">privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="3815d-147">privilegedRoleSettings</span></span>](privilegedrolesettings.md)| <span data-ttu-id="3815d-148">Параметры для этой роли.</span><span class="sxs-lookup"><span data-stu-id="3815d-148">The settings for this role.</span></span> <span data-ttu-id="3815d-149">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3815d-149">Read-only.</span></span> <span data-ttu-id="3815d-150">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="3815d-150">Nullable.</span></span>|
|<span data-ttu-id="3815d-151">summary</span><span class="sxs-lookup"><span data-stu-id="3815d-151">summary</span></span>|[<span data-ttu-id="3815d-152">privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="3815d-152">privilegedRoleSummary</span></span>](privilegedrolesummary.md)| <span data-ttu-id="3815d-153">Сводные данные для этой роли.</span><span class="sxs-lookup"><span data-stu-id="3815d-153">The summary information for this role.</span></span> <span data-ttu-id="3815d-154">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3815d-154">Read-only.</span></span> <span data-ttu-id="3815d-155">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="3815d-155">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3815d-156">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3815d-156">JSON representation</span></span>

<span data-ttu-id="3815d-157">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3815d-157">Here is a JSON representation of the resource.</span></span>

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
