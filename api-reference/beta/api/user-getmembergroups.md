---
title: 'user: getMemberGroups'
description: 'Возвращает все группы, в которых состоит пользователь. Это промежуточная проверка, в отличие от считывания '
localization_priority: Normal
author: krbain
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: c2ab1bcd9dce8e933ed65d51dd9b0ce010bc1b90
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896471"
---
# <a name="user-getmembergroups"></a><span data-ttu-id="6c2bc-104">user: getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="6c2bc-104">user: getMemberGroups</span></span>

<span data-ttu-id="6c2bc-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6c2bc-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6c2bc-106">Return all the groups that the user is a member of.</span><span class="sxs-lookup"><span data-stu-id="6c2bc-106">Return all the groups that the user is a member of.</span></span> <span data-ttu-id="6c2bc-107">The check is transitive, unlike reading the [memberOf](../api/user-list-memberof.md) navigation property, which returns only the groups that the user is a direct member of.</span><span class="sxs-lookup"><span data-stu-id="6c2bc-107">The check is transitive, unlike reading the [memberOf](../api/user-list-memberof.md) navigation property, which returns only the groups that the user is a direct member of.</span></span>

<span data-ttu-id="6c2bc-108">This function supports Microsoft 365 and other types of groups provisioned in Azure AD.</span><span class="sxs-lookup"><span data-stu-id="6c2bc-108">This function supports Microsoft 365 and other types of groups provisioned in Azure AD.</span></span> <span data-ttu-id="6c2bc-109">The maximum number of groups each request can return is 2046.</span><span class="sxs-lookup"><span data-stu-id="6c2bc-109">The maximum number of groups each request can return is 2046.</span></span> <span data-ttu-id="6c2bc-110">Note that Microsoft 365 groups cannot contain groups.</span><span class="sxs-lookup"><span data-stu-id="6c2bc-110">Note that Microsoft 365 groups cannot contain groups.</span></span> <span data-ttu-id="6c2bc-111">So membership in a Microsoft 365 group is always direct.</span><span class="sxs-lookup"><span data-stu-id="6c2bc-111">So membership in a Microsoft 365 group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="6c2bc-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6c2bc-112">Permissions</span></span>

<span data-ttu-id="6c2bc-113">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="6c2bc-113">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="6c2bc-114">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c2bc-114">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6c2bc-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6c2bc-115">Permission type</span></span>                        | <span data-ttu-id="6c2bc-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6c2bc-116">Permissions (from least to most privileged)</span></span>                                                                                                          |
| :------------------------------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="6c2bc-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6c2bc-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="6c2bc-118">User. ReadBasic. ALL и Граупмембер. Read. ALL, User. Read и Граупмембер. Read. ALL, User. Read. ALL и Граупмембер. Read. ALL, User. ReadBasic. ALL и Group. Read. ALL, User. Read. ALL и Group. Read. ALL, Directory. Read. ALL, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="6c2bc-118">User.ReadBasic.All and GroupMember.Read.All, User.Read and GroupMember.Read.All, User.Read.All and GroupMember.Read.All, User.ReadBasic.All and Group.Read.All, User.Read and Group.Read.All, User.Read.All and Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="6c2bc-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6c2bc-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6c2bc-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6c2bc-120">Not supported.</span></span>                                                                                                                                       |
| <span data-ttu-id="6c2bc-121">Для приложения</span><span class="sxs-lookup"><span data-stu-id="6c2bc-121">Application</span></span>                            | <span data-ttu-id="6c2bc-122">User.Read.All и GroupMember.Read.All, User.Read.All и Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c2bc-122">User.Read.All and GroupMember.Read.All, User.Read.All and Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span>            |

## <a name="http-request"></a><span data-ttu-id="6c2bc-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6c2bc-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /users/{id | userPrincipalName}/getMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="6c2bc-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6c2bc-124">Request headers</span></span>

| <span data-ttu-id="6c2bc-125">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6c2bc-125">Header</span></span>        | <span data-ttu-id="6c2bc-126">Значение</span><span class="sxs-lookup"><span data-stu-id="6c2bc-126">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="6c2bc-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6c2bc-127">Authorization</span></span> | <span data-ttu-id="6c2bc-128">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="6c2bc-128">Bearer {token}.</span></span> <span data-ttu-id="6c2bc-129">Required.</span><span class="sxs-lookup"><span data-stu-id="6c2bc-129">Required.</span></span> |
| <span data-ttu-id="6c2bc-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6c2bc-130">Content-Type</span></span>  | <span data-ttu-id="6c2bc-131">application/json</span><span class="sxs-lookup"><span data-stu-id="6c2bc-131">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="6c2bc-132">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6c2bc-132">Request body</span></span>

<span data-ttu-id="6c2bc-133">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="6c2bc-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6c2bc-134">Параметр</span><span class="sxs-lookup"><span data-stu-id="6c2bc-134">Parameter</span></span>           | <span data-ttu-id="6c2bc-135">Тип</span><span class="sxs-lookup"><span data-stu-id="6c2bc-135">Type</span></span>    | <span data-ttu-id="6c2bc-136">Описание</span><span class="sxs-lookup"><span data-stu-id="6c2bc-136">Description</span></span>                                                                                                                                                                                                                                                                         |
| :------------------ | :------ | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="6c2bc-137">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="6c2bc-137">securityEnabledOnly</span></span> | <span data-ttu-id="6c2bc-138">Логическое</span><span class="sxs-lookup"><span data-stu-id="6c2bc-138">Boolean</span></span> | <span data-ttu-id="6c2bc-139">**true** to specify that only security groups that the user is a member of should be returned; **false** to specify that all groups that the user is a member of should be returned.</span><span class="sxs-lookup"><span data-stu-id="6c2bc-139">**true** to specify that only security groups that the user is a member of should be returned; **false** to specify that all groups that the user is a member of should be returned.</span></span> <span data-ttu-id="6c2bc-140">Note: Setting this parameter to **true** is only supported when calling this method on a user.</span><span class="sxs-lookup"><span data-stu-id="6c2bc-140">Note: Setting this parameter to **true** is only supported when calling this method on a user.</span></span> |

## <a name="response"></a><span data-ttu-id="6c2bc-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="6c2bc-141">Response</span></span>

<span data-ttu-id="6c2bc-142">В случае успеха этот метод возвратит код отклика `200 OK` и коллекцию String в теле отклика, которое содержит идентификаторы групп, в которых состоит пользователь.</span><span class="sxs-lookup"><span data-stu-id="6c2bc-142">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the user is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="6c2bc-143">Пример</span><span class="sxs-lookup"><span data-stu-id="6c2bc-143">Example</span></span>

<span data-ttu-id="6c2bc-144">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="6c2bc-144">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="6c2bc-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="6c2bc-145">Request</span></span>

<span data-ttu-id="6c2bc-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6c2bc-146">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="6c2bc-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="6c2bc-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_getmembergroups"
}-->

```http
POST https://graph.microsoft.com/beta/me/getMemberGroups
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": true
}
```
# <a name="c"></a>[<span data-ttu-id="6c2bc-148">C#</span><span class="sxs-lookup"><span data-stu-id="6c2bc-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-getmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6c2bc-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6c2bc-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-getmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6c2bc-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6c2bc-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-getmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="6c2bc-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="6c2bc-151">Response</span></span>

<span data-ttu-id="6c2bc-152">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="6c2bc-152">Here is an example of the response.</span></span> <span data-ttu-id="6c2bc-153">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="6c2bc-153">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="6c2bc-154">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="6c2bc-154">All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 39

{
  "value": [
    "string-value"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!--
{
  "type": "#page.annotation",
  "description": "user: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
