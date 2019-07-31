---
title: Тип ресурса Привилежедроле
description: 'Представляет роль администратора Azure AD, например: глобальному **администратору, администратору выставления счетов, администратору служб, администратору пользователей, администратору паролей**и т. д.'
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 98e5cd2c53b398339e8db65bec520a16f72d8f39
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965749"
---
# <a name="privilegedrole-resource-type"></a><span data-ttu-id="75bd5-103">Тип ресурса Привилежедроле</span><span class="sxs-lookup"><span data-stu-id="75bd5-103">privilegedRole resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="75bd5-104">Представляет роль администратора Azure AD, например: глобальному **администратору, администратору выставления счетов, администратору служб, администратору пользователей, администратору паролей**и т. д.</span><span class="sxs-lookup"><span data-stu-id="75bd5-104">Represents an Azure AD administrator role, such as: **Global Administrator, Billing Administrator, Service Administrator, User Administrator, Password Administrator**, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="75bd5-105">Методы</span><span class="sxs-lookup"><span data-stu-id="75bd5-105">Methods</span></span>

| <span data-ttu-id="75bd5-106">Метод</span><span class="sxs-lookup"><span data-stu-id="75bd5-106">Method</span></span>           | <span data-ttu-id="75bd5-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="75bd5-107">Return Type</span></span>    |<span data-ttu-id="75bd5-108">Описание</span><span class="sxs-lookup"><span data-stu-id="75bd5-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="75bd5-109">Список объектов Привилежедроле</span><span class="sxs-lookup"><span data-stu-id="75bd5-109">List privilegedRole objects</span></span>](../api/privilegedrole-list.md) | <span data-ttu-id="75bd5-110">Коллекция [privilegedRole](privilegedrole.md)</span><span class="sxs-lookup"><span data-stu-id="75bd5-110">[privilegedRole](privilegedrole.md) collection</span></span>|<span data-ttu-id="75bd5-111">Получение коллекции Привилежедроле.</span><span class="sxs-lookup"><span data-stu-id="75bd5-111">Get the collection of privilegedRole.</span></span>|
|[<span data-ttu-id="75bd5-112">Получение privilegedRole</span><span class="sxs-lookup"><span data-stu-id="75bd5-112">Get privilegedRole</span></span>](../api/privilegedrole-get.md) | [<span data-ttu-id="75bd5-113">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="75bd5-113">privilegedRole</span></span>](privilegedrole.md) |<span data-ttu-id="75bd5-114">Чтение свойств и связей объекта Привилежедроле.</span><span class="sxs-lookup"><span data-stu-id="75bd5-114">Read properties and relationships of privilegedRole object.</span></span>|
|[<span data-ttu-id="75bd5-115">Перечисление заданий</span><span class="sxs-lookup"><span data-stu-id="75bd5-115">List assignments</span></span>](../api/privilegedrole-list-assignments.md) |<span data-ttu-id="75bd5-116">Коллекция [privilegedRoleAssignment](privilegedroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="75bd5-116">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>| <span data-ttu-id="75bd5-117">Получение коллекции объектов назначений для этой роли.</span><span class="sxs-lookup"><span data-stu-id="75bd5-117">Get a assignment object collection for this role.</span></span>|
|[<span data-ttu-id="75bd5-118">selfActivate</span><span class="sxs-lookup"><span data-stu-id="75bd5-118">selfActivate</span></span>](../api/privilegedrole-selfactivate.md)|[<span data-ttu-id="75bd5-119">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="75bd5-119">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="75bd5-120">Активируйте назначенную роль.</span><span class="sxs-lookup"><span data-stu-id="75bd5-120">Activate the assigned role.</span></span>|
|[<span data-ttu-id="75bd5-121">selfDeactivate</span><span class="sxs-lookup"><span data-stu-id="75bd5-121">selfDeactivate</span></span>](../api/privilegedrole-selfdeactivate.md)|[<span data-ttu-id="75bd5-122">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="75bd5-122">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="75bd5-123">Деактивация назначенной роли.</span><span class="sxs-lookup"><span data-stu-id="75bd5-123">Deactivate the assigned role.</span></span>|

## <a name="properties"></a><span data-ttu-id="75bd5-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="75bd5-124">Properties</span></span>
| <span data-ttu-id="75bd5-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="75bd5-125">Property</span></span>     | <span data-ttu-id="75bd5-126">Тип</span><span class="sxs-lookup"><span data-stu-id="75bd5-126">Type</span></span>   |<span data-ttu-id="75bd5-127">Описание</span><span class="sxs-lookup"><span data-stu-id="75bd5-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="75bd5-128">id</span><span class="sxs-lookup"><span data-stu-id="75bd5-128">id</span></span>|<span data-ttu-id="75bd5-129">string</span><span class="sxs-lookup"><span data-stu-id="75bd5-129">string</span></span>|<span data-ttu-id="75bd5-130">Уникальный идентификатор для роли администратора.</span><span class="sxs-lookup"><span data-stu-id="75bd5-130">The unique identifier for administrator role.</span></span> <span data-ttu-id="75bd5-131">Это строка GUID, имеющая то же значение, что и идентификатор шаблона роли из Azure AD для заданной роли.</span><span class="sxs-lookup"><span data-stu-id="75bd5-131">It is a GUID string and has the same value as the role template id from Azure AD for the given role.</span></span> <span data-ttu-id="75bd5-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="75bd5-132">Read-only.</span></span>|
|<span data-ttu-id="75bd5-133">name</span><span class="sxs-lookup"><span data-stu-id="75bd5-133">name</span></span>|<span data-ttu-id="75bd5-134">string</span><span class="sxs-lookup"><span data-stu-id="75bd5-134">string</span></span>|<span data-ttu-id="75bd5-135">Имя роли.</span><span class="sxs-lookup"><span data-stu-id="75bd5-135">Role name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="75bd5-136">Отношения</span><span class="sxs-lookup"><span data-stu-id="75bd5-136">Relationships</span></span>
| <span data-ttu-id="75bd5-137">Отношение</span><span class="sxs-lookup"><span data-stu-id="75bd5-137">Relationship</span></span> | <span data-ttu-id="75bd5-138">Тип</span><span class="sxs-lookup"><span data-stu-id="75bd5-138">Type</span></span>   |<span data-ttu-id="75bd5-139">Описание</span><span class="sxs-lookup"><span data-stu-id="75bd5-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="75bd5-140">assignments</span><span class="sxs-lookup"><span data-stu-id="75bd5-140">assignments</span></span>|<span data-ttu-id="75bd5-141">Коллекция [privilegedRoleAssignment](privilegedroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="75bd5-141">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>| <span data-ttu-id="75bd5-142">Назначения для этой роли.</span><span class="sxs-lookup"><span data-stu-id="75bd5-142">The assignments for this role.</span></span> <span data-ttu-id="75bd5-143">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="75bd5-143">Read-only.</span></span> <span data-ttu-id="75bd5-144">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="75bd5-144">Nullable.</span></span>|
|<span data-ttu-id="75bd5-145">settings</span><span class="sxs-lookup"><span data-stu-id="75bd5-145">settings</span></span>|[<span data-ttu-id="75bd5-146">privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="75bd5-146">privilegedRoleSettings</span></span>](privilegedrolesettings.md)| <span data-ttu-id="75bd5-147">Параметры для этой роли.</span><span class="sxs-lookup"><span data-stu-id="75bd5-147">The settings for this role.</span></span> <span data-ttu-id="75bd5-148">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="75bd5-148">Read-only.</span></span> <span data-ttu-id="75bd5-149">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="75bd5-149">Nullable.</span></span>|
|<span data-ttu-id="75bd5-150">summary</span><span class="sxs-lookup"><span data-stu-id="75bd5-150">summary</span></span>|[<span data-ttu-id="75bd5-151">privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="75bd5-151">privilegedRoleSummary</span></span>](privilegedrolesummary.md)| <span data-ttu-id="75bd5-152">Сводные данные для этой роли.</span><span class="sxs-lookup"><span data-stu-id="75bd5-152">The summary information for this role.</span></span> <span data-ttu-id="75bd5-153">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="75bd5-153">Read-only.</span></span> <span data-ttu-id="75bd5-154">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="75bd5-154">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="75bd5-155">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="75bd5-155">JSON representation</span></span>

<span data-ttu-id="75bd5-156">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="75bd5-156">Here is a JSON representation of the resource.</span></span>

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
