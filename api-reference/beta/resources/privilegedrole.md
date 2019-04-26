---
title: Тип ресурса Привилежедроле
description: 'Представляет роль администратора Azure AD, например: глобальному **администратору, администратору выставленИя счетов, администратору служб, администратору пользователей, администратору паролей**и т. д.'
localization_priority: Normal
ms.openlocfilehash: 131999f52a583400b018e98d2319118f69ca87e8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563430"
---
# <a name="privilegedrole-resource-type"></a><span data-ttu-id="9b708-103">Тип ресурса Привилежедроле</span><span class="sxs-lookup"><span data-stu-id="9b708-103">privilegedRole resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9b708-104">Представляет роль администратора Azure AD, например: глобальному **администратору, администратору выставленИя счетов, администратору служб, администратору пользователей, администратору паролей**и т. д.</span><span class="sxs-lookup"><span data-stu-id="9b708-104">Represents an Azure AD administrator role, such as: **Global Administrator, Billing Administrator, Service Administrator, User Administrator, Password Administrator**, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="9b708-105">Методы</span><span class="sxs-lookup"><span data-stu-id="9b708-105">Methods</span></span>

| <span data-ttu-id="9b708-106">Метод</span><span class="sxs-lookup"><span data-stu-id="9b708-106">Method</span></span>           | <span data-ttu-id="9b708-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="9b708-107">Return Type</span></span>    |<span data-ttu-id="9b708-108">Описание</span><span class="sxs-lookup"><span data-stu-id="9b708-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9b708-109">Список объектов Привилежедроле</span><span class="sxs-lookup"><span data-stu-id="9b708-109">List privilegedRole objects</span></span>](../api/privilegedrole-list.md) | <span data-ttu-id="9b708-110">Коллекция [privilegedRole](privilegedrole.md)</span><span class="sxs-lookup"><span data-stu-id="9b708-110">[privilegedRole](privilegedrole.md) collection</span></span>|<span data-ttu-id="9b708-111">Получение коллекции Привилежедроле.</span><span class="sxs-lookup"><span data-stu-id="9b708-111">Get the collection of privilegedRole.</span></span>|
|[<span data-ttu-id="9b708-112">Получение privilegedRole</span><span class="sxs-lookup"><span data-stu-id="9b708-112">Get privilegedRole</span></span>](../api/privilegedrole-get.md) | [<span data-ttu-id="9b708-113">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="9b708-113">privilegedRole</span></span>](privilegedrole.md) |<span data-ttu-id="9b708-114">Чтение свойств и связей объекта Привилежедроле.</span><span class="sxs-lookup"><span data-stu-id="9b708-114">Read properties and relationships of privilegedRole object.</span></span>|
|[<span data-ttu-id="9b708-115">Перечисление заданий</span><span class="sxs-lookup"><span data-stu-id="9b708-115">List assignments</span></span>](../api/privilegedrole-list-assignments.md) |<span data-ttu-id="9b708-116">Коллекция [privilegedRoleAssignment](privilegedroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="9b708-116">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>| <span data-ttu-id="9b708-117">Получение коллекции объектов назначений для этой роли.</span><span class="sxs-lookup"><span data-stu-id="9b708-117">Get a assignment object collection for this role.</span></span>|
|[<span data-ttu-id="9b708-118">selfActivate</span><span class="sxs-lookup"><span data-stu-id="9b708-118">selfActivate</span></span>](../api/privilegedrole-selfactivate.md)|[<span data-ttu-id="9b708-119">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="9b708-119">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="9b708-120">Активируйте назначенную роль.</span><span class="sxs-lookup"><span data-stu-id="9b708-120">Activate the assigned role.</span></span>|
|[<span data-ttu-id="9b708-121">selfDeactivate</span><span class="sxs-lookup"><span data-stu-id="9b708-121">selfDeactivate</span></span>](../api/privilegedrole-selfdeactivate.md)|[<span data-ttu-id="9b708-122">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="9b708-122">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="9b708-123">ДеАктивация назначенной роли.</span><span class="sxs-lookup"><span data-stu-id="9b708-123">Deactivate the assigned role.</span></span>|

## <a name="properties"></a><span data-ttu-id="9b708-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="9b708-124">Properties</span></span>
| <span data-ttu-id="9b708-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="9b708-125">Property</span></span>     | <span data-ttu-id="9b708-126">Тип</span><span class="sxs-lookup"><span data-stu-id="9b708-126">Type</span></span>   |<span data-ttu-id="9b708-127">Описание</span><span class="sxs-lookup"><span data-stu-id="9b708-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9b708-128">id</span><span class="sxs-lookup"><span data-stu-id="9b708-128">id</span></span>|<span data-ttu-id="9b708-129">строка</span><span class="sxs-lookup"><span data-stu-id="9b708-129">string</span></span>|<span data-ttu-id="9b708-130">Уникальный идентификатор для роли администратора.</span><span class="sxs-lookup"><span data-stu-id="9b708-130">The unique identifier for administrator role.</span></span> <span data-ttu-id="9b708-131">Это строка GUID, имеющая то же значение, что и идентификатор шаблона роли из Azure AD для заданной роли.</span><span class="sxs-lookup"><span data-stu-id="9b708-131">It is a GUID string and has the same value as the role template id from Azure AD for the given role.</span></span> <span data-ttu-id="9b708-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9b708-132">Read-only.</span></span>|
|<span data-ttu-id="9b708-133">name</span><span class="sxs-lookup"><span data-stu-id="9b708-133">name</span></span>|<span data-ttu-id="9b708-134">string</span><span class="sxs-lookup"><span data-stu-id="9b708-134">string</span></span>|<span data-ttu-id="9b708-135">Имя роли.</span><span class="sxs-lookup"><span data-stu-id="9b708-135">Role name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9b708-136">Связи</span><span class="sxs-lookup"><span data-stu-id="9b708-136">Relationships</span></span>
| <span data-ttu-id="9b708-137">Отношение</span><span class="sxs-lookup"><span data-stu-id="9b708-137">Relationship</span></span> | <span data-ttu-id="9b708-138">Тип</span><span class="sxs-lookup"><span data-stu-id="9b708-138">Type</span></span>   |<span data-ttu-id="9b708-139">Описание</span><span class="sxs-lookup"><span data-stu-id="9b708-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9b708-140">assignments</span><span class="sxs-lookup"><span data-stu-id="9b708-140">assignments</span></span>|<span data-ttu-id="9b708-141">Коллекция [privilegedRoleAssignment](privilegedroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="9b708-141">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>| <span data-ttu-id="9b708-142">Назначения для этой роли.</span><span class="sxs-lookup"><span data-stu-id="9b708-142">The assignments for this role.</span></span> <span data-ttu-id="9b708-143">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9b708-143">Read-only.</span></span> <span data-ttu-id="9b708-144">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="9b708-144">Nullable.</span></span>|
|<span data-ttu-id="9b708-145">settings</span><span class="sxs-lookup"><span data-stu-id="9b708-145">settings</span></span>|[<span data-ttu-id="9b708-146">privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="9b708-146">privilegedRoleSettings</span></span>](privilegedrolesettings.md)| <span data-ttu-id="9b708-147">Параметры для этой роли.</span><span class="sxs-lookup"><span data-stu-id="9b708-147">The settings for this role.</span></span> <span data-ttu-id="9b708-148">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9b708-148">Read-only.</span></span> <span data-ttu-id="9b708-149">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="9b708-149">Nullable.</span></span>|
|<span data-ttu-id="9b708-150">summary</span><span class="sxs-lookup"><span data-stu-id="9b708-150">summary</span></span>|[<span data-ttu-id="9b708-151">privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="9b708-151">privilegedRoleSummary</span></span>](privilegedrolesummary.md)| <span data-ttu-id="9b708-152">Сводные данные для этой роли.</span><span class="sxs-lookup"><span data-stu-id="9b708-152">The summary information for this role.</span></span> <span data-ttu-id="9b708-153">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9b708-153">Read-only.</span></span> <span data-ttu-id="9b708-154">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="9b708-154">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9b708-155">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9b708-155">JSON representation</span></span>

<span data-ttu-id="9b708-156">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9b708-156">Here is a JSON representation of the resource.</span></span>

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
