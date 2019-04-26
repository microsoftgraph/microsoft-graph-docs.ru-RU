---
title: Тип ресурса Привилежедроле
description: 'Представляет роль администратора Azure AD, например: глобальному **администратору, администратору выставленИя счетов, администратору служб, администратору пользователей, администратору паролей**и т. д.'
localization_priority: Normal
ms.openlocfilehash: 9b5454745257bea071f967b654d3b6174c3c3289
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344298"
---
# <a name="privilegedrole-resource-type"></a><span data-ttu-id="1df48-103">Тип ресурса Привилежедроле</span><span class="sxs-lookup"><span data-stu-id="1df48-103">privilegedRole resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1df48-104">Представляет роль администратора Azure AD, например: глобальному **администратору, администратору выставленИя счетов, администратору служб, администратору пользователей, администратору паролей**и т. д.</span><span class="sxs-lookup"><span data-stu-id="1df48-104">Represents an Azure AD administrator role, such as: **Global Administrator, Billing Administrator, Service Administrator, User Administrator, Password Administrator**, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="1df48-105">Методы</span><span class="sxs-lookup"><span data-stu-id="1df48-105">Methods</span></span>

| <span data-ttu-id="1df48-106">Метод</span><span class="sxs-lookup"><span data-stu-id="1df48-106">Method</span></span>           | <span data-ttu-id="1df48-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1df48-107">Return Type</span></span>    |<span data-ttu-id="1df48-108">Описание</span><span class="sxs-lookup"><span data-stu-id="1df48-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1df48-109">Список объектов Привилежедроле</span><span class="sxs-lookup"><span data-stu-id="1df48-109">List privilegedRole objects</span></span>](../api/privilegedrole-list.md) | <span data-ttu-id="1df48-110">Коллекция [privilegedRole](privilegedrole.md)</span><span class="sxs-lookup"><span data-stu-id="1df48-110">[privilegedRole](privilegedrole.md) collection</span></span>|<span data-ttu-id="1df48-111">Получение коллекции Привилежедроле.</span><span class="sxs-lookup"><span data-stu-id="1df48-111">Get the collection of privilegedRole.</span></span>|
|[<span data-ttu-id="1df48-112">Получение privilegedRole</span><span class="sxs-lookup"><span data-stu-id="1df48-112">Get privilegedRole</span></span>](../api/privilegedrole-get.md) | [<span data-ttu-id="1df48-113">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="1df48-113">privilegedRole</span></span>](privilegedrole.md) |<span data-ttu-id="1df48-114">Чтение свойств и связей объекта Привилежедроле.</span><span class="sxs-lookup"><span data-stu-id="1df48-114">Read properties and relationships of privilegedRole object.</span></span>|
|[<span data-ttu-id="1df48-115">Перечисление заданий</span><span class="sxs-lookup"><span data-stu-id="1df48-115">List assignments</span></span>](../api/privilegedrole-list-assignments.md) |<span data-ttu-id="1df48-116">Коллекция [privilegedRoleAssignment](privilegedroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="1df48-116">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>| <span data-ttu-id="1df48-117">Получение коллекции объектов назначений для этой роли.</span><span class="sxs-lookup"><span data-stu-id="1df48-117">Get a assignment object collection for this role.</span></span>|
|[<span data-ttu-id="1df48-118">selfActivate</span><span class="sxs-lookup"><span data-stu-id="1df48-118">selfActivate</span></span>](../api/privilegedrole-selfactivate.md)|[<span data-ttu-id="1df48-119">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="1df48-119">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="1df48-120">Активируйте назначенную роль.</span><span class="sxs-lookup"><span data-stu-id="1df48-120">Activate the assigned role.</span></span>|
|[<span data-ttu-id="1df48-121">selfDeactivate</span><span class="sxs-lookup"><span data-stu-id="1df48-121">selfDeactivate</span></span>](../api/privilegedrole-selfdeactivate.md)|[<span data-ttu-id="1df48-122">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="1df48-122">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="1df48-123">ДеАктивация назначенной роли.</span><span class="sxs-lookup"><span data-stu-id="1df48-123">Deactivate the assigned role.</span></span>|

## <a name="properties"></a><span data-ttu-id="1df48-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="1df48-124">Properties</span></span>
| <span data-ttu-id="1df48-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="1df48-125">Property</span></span>     | <span data-ttu-id="1df48-126">Тип</span><span class="sxs-lookup"><span data-stu-id="1df48-126">Type</span></span>   |<span data-ttu-id="1df48-127">Описание</span><span class="sxs-lookup"><span data-stu-id="1df48-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1df48-128">id</span><span class="sxs-lookup"><span data-stu-id="1df48-128">id</span></span>|<span data-ttu-id="1df48-129">строка</span><span class="sxs-lookup"><span data-stu-id="1df48-129">string</span></span>|<span data-ttu-id="1df48-130">Уникальный идентификатор для роли администратора.</span><span class="sxs-lookup"><span data-stu-id="1df48-130">The unique identifier for administrator role.</span></span> <span data-ttu-id="1df48-131">Это строка GUID, имеющая то же значение, что и идентификатор шаблона роли из Azure AD для заданной роли.</span><span class="sxs-lookup"><span data-stu-id="1df48-131">It is a GUID string and has the same value as the role template id from Azure AD for the given role.</span></span> <span data-ttu-id="1df48-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1df48-132">Read-only.</span></span>|
|<span data-ttu-id="1df48-133">name</span><span class="sxs-lookup"><span data-stu-id="1df48-133">name</span></span>|<span data-ttu-id="1df48-134">string</span><span class="sxs-lookup"><span data-stu-id="1df48-134">string</span></span>|<span data-ttu-id="1df48-135">Имя роли.</span><span class="sxs-lookup"><span data-stu-id="1df48-135">Role name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1df48-136">Связи</span><span class="sxs-lookup"><span data-stu-id="1df48-136">Relationships</span></span>
| <span data-ttu-id="1df48-137">Отношение</span><span class="sxs-lookup"><span data-stu-id="1df48-137">Relationship</span></span> | <span data-ttu-id="1df48-138">Тип</span><span class="sxs-lookup"><span data-stu-id="1df48-138">Type</span></span>   |<span data-ttu-id="1df48-139">Описание</span><span class="sxs-lookup"><span data-stu-id="1df48-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1df48-140">assignments</span><span class="sxs-lookup"><span data-stu-id="1df48-140">assignments</span></span>|<span data-ttu-id="1df48-141">Коллекция [privilegedRoleAssignment](privilegedroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="1df48-141">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>| <span data-ttu-id="1df48-142">Назначения для этой роли.</span><span class="sxs-lookup"><span data-stu-id="1df48-142">The assignments for this role.</span></span> <span data-ttu-id="1df48-143">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1df48-143">Read-only.</span></span> <span data-ttu-id="1df48-144">Допускает значение null.</span><span class="sxs-lookup"><span data-stu-id="1df48-144">Nullable.</span></span>|
|<span data-ttu-id="1df48-145">settings</span><span class="sxs-lookup"><span data-stu-id="1df48-145">settings</span></span>|[<span data-ttu-id="1df48-146">privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="1df48-146">privilegedRoleSettings</span></span>](privilegedrolesettings.md)| <span data-ttu-id="1df48-147">Параметры для этой роли.</span><span class="sxs-lookup"><span data-stu-id="1df48-147">The settings for this role.</span></span> <span data-ttu-id="1df48-148">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1df48-148">Read-only.</span></span> <span data-ttu-id="1df48-149">Допускает значение null.</span><span class="sxs-lookup"><span data-stu-id="1df48-149">Nullable.</span></span>|
|<span data-ttu-id="1df48-150">summary</span><span class="sxs-lookup"><span data-stu-id="1df48-150">summary</span></span>|[<span data-ttu-id="1df48-151">privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="1df48-151">privilegedRoleSummary</span></span>](privilegedrolesummary.md)| <span data-ttu-id="1df48-152">Сводные данные для этой роли.</span><span class="sxs-lookup"><span data-stu-id="1df48-152">The summary information for this role.</span></span> <span data-ttu-id="1df48-153">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1df48-153">Read-only.</span></span> <span data-ttu-id="1df48-154">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="1df48-154">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1df48-155">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1df48-155">JSON representation</span></span>

<span data-ttu-id="1df48-156">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1df48-156">Here is a JSON representation of the resource.</span></span>

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
