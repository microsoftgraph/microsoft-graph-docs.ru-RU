---
title: Перечисление group transitive memberOf
description: Получите группы, в которые входит группа.  Эта операция является транзитной и также будет включать все группы, вложенные в эту группу. В отличие от получения пользовательских Microsoft 365, это возвращает все типы групп, а не только Microsoft 365 групп.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 448303bdc4cf158a41d376f4a2f2f0b69cad9a56
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052301"
---
# <a name="list-group-transitive-memberof"></a><span data-ttu-id="ef696-105">Перечисление group transitive memberOf</span><span class="sxs-lookup"><span data-stu-id="ef696-105">List group transitive memberOf</span></span>

<span data-ttu-id="ef696-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ef696-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ef696-107">Получите группы, в которые входит группа.</span><span class="sxs-lookup"><span data-stu-id="ef696-107">Get groups that the group is a member of.</span></span>  <span data-ttu-id="ef696-108">Эта операция является транзитной и также будет включать все группы, вложенные в эту группу.</span><span class="sxs-lookup"><span data-stu-id="ef696-108">This operation is transitive and will also include all groups that this groups is a nested member of.</span></span> <span data-ttu-id="ef696-109">В отличие от получения пользовательских Microsoft 365, это возвращает все типы групп, а не только Microsoft 365 групп.</span><span class="sxs-lookup"><span data-stu-id="ef696-109">Unlike getting a user's Microsoft 365 groups, this returns all types of groups, not just Microsoft 365 groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="ef696-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ef696-110">Permissions</span></span>

<span data-ttu-id="ef696-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef696-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef696-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ef696-113">Permission type</span></span>      | <span data-ttu-id="ef696-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ef696-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ef696-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ef696-115">Delegated (work or school account)</span></span> | <span data-ttu-id="ef696-116">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ef696-116">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ef696-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ef696-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ef696-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef696-118">Not supported.</span></span>    |
|<span data-ttu-id="ef696-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ef696-119">Application</span></span> | <span data-ttu-id="ef696-120">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef696-120">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="ef696-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ef696-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ef696-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ef696-122">Optional query parameters</span></span>

<span data-ttu-id="ef696-123">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа, в том числе `$search`, `$count` і `$filter`.</span><span class="sxs-lookup"><span data-stu-id="ef696-123">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="ef696-124">Также включено литье OData, например, для получения только транзитных участников группы.</span><span class="sxs-lookup"><span data-stu-id="ef696-124">OData cast is also enabled, for example, you can cast to get just the transitive group members of a group.</span></span> <span data-ttu-id="ef696-125">Вы можете использовать `$search` в свойствах **displayName** и **description**.</span><span class="sxs-lookup"><span data-stu-id="ef696-125">You can use `$search` on the **displayName** and **description** properties.</span></span> <span data-ttu-id="ef696-126">Когда элементы добавляются или обновляются для этого ресурса, они специально индексируются для использования с помощью параметров `$count` и `$search`.</span><span class="sxs-lookup"><span data-stu-id="ef696-126">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="ef696-127">Между добавлением или обновлением элемента и его появлением в индексе может возникать небольшая задержка.</span><span class="sxs-lookup"><span data-stu-id="ef696-127">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ef696-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ef696-128">Request headers</span></span>

| <span data-ttu-id="ef696-129">Имя</span><span class="sxs-lookup"><span data-stu-id="ef696-129">Name</span></span> | <span data-ttu-id="ef696-130">Описание</span><span class="sxs-lookup"><span data-stu-id="ef696-130">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="ef696-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ef696-131">Authorization</span></span>  | <span data-ttu-id="ef696-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ef696-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ef696-134">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="ef696-134">ConsistencyLevel</span></span> | <span data-ttu-id="ef696-135">необязательный.</span><span class="sxs-lookup"><span data-stu-id="ef696-135">eventual.</span></span> <span data-ttu-id="ef696-136">Этот заголовок и `$count` требуются при использовании `$search`, `$filter`, `$orderby` или с параметрами запросов OData cast.</span><span class="sxs-lookup"><span data-stu-id="ef696-136">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="ef696-137">В нем используется индекс, который может не соответствовать последним изменениям объекта.</span><span class="sxs-lookup"><span data-stu-id="ef696-137">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ef696-138">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ef696-138">Request body</span></span>
<span data-ttu-id="ef696-139">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ef696-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ef696-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="ef696-140">Response</span></span>
<span data-ttu-id="ef696-141">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ef696-141">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ef696-142">Примеры</span><span class="sxs-lookup"><span data-stu-id="ef696-142">Examples</span></span>

### <a name="example-1-get-groups-and-administrative-units-that-the-group-is-a-transitive-member-of"></a><span data-ttu-id="ef696-143">Пример 1. Получить группы и административные единицы, которые группа является транзитным членом</span><span class="sxs-lookup"><span data-stu-id="ef696-143">Example 1: Get groups and administrative units that the group is a transitive member of</span></span>

#### <a name="request"></a><span data-ttu-id="ef696-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="ef696-144">Request</span></span>

<span data-ttu-id="ef696-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ef696-145">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ef696-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="ef696-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_transitivememberof"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/transitiveMemberOf
```
# <a name="c"></a>[<span data-ttu-id="ef696-147">C#</span><span class="sxs-lookup"><span data-stu-id="ef696-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-transitivememberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ef696-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ef696-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-transitivememberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ef696-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ef696-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-transitivememberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ef696-150">Java</span><span class="sxs-lookup"><span data-stu-id="ef696-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-transitivememberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="ef696-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="ef696-151">Response</span></span>

<span data-ttu-id="ef696-152">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ef696-152">The following is an example of the response.</span></span>

><span data-ttu-id="ef696-153">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ef696-153">**Note:** The response object shown here might be shortened for readability.</span></span>

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
      "@odata.type": "#microsoft.graph.group",
      "id": "11111111-2222-3333-4444-555555555555",
      "mail": "group1@contoso.com"
    }
  ]
}
```

### <a name="example-2-get-only-a-count-of-all-transitive-membership"></a><span data-ttu-id="ef696-154">Пример 2: Получение только количества транзитивных участников</span><span class="sxs-lookup"><span data-stu-id="ef696-154">Example 2: Get only a count of all transitive membership</span></span>

#### <a name="request"></a><span data-ttu-id="ef696-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="ef696-155">Request</span></span>

<span data-ttu-id="ef696-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ef696-156">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/transitiveMemberOf/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="ef696-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="ef696-157">Response</span></span>

<span data-ttu-id="ef696-158">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ef696-158">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

`294`

### <a name="example-3-use-odata-cast-to-get-only-a-count-of-transitive-membership-in-groups"></a><span data-ttu-id="ef696-159">Пример 3. Использование OData cast для получения только количества транзитивных участников в группах</span><span class="sxs-lookup"><span data-stu-id="ef696-159">Example 3: Use OData cast to get only a count of transitive membership in groups</span></span>

#### <a name="request"></a><span data-ttu-id="ef696-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="ef696-160">Request</span></span>

<span data-ttu-id="ef696-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ef696-161">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/transitiveMemberOf/microsoft.graph.group/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="ef696-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="ef696-162">Response</span></span>

<span data-ttu-id="ef696-163">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ef696-163">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

`294`

### <a name="example-4-use-odata-cast-and-search-to-get-membership-in-groups-with-display-names-that-contain-the-letters-tier-including-a-count-of-returned-objects"></a><span data-ttu-id="ef696-164">Пример 4. Использование литых и $search OData для получения членства в группах с отображаемой именами, которые содержат буквы "tier", включая количество возвращенных объектов</span><span class="sxs-lookup"><span data-stu-id="ef696-164">Example 4: Use OData cast and $search to get membership in groups with display names that contain the letters 'tier' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="ef696-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="ef696-165">Request</span></span>

<span data-ttu-id="ef696-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ef696-166">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_tier_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderby=displayName&$search="displayName:tier"&$select=displayName,id
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="ef696-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="ef696-167">Response</span></span>

<span data-ttu-id="ef696-168">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ef696-168">The following is an example of the response.</span></span>

><span data-ttu-id="ef696-169">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ef696-169">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups(displayName,id)",
  "@odata.count":7,
  "value":[
    {
      "displayName":"Contoso-tier Query Notification",
      "id":"11111111-2222-3333-4444-555555555555"
    }
  ]
}
```

### <a name="example-5-use-odata-cast-and-filter-to-get-membership-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="ef696-170">Пример 5. Использование литых и $filter OData для получения членства с именем отображения, которое начинается с "A", включая количество возвращенных объектов</span><span class="sxs-lookup"><span data-stu-id="ef696-170">Example 5: Use OData cast and $filter to get membership with a display name that starts with 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="ef696-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="ef696-171">Request</span></span>

<span data-ttu-id="ef696-172">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ef696-172">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderby=displayName&$filter=startswith(displayName, 'a')
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="ef696-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="ef696-173">Response</span></span>

<span data-ttu-id="ef696-174">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ef696-174">The following is an example of the response.</span></span>

><span data-ttu-id="ef696-175">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ef696-175">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
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
  "description": "List group transitive memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
