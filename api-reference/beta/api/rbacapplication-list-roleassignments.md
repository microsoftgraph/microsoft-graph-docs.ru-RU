---
title: Список Унифиедролеассигнментс
description: Получение списка объектов Унифиедролеассигнмент.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8a9458a16f9d2d8dabce4514bafef7aef50fb7fd
ms.sourcegitcommit: 9edfcf99706c8490cd5832a1c706a88a89e24db1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/07/2020
ms.locfileid: "43160270"
---
# <a name="list-unifiedroleassignments"></a><span data-ttu-id="91066-103">Список Унифиедролеассигнментс</span><span class="sxs-lookup"><span data-stu-id="91066-103">List unifiedRoleAssignments</span></span>

<span data-ttu-id="91066-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="91066-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="91066-105">Получение списка объектов [унифиедролеассигнмент](../resources/unifiedroleassignment.md) для поставщика.</span><span class="sxs-lookup"><span data-stu-id="91066-105">Get a list of [unifiedRoleAssignment](../resources/unifiedroleassignment.md) objects for the provider.</span></span>

## <a name="permissions"></a><span data-ttu-id="91066-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="91066-106">Permissions</span></span>

<span data-ttu-id="91066-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91066-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91066-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="91066-109">Permission type</span></span>      | <span data-ttu-id="91066-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="91066-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="91066-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="91066-111">Delegated (work or school account)</span></span> | <span data-ttu-id="91066-112">Ролеманажемент. Read. Directory, Directory. Read. ALL, Ролеманажемент. ReadWrite. Directory, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="91066-112">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="91066-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="91066-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="91066-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="91066-114">Not supported.</span></span>    |
|<span data-ttu-id="91066-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="91066-115">Application</span></span> | <span data-ttu-id="91066-116">Ролеманажемент. Read. Directory, Directory. Read. ALL, Ролеманажемент. ReadWrite. Directory, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="91066-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="91066-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="91066-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /roleManagement/directory/roleAssignments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="91066-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="91066-118">Optional query parameters</span></span>

<span data-ttu-id="91066-119">Для `$filter` выполнения этой операции требуется параметр запроса.</span><span class="sxs-lookup"><span data-stu-id="91066-119">This operation requires the `$filter` query parameter.</span></span> <span data-ttu-id="91066-120">Вы можете отфильтровать `roleDefinitionId` по `principalId` свойствам или.</span><span class="sxs-lookup"><span data-stu-id="91066-120">You can filter on the `roleDefinitionId` or `principalId` properties.</span></span> <span data-ttu-id="91066-121">`roleDefinitionId` Свойство может быть идентификатором объекта Role или шаблоном роли.</span><span class="sxs-lookup"><span data-stu-id="91066-121">The `roleDefinitionId` property can be either a role object ID or a role template object ID.</span></span> <span data-ttu-id="91066-122">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="91066-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="91066-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="91066-123">Request headers</span></span>

| <span data-ttu-id="91066-124">Имя</span><span class="sxs-lookup"><span data-stu-id="91066-124">Name</span></span>      |<span data-ttu-id="91066-125">Описание</span><span class="sxs-lookup"><span data-stu-id="91066-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="91066-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="91066-126">Authorization</span></span> | <span data-ttu-id="91066-127">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="91066-127">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="91066-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="91066-128">Request body</span></span>

<span data-ttu-id="91066-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="91066-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="91066-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="91066-130">Response</span></span>

<span data-ttu-id="91066-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [унифиедролеассигнмент](../resources/unifiedroleassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="91066-131">If successful, this method returns a `200 OK` response code and a collection of [unifiedRoleAssignment](../resources/unifiedroleassignment.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="91066-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="91066-132">Examples</span></span>

### <a name="example-1-request-using-a-filter-on-role-definition-id"></a><span data-ttu-id="91066-133">Пример 1: запрос с использованием фильтра по ИДЕНТИФИКАТОРу определения роли</span><span class="sxs-lookup"><span data-stu-id="91066-133">Example 1: Request using a filter on role definition ID</span></span>

#### <a name="request"></a><span data-ttu-id="91066-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="91066-134">Request</span></span>

<span data-ttu-id="91066-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="91066-135">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_roleAssignments"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments?$filter=roleDefinitionId eq '62e90394-69f5-4237-9190-012177145e10'
```

#### <a name="response"></a><span data-ttu-id="91066-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="91066-136">Response</span></span>

<span data-ttu-id="91066-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="91066-137">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignment",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleAssignments",
    "value": [
        {
            "@odata.type": "#microsoft.graph.unifiedRoleAssignment",
            "id": "lAPpYvVpN0KRkAEhdxReEGm3jqnUe4lEhvatluHVi2I-1",
            "roleDefinitionId": "62e90394-69f5-4237-9190-012177145e10",
            "principalId": "a98eb769-7bd4-4489-86f6-ad96e1d58b62",
            "directoryScopeId": "/"
        },
        {
            "@odata.type": "#microsoft.graph.unifiedRoleAssignment",
            "id": "lAPpYvVpN0KRkAEhdxReEGnbHktRMANMpnGtLZ3MXeY-1",
            "roleDefinitionId": "62e90394-69f5-4237-9190-012177145e10",
            "principalId": "4b1edb69-3051-4c03-a671-ad2d9dcc5de6",
            "directoryScopeId": "/"
        },
        {
            "@odata.type": "#microsoft.graph.unifiedRoleAssignment",
            "id": "lAPpYvVpN0KRkAEhdxReEKLh1vKaL9NIi6cTuyyN_6Q-1",
            "roleDefinitionId": "62e90394-69f5-4237-9190-012177145e10",
            "principalId": "f2d6e1a2-2f9a-48d3-8ba7-13bb2c8dffa4",
            "directoryScopeId": "/"
        },
        {
            "@odata.type": "#microsoft.graph.unifiedRoleAssignment",
            "id": "lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1",
            "roleDefinitionId": "62e90394-69f5-4237-9190-012177145e10",
            "principalId": "4ab0b690-479b-47ff-af8f-2576cf521872",
            "directoryScopeId": "/"
        },
        {
            "@odata.type": "#microsoft.graph.unifiedRoleAssignment",
            "id": "lAPpYvVpN0KRkAEhdxReEGXxIcn3O7hBqaGB0NGuCwE-1",
            "roleDefinitionId": "62e90394-69f5-4237-9190-012177145e10",
            "principalId": "c921f165-3bf7-41b8-a9a1-81d0d1ae0b01",
            "directoryScopeId": "/"
        },
        {
            "@odata.type": "#microsoft.graph.unifiedRoleAssignment",
            "id": "lAPpYvVpN0KRkAEhdxReEAWO6-FSXqhEg1mkkLETmA8-1",
            "roleDefinitionId": "62e90394-69f5-4237-9190-012177145e10",
            "principalId": "e1eb8e05-5e52-44a8-8359-a490b113980f",
            "directoryScopeId": "/"
        }
    ]
}
```

### <a name="example-2-request-using-a-filter-on-principal-id"></a><span data-ttu-id="91066-138">Пример 2: запрос с использованием фильтра по ИДЕНТИФИКАТОРу субъекта</span><span class="sxs-lookup"><span data-stu-id="91066-138">Example 2: Request using a filter on principal ID</span></span>

#### <a name="request"></a><span data-ttu-id="91066-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="91066-139">Request</span></span>

<span data-ttu-id="91066-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="91066-140">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_roleAssignments"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments?$filter=principalId eq 'a98eb769-7bd4-4489-86f6-ad96e1d58b62'
```

#### <a name="response"></a><span data-ttu-id="91066-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="91066-141">Response</span></span>

<span data-ttu-id="91066-142">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="91066-142">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignment",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleAssignments",
    "value": [
        {
            "@odata.type": "#microsoft.graph.unifiedRoleAssignment",
            "id": "lAPpYvVpN0KRkAEhdxReEGm3jqnUe4lEhvatluHVi2I-1",
            "roleDefinitionId": "62e90394-69f5-4237-9190-012177145e10",
            "principalId": "a98eb769-7bd4-4489-86f6-ad96e1d58b62",
            "directoryScopeId": "/"            
        },
        {
            "@odata.type": "#microsoft.graph.unifiedRoleAssignment",
            "id": "uBph6InB6EaU4WAhOrH4FGm3jqnUe4lEhvatluHVi2I-1",
            "roleDefinitionId": "e8611ab8-c189-46e8-94e1-60213ab1f814",
            "principalId": "a98eb769-7bd4-4489-86f6-ad96e1d58b62",
            "directoryScopeId": "/"            
        },
        {
            "@odata.type": "#microsoft.graph.unifiedRoleAssignment",
            "id": "5wuT_mJe20eRr5jDpJo4sWm3jqnUe4lEhvatluHVi2I-1",
            "roleDefinitionId": "fe930be7-5e62-47db-91af-98c3a49a38b1",
            "principalId": "a98eb769-7bd4-4489-86f6-ad96e1d58b62",
            "directoryScopeId": "/"            
        },
        {
            "@odata.type": "#microsoft.graph.unifiedRoleAssignment",
            "id": "5TgczyE2BECny4eWJNztfGm3jqnUe4lEhvatluHVi2I-1",
            "roleDefinitionId": "cf1c38e5-3621-4004-a7cb-879624dced7c",
            "principalId": "a98eb769-7bd4-4489-86f6-ad96e1d58b62",
            "directoryScopeId": "/"            
        },
        {
            "@odata.type": "#microsoft.graph.unifiedRoleAssignment",
            "id": "CRCUdVqRaUir52kb_xgnnmm3jqnUe4lEhvatluHVi2I-1",
            "roleDefinitionId": "75941009-915a-4869-abe7-691bff18279e",
            "principalId": "a98eb769-7bd4-4489-86f6-ad96e1d58b62",
            "directoryScopeId": "/"            
        },
        {
            "@odata.type": "#microsoft.graph.unifiedRoleAssignment",
            "id": "4yeYchSc90m7G5YI8Va7uGm3jqnUe4lEhvatluHVi2I-1",
            "roleDefinitionId": "729827e3-9c14-49f7-bb1b-9608f156bbb8",
            "principalId": "a98eb769-7bd4-4489-86f6-ad96e1d58b62",
            "directoryScopeId": "/"            
        },
        {
            "@odata.type": "#microsoft.graph.unifiedRoleAssignment",
            "id": "y-RKGSaxskC9W2CRs4CXfWm3jqnUe4lEhvatluHVi2I-1",
            "roleDefinitionId": "194ae4cb-b126-40b2-bd5b-6091b380977d",
            "principalId": "a98eb769-7bd4-4489-86f6-ad96e1d58b62",
            "directoryScopeId": "/"
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List roleAssignments",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->