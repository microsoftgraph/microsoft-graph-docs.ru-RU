---
title: Список участников
description: Получение списка непосредственных участников группы. Участниками групп могут быть пользователи, контакты организации, устройства, субъекты-службы и другие группы.
localization_priority: Priority
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 34b8a353455ee4392a984284f27adae562f34248
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048717"
---
# <a name="list-members"></a><span data-ttu-id="41d08-104">Список участников</span><span class="sxs-lookup"><span data-stu-id="41d08-104">List members</span></span>

<span data-ttu-id="41d08-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="41d08-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="41d08-106">Получение списка непосредственных участников группы.</span><span class="sxs-lookup"><span data-stu-id="41d08-106">Get a list of the group's direct members.</span></span> <span data-ttu-id="41d08-107">Участниками группы могут быть пользователи, контакты организации, устройства, субъекты-службы и другие группы.</span><span class="sxs-lookup"><span data-stu-id="41d08-107">A group can have users, organizational contacts, devices, service principals and other groups as members.</span></span> <span data-ttu-id="41d08-108">В настоящее время субъекты-службы не указаны как участники группы благодаря поэтапному развертыванию субъектов-служб в конечной точке Microsoft Graph версии 1.0.</span><span class="sxs-lookup"><span data-stu-id="41d08-108">Currently service principals are not listed as group members due to staged roll-out of service principals on Graph V1.0 endpoint.</span></span> <span data-ttu-id="41d08-109">Эта операция не является транзитивной.</span><span class="sxs-lookup"><span data-stu-id="41d08-109">This operation is not transitive.</span></span>

<span data-ttu-id="41d08-110">Если группа содержит более 100 участников, Microsoft Graph возвращает в отклике свойство `@odata.nextLink`, содержащее URL-адрес следующей страницы результатов.</span><span class="sxs-lookup"><span data-stu-id="41d08-110">When a group contains more than 100 members, Microsoft Graph returns a `@odata.nextLink` property in the response that contains a URL to the next page of results.</span></span> <span data-ttu-id="41d08-111">При наличии этого свойства продолжайте выполнять дополнительные запросы с URL-адресом `@odata.nextLink` в каждом отклике, пока не будут возвращены все результаты, как описано в статье [Разбиение данных Microsoft Graph по страницам в приложении](/graph/paging).</span><span class="sxs-lookup"><span data-stu-id="41d08-111">If that property is present, continue making additional requests with the `@odata.nextLink` URL in each response, until all the results are returned, as described in [paging Microsoft Graph data in your app](/graph/paging).</span></span>

## <a name="permissions"></a><span data-ttu-id="41d08-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="41d08-112">Permissions</span></span>
<span data-ttu-id="41d08-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41d08-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41d08-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="41d08-115">Permission type</span></span>      | <span data-ttu-id="41d08-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="41d08-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="41d08-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="41d08-117">Delegated (work or school account)</span></span> | <span data-ttu-id="41d08-118">GroupMember.Read.All, Group.Read.All, GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="41d08-118">GroupMember.Read.All, Group.Read.All, GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All</span></span>  |
|<span data-ttu-id="41d08-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="41d08-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="41d08-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="41d08-120">Not supported.</span></span>    |
|<span data-ttu-id="41d08-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="41d08-121">Application</span></span> | <span data-ttu-id="41d08-122">GroupMember.Read.All, Group.Read.All, GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="41d08-122">GroupMember.Read.All, Group.Read.All, GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="41d08-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="41d08-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="41d08-124">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="41d08-124">Optional query parameters</span></span>

<span data-ttu-id="41d08-125">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа, в том числе `$search`, `$count` і `$filter`.</span><span class="sxs-lookup"><span data-stu-id="41d08-125">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="41d08-126">Кроме того, включено приведение к OData, например, вы можете получить только пользователей, которые являются участниками группы.</span><span class="sxs-lookup"><span data-stu-id="41d08-126">OData cast is also enabled, for example, you can cast to get just the users that are a member of the group.</span></span> <span data-ttu-id="41d08-127">Вы можете использовать `$search` в свойствах **displayName** и **description**.</span><span class="sxs-lookup"><span data-stu-id="41d08-127">You can use `$search` on the **displayName** and **description** properties.</span></span> <span data-ttu-id="41d08-128">Когда элементы добавляются или обновляются для этого ресурса, они специально индексируются для использования с помощью параметров `$count` и `$search`.</span><span class="sxs-lookup"><span data-stu-id="41d08-128">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="41d08-129">Между добавлением или обновлением элемента и его появлением в индексе может возникать небольшая задержка.</span><span class="sxs-lookup"><span data-stu-id="41d08-129">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="41d08-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="41d08-130">Request headers</span></span>

| <span data-ttu-id="41d08-131">Заголовок</span><span class="sxs-lookup"><span data-stu-id="41d08-131">Header</span></span>       | <span data-ttu-id="41d08-132">Значение</span><span class="sxs-lookup"><span data-stu-id="41d08-132">Value</span></span> |
|:-----------|:----------|
| <span data-ttu-id="41d08-133">Авторизация</span><span class="sxs-lookup"><span data-stu-id="41d08-133">Authorization</span></span>  | <span data-ttu-id="41d08-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="41d08-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="41d08-136">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="41d08-136">ConsistencyLevel</span></span> | <span data-ttu-id="41d08-137">необязательный.</span><span class="sxs-lookup"><span data-stu-id="41d08-137">eventual.</span></span> <span data-ttu-id="41d08-138">Этот заголовок и `$count` требуются при использовании `$search`, `$filter`, `$orderby` или с параметрами запросов OData cast.</span><span class="sxs-lookup"><span data-stu-id="41d08-138">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="41d08-139">В нем используется индекс, который может не соответствовать последним изменениям объекта.</span><span class="sxs-lookup"><span data-stu-id="41d08-139">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="41d08-140">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="41d08-140">Request body</span></span>
<span data-ttu-id="41d08-141">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="41d08-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="41d08-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="41d08-142">Response</span></span>
<span data-ttu-id="41d08-143">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="41d08-143">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="41d08-144">Примеры</span><span class="sxs-lookup"><span data-stu-id="41d08-144">Examples</span></span>

### <a name="example-1-get-the-direct-membership-in-a-group"></a><span data-ttu-id="41d08-145">Пример 1. Получение сведений о непосредственном участии в группе</span><span class="sxs-lookup"><span data-stu-id="41d08-145">Example 1: Get the direct membership in a group</span></span>

#### <a name="request"></a><span data-ttu-id="41d08-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="41d08-146">Request</span></span>

<span data-ttu-id="41d08-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="41d08-147">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="41d08-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="41d08-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_members"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/members
```
# <a name="c"></a>[<span data-ttu-id="41d08-149">C#</span><span class="sxs-lookup"><span data-stu-id="41d08-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-members-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="41d08-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="41d08-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-members-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="41d08-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="41d08-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-members-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="41d08-152">Java</span><span class="sxs-lookup"><span data-stu-id="41d08-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-members-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="41d08-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="41d08-153">Response</span></span>

<span data-ttu-id="41d08-154">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="41d08-154">The following is an example of the response.</span></span>

><span data-ttu-id="41d08-155">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="41d08-155">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#directoryObjects",
  "value": [
    {
      "id": "11111111-2222-3333-4444-555555555555",
      "mail": "user1@contoso.com"
    }
  ]
}
```

### <a name="example-2-get-only-a-count-of-all-membership"></a><span data-ttu-id="41d08-156">Пример 2. Получение только количества всех участий</span><span class="sxs-lookup"><span data-stu-id="41d08-156">Example 2: Get only a count of all membership</span></span>

#### <a name="request"></a><span data-ttu-id="41d08-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="41d08-157">Request</span></span>

<span data-ttu-id="41d08-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="41d08-158">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/members/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="41d08-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="41d08-159">Response</span></span>

<span data-ttu-id="41d08-160">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="41d08-160">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

`893`


### <a name="example-3-use-odata-cast-to-get-only-a-count-of-user-membership"></a><span data-ttu-id="41d08-161">Пример 3. Использование приведения к OData для получения только количества участий пользователей</span><span class="sxs-lookup"><span data-stu-id="41d08-161">Example 3: Use OData cast to get only a count of user membership</span></span>

#### <a name="request"></a><span data-ttu-id="41d08-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="41d08-162">Request</span></span>

<span data-ttu-id="41d08-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="41d08-163">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_user_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/members/microsoft.graph.user/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="41d08-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="41d08-164">Response</span></span>

<span data-ttu-id="41d08-165">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="41d08-165">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

`893`

### <a name="example-4-use-searchand-odata-cast-to-get-user-membership-in-groups-with-display-names-that-contain-the-letters-pr-including-a-count-of-returned-objects"></a><span data-ttu-id="41d08-166">Пример 4. Использование приведения к OData и параметра $search для получения участия пользователей в группах с отображаемыми именами, содержащими буквы "Pr", включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="41d08-166">Example 4: Use $searchand OData cast to get user membership in groups with display names that contain the letters 'Pr' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="41d08-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="41d08-167">Request</span></span>

<span data-ttu-id="41d08-168">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="41d08-168">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_pr_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/members/microsoft.graph.user?$count=true&$orderby=displayName&$search="displayName:Pr"&$select=displayName,id
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="41d08-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="41d08-169">Response</span></span>

<span data-ttu-id="41d08-170">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="41d08-170">The following is an example of the response.</span></span>

><span data-ttu-id="41d08-171">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="41d08-171">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users(displayName,id)",
  "@odata.count":7,
  "value":[
    {
      "displayName":"Joseph Price",
      "id":"11111111-2222-3333-4444-555555555555"
    },
    {
      "displayName":"Preston Morales",
      "id":"66666666-7777-8888-9999-000000000000"
    }
  ]
}
```

### <a name="example-5-use-filter-to-get-group-membership-with-a-display-name-that-starts-with-the-letter-a-including-a-count-of-returned-objects"></a><span data-ttu-id="41d08-172">Пример 5. Использование параметра $filter для получения участия в группах с отображаемым именем, которое начинается на "А", включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="41d08-172">Example 5: Use $filter to get group membership with a display name that starts with the letter 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="41d08-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="41d08-173">Request</span></span>

<span data-ttu-id="41d08-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="41d08-174">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/members?$count=true&$filter=startswith(displayName, 'a')
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="41d08-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="41d08-175">Response</span></span>

<span data-ttu-id="41d08-176">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="41d08-176">The following is an example of the response.</span></span>

><span data-ttu-id="41d08-177">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="41d08-177">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#directoryObjects",
  "@odata.count":76,
  "value":[
    {
      "displayName":"AAD Contoso Users",
      "mail":"AADContoso_Users@contoso.com"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
