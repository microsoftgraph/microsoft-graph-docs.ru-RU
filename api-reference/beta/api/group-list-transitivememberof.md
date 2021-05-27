---
title: Перечисление group transitive memberOf
description: Получите группы и административные единицы, в которые входит группа.
localization_priority: Normal
author: Jordanndahl
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: f2a1daf44989034c02abb780d3d53cdce9c6a166
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52681489"
---
# <a name="list-group-transitive-memberof"></a><span data-ttu-id="13cf4-103">Перечисление group transitive memberOf</span><span class="sxs-lookup"><span data-stu-id="13cf4-103">List group transitive memberOf</span></span>

<span data-ttu-id="13cf4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="13cf4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="13cf4-105">Получите группы и административные единицы, в которые входит группа.</span><span class="sxs-lookup"><span data-stu-id="13cf4-105">Get groups and administrative units that the group is a member of.</span></span>  <span data-ttu-id="13cf4-106">Эта операция является транзитной и также будет включать все группы, вложенные в эту группу.</span><span class="sxs-lookup"><span data-stu-id="13cf4-106">This operation is transitive and will also include all groups that this groups is a nested member of.</span></span> <span data-ttu-id="13cf4-107">В отличие от получения пользовательских Microsoft 365, это возвращает все типы групп, а не только Microsoft 365 групп.</span><span class="sxs-lookup"><span data-stu-id="13cf4-107">Unlike getting a user's Microsoft 365 groups, this returns all types of groups, not just Microsoft 365 groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="13cf4-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="13cf4-108">Permissions</span></span>

<span data-ttu-id="13cf4-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="13cf4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="13cf4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="13cf4-111">Permission type</span></span> | <span data-ttu-id="13cf4-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="13cf4-112">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="13cf4-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="13cf4-113">Delegated (work or school account)</span></span> | <span data-ttu-id="13cf4-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="13cf4-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
| <span data-ttu-id="13cf4-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="13cf4-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="13cf4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="13cf4-116">Not supported.</span></span> |
| <span data-ttu-id="13cf4-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="13cf4-117">Application</span></span> | <span data-ttu-id="13cf4-118">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13cf4-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="13cf4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="13cf4-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="13cf4-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="13cf4-120">Optional query parameters</span></span>

<span data-ttu-id="13cf4-121">Этот метод поддерживает [параметры запросов OData](/graph/query_parameters) для настройки ответа, в том числе `$search`, `$count` і `$filter`.</span><span class="sxs-lookup"><span data-stu-id="13cf4-121">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="13cf4-122">Также включено литье OData, например, для получения только транзитных участников группы.</span><span class="sxs-lookup"><span data-stu-id="13cf4-122">OData cast is also enabled, for example, you can cast to get just the transitive group members of a group.</span></span> <span data-ttu-id="13cf4-123">`$search` можно использовать в свойстве **displayName**.</span><span class="sxs-lookup"><span data-stu-id="13cf4-123">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="13cf4-124">Когда элементы добавляются или обновляются для этого ресурса, они специально индексируются для использования с помощью параметров `$count` и `$search`.</span><span class="sxs-lookup"><span data-stu-id="13cf4-124">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="13cf4-125">Между добавлением или обновлением элемента и его появлением в индексе может возникать небольшая задержка.</span><span class="sxs-lookup"><span data-stu-id="13cf4-125">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="13cf4-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="13cf4-126">Request headers</span></span>

| <span data-ttu-id="13cf4-127">Имя</span><span class="sxs-lookup"><span data-stu-id="13cf4-127">Name</span></span> | <span data-ttu-id="13cf4-128">Описание</span><span class="sxs-lookup"><span data-stu-id="13cf4-128">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="13cf4-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="13cf4-129">Authorization</span></span>  | <span data-ttu-id="13cf4-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="13cf4-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="13cf4-132">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="13cf4-132">ConsistencyLevel</span></span> | <span data-ttu-id="13cf4-133">необязательный.</span><span class="sxs-lookup"><span data-stu-id="13cf4-133">eventual.</span></span> <span data-ttu-id="13cf4-134">Этот заголовок и `$count` требуются при использовании `$search`, `$filter`, `$orderby` или с параметрами запросов OData cast.</span><span class="sxs-lookup"><span data-stu-id="13cf4-134">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="13cf4-135">В нем используется индекс, который может не соответствовать последним изменениям объекта.</span><span class="sxs-lookup"><span data-stu-id="13cf4-135">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="13cf4-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="13cf4-136">Request body</span></span>

<span data-ttu-id="13cf4-137">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="13cf4-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="13cf4-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="13cf4-138">Response</span></span>

<span data-ttu-id="13cf4-139">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="13cf4-139">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="13cf4-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="13cf4-140">Examples</span></span>

### <a name="example-1-get-groups-and-administrative-units-that-the-group-is-a-transitive-member-of"></a><span data-ttu-id="13cf4-141">Пример 1. Получить группы и административные единицы, которые группа является транзитным членом</span><span class="sxs-lookup"><span data-stu-id="13cf4-141">Example 1: Get groups and administrative units that the group is a transitive member of</span></span>

#### <a name="request"></a><span data-ttu-id="13cf4-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="13cf4-142">Request</span></span>

<span data-ttu-id="13cf4-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="13cf4-143">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="13cf4-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="13cf4-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_transitivememberof"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMemberOf
```
# <a name="c"></a>[<span data-ttu-id="13cf4-145">C#</span><span class="sxs-lookup"><span data-stu-id="13cf4-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-transitivememberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="13cf4-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="13cf4-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-transitivememberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="13cf4-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="13cf4-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-transitivememberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="13cf4-148">Java</span><span class="sxs-lookup"><span data-stu-id="13cf4-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-transitivememberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="13cf4-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="13cf4-149">Response</span></span>

<span data-ttu-id="13cf4-150">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="13cf4-150">The following is an example of the response.</span></span>
><span data-ttu-id="13cf4-151">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="13cf4-151">**Note:** The response object shown here might be shortened for readability.</span></span>

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
      "mailNickname": "ContosoGroup1",
      "securityEnabled": true
    }
  ]
}
```

### <a name="example-2-get-only-a-count-of-all-transitive-membership"></a><span data-ttu-id="13cf4-152">Пример 2: Получение только количества транзитивных участников</span><span class="sxs-lookup"><span data-stu-id="13cf4-152">Example 2: Get only a count of all transitive membership</span></span>

#### <a name="request"></a><span data-ttu-id="13cf4-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="13cf4-153">Request</span></span>

<span data-ttu-id="13cf4-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="13cf4-154">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMemberOf/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="13cf4-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="13cf4-155">Response</span></span>

<span data-ttu-id="13cf4-156">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="13cf4-156">The following is an example of the response.</span></span>

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

<span data-ttu-id="13cf4-157">294</span><span class="sxs-lookup"><span data-stu-id="13cf4-157">294</span></span>

### <a name="example-3-use-odata-cast-to-get-only-a-count-of-transitive-membership-in-groups"></a><span data-ttu-id="13cf4-158">Пример 3. Использование OData cast для получения только количества транзитивных участников в группах</span><span class="sxs-lookup"><span data-stu-id="13cf4-158">Example 3: Use OData cast to get only a count of transitive membership in groups</span></span>

#### <a name="request"></a><span data-ttu-id="13cf4-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="13cf4-159">Request</span></span>

<span data-ttu-id="13cf4-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="13cf4-160">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMemberOf/microsoft.graph.group/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="13cf4-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="13cf4-161">Response</span></span>

<span data-ttu-id="13cf4-162">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="13cf4-162">The following is an example of the response.</span></span>

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

<span data-ttu-id="13cf4-163">294</span><span class="sxs-lookup"><span data-stu-id="13cf4-163">294</span></span>


### <a name="example-4-use-odata-cast-and-search-to-get-membership-in-groups-with-display-names-that-contain-the-letters-tier-including-a-count-of-returned-objects"></a><span data-ttu-id="13cf4-164">Пример 4. Использование литых и $search OData для получения членства в группах с отображаемой именами, которые содержат буквы "tier", включая количество возвращенных объектов</span><span class="sxs-lookup"><span data-stu-id="13cf4-164">Example 4: Use OData cast and $search to get membership in groups with display names that contain the letters 'tier' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="13cf4-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="13cf4-165">Request</span></span>

<span data-ttu-id="13cf4-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="13cf4-166">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_tier_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderby=displayName&$search="displayName:tier"&$select=displayName,id
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="13cf4-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="13cf4-167">Response</span></span>

<span data-ttu-id="13cf4-168">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="13cf4-168">The following is an example of the response.</span></span>
><span data-ttu-id="13cf4-169">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="13cf4-169">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups(displayName,id)",
  "@odata.count":7,
  "value":[
    {
      "displayName":"Contoso-tier Query Notification",
      "id":"11111111-2222-3333-4444-555555555555"
    }
  ]
}
```

### <a name="example-5-use-odata-cast-and-filter-to-get-membership-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="13cf4-170">Пример 5. Использование литых и $filter OData для получения членства с именем отображения, которое начинается с "A", включая количество возвращенных объектов</span><span class="sxs-lookup"><span data-stu-id="13cf4-170">Example 5: Use OData cast and $filter to get membership with a display name that starts with 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="13cf4-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="13cf4-171">Request</span></span>

<span data-ttu-id="13cf4-172">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="13cf4-172">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderby=displayName&$filter=startswith(displayName, 'a')
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="13cf4-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="13cf4-173">Response</span></span>

<span data-ttu-id="13cf4-174">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="13cf4-174">The following is an example of the response.</span></span>
><span data-ttu-id="13cf4-175">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="13cf4-175">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "description": "List group transitive memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


