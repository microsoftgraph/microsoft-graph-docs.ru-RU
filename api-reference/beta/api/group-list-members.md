---
title: Перечисление участников группы
description: Получение списка непосредственных участников группы.
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: c12cb905ff49b2997c123aa881f2d6281c2591f3
ms.sourcegitcommit: eafb1629e52450dab0da6a1fb6d1ddfa878777c6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2020
ms.locfileid: "49082064"
---
# <a name="list-group-members"></a><span data-ttu-id="92b8a-103">Перечисление участников группы</span><span class="sxs-lookup"><span data-stu-id="92b8a-103">List group members</span></span>

<span data-ttu-id="92b8a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="92b8a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="92b8a-105">Получение списка непосредственных участников группы.</span><span class="sxs-lookup"><span data-stu-id="92b8a-105">Get a list of the group's direct members.</span></span> <span data-ttu-id="92b8a-106">У группы могут быть пользователи, контакты, устройства, субъекты служб и другие группы в качестве участников.</span><span class="sxs-lookup"><span data-stu-id="92b8a-106">A group can have users, contacts, devices, service principals, and other groups as members.</span></span> <span data-ttu-id="92b8a-107">Эта операция не является транзитивной.</span><span class="sxs-lookup"><span data-stu-id="92b8a-107">This operation is not transitive.</span></span>

<span data-ttu-id="92b8a-108">Если группа содержит более 100 участников, Microsoft Graph возвращает в отклике свойство `@odata.nextLink`, содержащее URL-адрес следующей страницы результатов.</span><span class="sxs-lookup"><span data-stu-id="92b8a-108">When a group contains more than 100 members, Microsoft Graph returns a `@odata.nextLink` property in the response that contains a URL to the next page of results.</span></span> <span data-ttu-id="92b8a-109">При наличии этого свойства продолжайте выполнять дополнительные запросы с URL-адресом `@odata.nextLink` в каждом отклике, пока не будут возвращены все результаты, как описано в статье [Разбиение данных Microsoft Graph по страницам в приложении](/graph/paging).</span><span class="sxs-lookup"><span data-stu-id="92b8a-109">If that property is present, continue making additional requests with the `@odata.nextLink` URL in each response, until all the results are returned, as described in [paging Microsoft Graph data in your app](/graph/paging).</span></span>

## <a name="permissions"></a><span data-ttu-id="92b8a-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="92b8a-110">Permissions</span></span>

<span data-ttu-id="92b8a-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92b8a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="92b8a-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="92b8a-113">Permission type</span></span> | <span data-ttu-id="92b8a-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="92b8a-114">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="92b8a-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="92b8a-115">Delegated (work or school account)</span></span> | <span data-ttu-id="92b8a-116">Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="92b8a-116">Group.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="92b8a-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="92b8a-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="92b8a-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="92b8a-118">Not supported.</span></span> |
| <span data-ttu-id="92b8a-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="92b8a-119">Application</span></span> | <span data-ttu-id="92b8a-120">Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="92b8a-120">Group.Read.All, Directory.Read.All</span></span> |

> <span data-ttu-id="92b8a-121">**Примечание:** Чтобы получить список членов скрытой группы членства, требуется разрешение Member. Read. Hidden.</span><span class="sxs-lookup"><span data-stu-id="92b8a-121">**Note:** To list the members of a hidden membership group, the Member.Read.Hidden permission is required.</span></span>

[!INCLUDE [limited-info](../../includes/limited-info.md)]
 
## <a name="http-request"></a><span data-ttu-id="92b8a-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="92b8a-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="92b8a-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="92b8a-123">Optional query parameters</span></span>

<span data-ttu-id="92b8a-124">Этот метод поддерживает [параметры запросов OData](/graph/query_parameters) для настройки ответа, в том числе `$search`, `$count` і `$filter`.</span><span class="sxs-lookup"><span data-stu-id="92b8a-124">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="92b8a-125">Кроме того, включено приведение к OData, например, вы можете получить только пользователей, которые являются участниками группы.</span><span class="sxs-lookup"><span data-stu-id="92b8a-125">OData cast is also enabled, for example, you can cast to get just the users that are a member of the group.</span></span> <span data-ttu-id="92b8a-126">`$search` можно использовать в свойстве **displayName**.</span><span class="sxs-lookup"><span data-stu-id="92b8a-126">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="92b8a-127">Когда элементы добавляются или обновляются для этого ресурса, они специально индексируются для использования с помощью параметров `$count` и `$search`.</span><span class="sxs-lookup"><span data-stu-id="92b8a-127">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="92b8a-128">Между добавлением или обновлением элемента и его появлением в индексе может возникать небольшая задержка.</span><span class="sxs-lookup"><span data-stu-id="92b8a-128">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="92b8a-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="92b8a-129">Request headers</span></span>

| <span data-ttu-id="92b8a-130">Имя</span><span class="sxs-lookup"><span data-stu-id="92b8a-130">Name</span></span> | <span data-ttu-id="92b8a-131">Описание</span><span class="sxs-lookup"><span data-stu-id="92b8a-131">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="92b8a-132">Авторизация</span><span class="sxs-lookup"><span data-stu-id="92b8a-132">Authorization</span></span> | <span data-ttu-id="92b8a-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="92b8a-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="92b8a-135">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="92b8a-135">ConsistencyLevel</span></span> | <span data-ttu-id="92b8a-136">необязательный.</span><span class="sxs-lookup"><span data-stu-id="92b8a-136">eventual.</span></span> <span data-ttu-id="92b8a-137">Этот заголовок и `$count` требуются при использовании `$search`, `$filter`, `$orderby` или с параметрами запросов OData cast.</span><span class="sxs-lookup"><span data-stu-id="92b8a-137">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="92b8a-138">В нем используется индекс, который может не соответствовать последним изменениям объекта.</span><span class="sxs-lookup"><span data-stu-id="92b8a-138">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="92b8a-139">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="92b8a-139">Request body</span></span>

<span data-ttu-id="92b8a-140">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="92b8a-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="92b8a-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="92b8a-141">Response</span></span>

<span data-ttu-id="92b8a-142">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="92b8a-142">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="92b8a-143">Примеры</span><span class="sxs-lookup"><span data-stu-id="92b8a-143">Examples</span></span>

### <a name="example-1-get-the-direct-membership-in-a-group"></a><span data-ttu-id="92b8a-144">Пример 1. Получение сведений о непосредственном участии в группе</span><span class="sxs-lookup"><span data-stu-id="92b8a-144">Example 1: Get the direct membership in a group</span></span>

#### <a name="request"></a><span data-ttu-id="92b8a-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="92b8a-145">Request</span></span>

<span data-ttu-id="92b8a-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="92b8a-146">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="92b8a-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="92b8a-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_members"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/members
```
# <a name="c"></a>[<span data-ttu-id="92b8a-148">C#</span><span class="sxs-lookup"><span data-stu-id="92b8a-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-members-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="92b8a-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="92b8a-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-members-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="92b8a-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="92b8a-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-members-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="92b8a-151">Java</span><span class="sxs-lookup"><span data-stu-id="92b8a-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-members-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="92b8a-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="92b8a-152">Response</span></span>

<span data-ttu-id="92b8a-153">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="92b8a-153">The following is an example of the response.</span></span>
><span data-ttu-id="92b8a-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="92b8a-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-only-a-count-of-all-membership"></a><span data-ttu-id="92b8a-156">Пример 2. Получение только количества всех участий</span><span class="sxs-lookup"><span data-stu-id="92b8a-156">Example 2: Get only a count of all membership</span></span>

#### <a name="request"></a><span data-ttu-id="92b8a-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="92b8a-157">Request</span></span>

<span data-ttu-id="92b8a-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="92b8a-158">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/members/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="92b8a-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="92b8a-159">Response</span></span>

<span data-ttu-id="92b8a-160">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="92b8a-160">The following is an example of the response.</span></span>

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

<span data-ttu-id="92b8a-161">893</span><span class="sxs-lookup"><span data-stu-id="92b8a-161">893</span></span>

### <a name="example-3-use-odata-cast-to-get-only-a-count-of-user-membership"></a><span data-ttu-id="92b8a-162">Пример 3. Использование приведения к OData для получения только количества участий пользователей</span><span class="sxs-lookup"><span data-stu-id="92b8a-162">Example 3: Use OData cast to get only a count of user membership</span></span>

#### <a name="request"></a><span data-ttu-id="92b8a-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="92b8a-163">Request</span></span>

<span data-ttu-id="92b8a-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="92b8a-164">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_user_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/members/microsoft.graph.user/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="92b8a-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="92b8a-165">Response</span></span>

<span data-ttu-id="92b8a-166">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="92b8a-166">The following is an example of the response.</span></span>

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

<span data-ttu-id="92b8a-167">893</span><span class="sxs-lookup"><span data-stu-id="92b8a-167">893</span></span>

### <a name="example-4-use-search-and-odata-cast-to-get-user-membership-in-groups-with-display-names-that-contain-the-letters-pr-including-a-count-of-returned-objects"></a><span data-ttu-id="92b8a-168">Пример 4: используйте $search и приведение OData для получения членства пользователя в группах с отображаемыми именами, содержащими буквы "PR", включая число возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="92b8a-168">Example 4: Use $search and OData cast to get user membership in groups with display names that contain the letters 'Pr' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="92b8a-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="92b8a-169">Request</span></span>

<span data-ttu-id="92b8a-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="92b8a-170">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_pr_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/members/microsoft.graph.user?$count=true&$orderby=displayName&$search="displayName:Pr"&$select=displayName,id
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="92b8a-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="92b8a-171">Response</span></span>

<span data-ttu-id="92b8a-172">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="92b8a-172">The following is an example of the response.</span></span>
><span data-ttu-id="92b8a-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="92b8a-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-5-use-filter-to-get-group-membership-with-a-display-name-that-starts-with-the-letter-a-including-a-count-of-returned-objects"></a><span data-ttu-id="92b8a-175">Пример 5. Использование параметра $filter для получения участия в группах с отображаемым именем, которое начинается на "А", включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="92b8a-175">Example 5: Use $filter to get group membership with a display name that starts with the letter 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="92b8a-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="92b8a-176">Request</span></span>

<span data-ttu-id="92b8a-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="92b8a-177">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/members?$count=true&$filter=startswith(displayName, 'a')
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="92b8a-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="92b8a-178">Response</span></span>

<span data-ttu-id="92b8a-179">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="92b8a-179">The following is an example of the response.</span></span>
><span data-ttu-id="92b8a-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="92b8a-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


