---
title: Список членов группы
description: Получение списка непосредственных участников группы.
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 1aecbc2fe5c9f73902c3b247c499741468c163db
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2020
ms.locfileid: "44289625"
---
# <a name="list-group-members"></a><span data-ttu-id="b78a9-103">Список членов группы</span><span class="sxs-lookup"><span data-stu-id="b78a9-103">List group members</span></span>

<span data-ttu-id="b78a9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b78a9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b78a9-105">Получение списка непосредственных участников группы.</span><span class="sxs-lookup"><span data-stu-id="b78a9-105">Get a list of the group's direct members.</span></span> <span data-ttu-id="b78a9-106">У группы могут быть пользователи, контакты, устройства, субъекты служб и другие группы в качестве участников.</span><span class="sxs-lookup"><span data-stu-id="b78a9-106">A group can have users, contacts, devices, service principals, and other groups as members.</span></span> <span data-ttu-id="b78a9-107">Эта операция не является транзитивной.</span><span class="sxs-lookup"><span data-stu-id="b78a9-107">This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="b78a9-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b78a9-108">Permissions</span></span>

<span data-ttu-id="b78a9-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b78a9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b78a9-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b78a9-111">Permission type</span></span> | <span data-ttu-id="b78a9-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b78a9-112">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="b78a9-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b78a9-113">Delegated (work or school account)</span></span> | <span data-ttu-id="b78a9-114">User.ReadBasic.All, User.Read.All, Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="b78a9-114">User.ReadBasic.All, User.Read.All, Group.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="b78a9-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b78a9-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b78a9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b78a9-116">Not supported.</span></span> |
| <span data-ttu-id="b78a9-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b78a9-117">Application</span></span> | <span data-ttu-id="b78a9-118">Group. Read. ALL, User. Read. ALL, Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="b78a9-118">Group.Read.All, User.Read.All, Directory.Read.All</span></span> |

> <span data-ttu-id="b78a9-119">**Примечание:** Чтобы получить список членов скрытой группы членства, требуется разрешение Member. Read. Hidden.</span><span class="sxs-lookup"><span data-stu-id="b78a9-119">**Note:** To list the members of a hidden membership group, the Member.Read.Hidden permission is required.</span></span>

[!INCLUDE [limited-info](../../includes/limited-info.md)]
 
## <a name="http-request"></a><span data-ttu-id="b78a9-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b78a9-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b78a9-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b78a9-121">Optional query parameters</span></span>

<span data-ttu-id="b78a9-122">Этот метод поддерживает [параметры запросов OData](/graph/query_parameters) для настройки ответа, включая `$search` , `$count` и `$filter` .</span><span class="sxs-lookup"><span data-stu-id="b78a9-122">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="b78a9-123">Приведение OData также включено, например, можно выполнить приведение, чтобы получить только тех пользователей, которые являются членами группы.</span><span class="sxs-lookup"><span data-stu-id="b78a9-123">OData cast is also enabled, for example, you can cast to get just the users that are a member of the group.</span></span> <span data-ttu-id="b78a9-124">Можно использовать `$search` свойство **DisplayName** .</span><span class="sxs-lookup"><span data-stu-id="b78a9-124">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="b78a9-125">При добавлении или обновлении элементов для этого ресурса они могут индексироваться для использования с `$count` `$search` параметрами запроса.</span><span class="sxs-lookup"><span data-stu-id="b78a9-125">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="b78a9-126">Между добавлением или обновлением элемента может быть небольшая задержка, а когда он доступен в индексе.</span><span class="sxs-lookup"><span data-stu-id="b78a9-126">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b78a9-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b78a9-127">Request headers</span></span>

| <span data-ttu-id="b78a9-128">Имя</span><span class="sxs-lookup"><span data-stu-id="b78a9-128">Name</span></span> | <span data-ttu-id="b78a9-129">Описание</span><span class="sxs-lookup"><span data-stu-id="b78a9-129">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="b78a9-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b78a9-130">Authorization</span></span> | <span data-ttu-id="b78a9-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b78a9-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b78a9-133">консистенцилевел</span><span class="sxs-lookup"><span data-stu-id="b78a9-133">ConsistencyLevel</span></span> | <span data-ttu-id="b78a9-134">закончить.</span><span class="sxs-lookup"><span data-stu-id="b78a9-134">eventual.</span></span> <span data-ttu-id="b78a9-135">Этот заголовок и `$count` при использовании `$search` `$filter` `$orderby` параметров запроса на приведение,, или OData.</span><span class="sxs-lookup"><span data-stu-id="b78a9-135">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="b78a9-136">Он использует индекс, который может не быть актуальным с последними изменениями объекта.</span><span class="sxs-lookup"><span data-stu-id="b78a9-136">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b78a9-137">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b78a9-137">Request body</span></span>

<span data-ttu-id="b78a9-138">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b78a9-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b78a9-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="b78a9-139">Response</span></span>

<span data-ttu-id="b78a9-140">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b78a9-140">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b78a9-141">Примеры</span><span class="sxs-lookup"><span data-stu-id="b78a9-141">Examples</span></span>

### <a name="example-1-get-the-direct-membership-in-a-group"></a><span data-ttu-id="b78a9-142">Пример 1: получение прямого членства в группе</span><span class="sxs-lookup"><span data-stu-id="b78a9-142">Example 1: Get the direct membership in a group</span></span>

#### <a name="request"></a><span data-ttu-id="b78a9-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="b78a9-143">Request</span></span>

<span data-ttu-id="b78a9-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b78a9-144">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b78a9-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="b78a9-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_members"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/members
```
# <a name="c"></a>[<span data-ttu-id="b78a9-146">C#</span><span class="sxs-lookup"><span data-stu-id="b78a9-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-members-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b78a9-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b78a9-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-members-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b78a9-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b78a9-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-members-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="b78a9-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="b78a9-149">Response</span></span>

<span data-ttu-id="b78a9-150">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b78a9-150">The following is an example of the response.</span></span>
><span data-ttu-id="b78a9-151">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b78a9-151">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b78a9-152">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b78a9-152">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "11111111-2222-3333-4444-555555555555",
      "mail": "group1@contoso.com",
      "mailEnabled": true,
      "mailNickname": "Contoso1",
      "securityEnabled": true
    }
  ]
}
```

### <a name="example-2-get-only-a-count-of-all-membership"></a><span data-ttu-id="b78a9-153">Пример 2: получение только количества всех участников</span><span class="sxs-lookup"><span data-stu-id="b78a9-153">Example 2: Get only a count of all membership</span></span>

#### <a name="request"></a><span data-ttu-id="b78a9-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="b78a9-154">Request</span></span>

<span data-ttu-id="b78a9-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b78a9-155">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/members/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="b78a9-156">Ответ</span><span class="sxs-lookup"><span data-stu-id="b78a9-156">Response</span></span>

<span data-ttu-id="b78a9-157">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b78a9-157">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

<span data-ttu-id="b78a9-158">893</span><span class="sxs-lookup"><span data-stu-id="b78a9-158">893</span></span>

### <a name="example-3-use-odata-cast-to-get-only-a-count-of-user-membership"></a><span data-ttu-id="b78a9-159">Пример 3: Использование приведения OData для получения только количества членства пользователя</span><span class="sxs-lookup"><span data-stu-id="b78a9-159">Example 3: Use OData cast to get only a count of user membership</span></span>

#### <a name="request"></a><span data-ttu-id="b78a9-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="b78a9-160">Request</span></span>

<span data-ttu-id="b78a9-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b78a9-161">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_count_user_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/members/microsoft.graph.user/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="b78a9-162">Ответ</span><span class="sxs-lookup"><span data-stu-id="b78a9-162">Response</span></span>

<span data-ttu-id="b78a9-163">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b78a9-163">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

<span data-ttu-id="b78a9-164">893</span><span class="sxs-lookup"><span data-stu-id="b78a9-164">893</span></span>

### <a name="example-4-use-searchand-odata-cast-to-get-user-membership-in-groups-with-display-names-that-contain-the-letters-pr-including-a-count-of-returned-objects"></a><span data-ttu-id="b78a9-165">Пример 4: использование $searchandной приведение OData для получения членства пользователя в группах с отображаемыми именами, содержащими буквы "PR", включая число возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="b78a9-165">Example 4: Use $searchand OData cast to get user membership in groups with display names that contain the letters 'Pr' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="b78a9-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="b78a9-166">Request</span></span>

<span data-ttu-id="b78a9-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b78a9-167">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_pr_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/members/microsoft.graph.user?$count=true&$orderby=displayName&$search="displayName:Pr"&$select=displayName,id
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="b78a9-168">Ответ</span><span class="sxs-lookup"><span data-stu-id="b78a9-168">Response</span></span>

<span data-ttu-id="b78a9-169">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b78a9-169">The following is an example of the response.</span></span>
><span data-ttu-id="b78a9-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b78a9-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users(displayName,id)",
  "@odata.count":7,
  "value":[
    {
      "displayName":"Joseph Price",
      "id":"11111111-2222-3333-4444-555555555555"
    },
    {
      "displayName":"Preston Morales",
      "id":"11111111-2222-3333-4444-555555555555"
    }
  ]
}
```

### <a name="example-5-use-filter-to-get-group-membership-with-a-display-name-that-starts-with-the-letter-a-including-a-count-of-returned-objects"></a><span data-ttu-id="b78a9-172">Пример 5: использование $filter для получения сведений о членстве в группах с отображаемым именем, начинающимся с буквы "A", в том числе числа возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="b78a9-172">Example 5: Use $filter to get group membership with a display name that starts with the letter 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="b78a9-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="b78a9-173">Request</span></span>

<span data-ttu-id="b78a9-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b78a9-174">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/members?$count=true&$filter=startswith(displayName, 'a')
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="b78a9-175">Ответ</span><span class="sxs-lookup"><span data-stu-id="b78a9-175">Response</span></span>

<span data-ttu-id="b78a9-176">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b78a9-176">The following is an example of the response.</span></span>
><span data-ttu-id="b78a9-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b78a9-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups",
  "@odata.count":76,
  "value":[
    {
      "displayName":"AAD Contoso Users",
      "mail":"AADContoso_Users@contoso.com",
      "mailEnabled":true,
      "mailNickname":"AADContoso_Users",
      "securityEnabled":true
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List group members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
