---
title: Перечисление транзитивных участников группы
description: Получите список участников группы.
localization_priority: Normal
author: Jordanndahl
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 596bdaf0ba02046465cb2456f4c2c88e935f31d4
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53207235"
---
# <a name="list-group-transitive-members"></a><span data-ttu-id="256d5-103">Перечисление транзитивных участников группы</span><span class="sxs-lookup"><span data-stu-id="256d5-103">List group transitive members</span></span>

<span data-ttu-id="256d5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="256d5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="256d5-105">Получите список участников группы.</span><span class="sxs-lookup"><span data-stu-id="256d5-105">Get a list of the group's members.</span></span> <span data-ttu-id="256d5-106">В группе могут быть пользователи, контакты, устройства, директора службы и другие группы в качестве участников.</span><span class="sxs-lookup"><span data-stu-id="256d5-106">A group can have users, contacts, devices, service principals, and other groups as members.</span></span> <span data-ttu-id="256d5-107">Эта операция является транзитной и также возвращает плоский список всех вложенных членов.</span><span class="sxs-lookup"><span data-stu-id="256d5-107">This operation is transitive and will also return a flat list of all nested members.</span></span>

## <a name="permissions"></a><span data-ttu-id="256d5-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="256d5-108">Permissions</span></span>

<span data-ttu-id="256d5-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="256d5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="256d5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="256d5-111">Permission type</span></span> | <span data-ttu-id="256d5-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="256d5-112">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="256d5-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="256d5-113">Delegated (work or school account)</span></span> | <span data-ttu-id="256d5-114">GroupMember.Read.All, Group.Read.All, GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="256d5-114">GroupMember.Read.All, Group.Read.All, GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
| <span data-ttu-id="256d5-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="256d5-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="256d5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="256d5-116">Not supported.</span></span> |
| <span data-ttu-id="256d5-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="256d5-117">Application</span></span> | <span data-ttu-id="256d5-118">GroupMember.Read.All, Group.Read.All, GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="256d5-118">GroupMember.Read.All, Group.Read.All, GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All</span></span> |

> <span data-ttu-id="256d5-119">**Примечание:** Чтобы перечислить членов скрытой группы членства, требуется разрешение *Member.Read.Hidden.*</span><span class="sxs-lookup"><span data-stu-id="256d5-119">**Note:** To list the members of a hidden membership group, the *Member.Read.Hidden* permission is required.</span></span>

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="256d5-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="256d5-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /groups/{id}/transitiveMembers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="256d5-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="256d5-121">Optional query parameters</span></span>

<span data-ttu-id="256d5-122">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа, в том числе `$search`, `$count` і `$filter`.</span><span class="sxs-lookup"><span data-stu-id="256d5-122">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="256d5-123">Вы можете использовать `$search` в свойствах **displayName** и **description**.</span><span class="sxs-lookup"><span data-stu-id="256d5-123">You can use `$search` on the **displayName** and **description** properties.</span></span> <span data-ttu-id="256d5-124">Когда элементы добавляются или обновляются для этого ресурса, они специально индексируются для использования с помощью параметров `$count` и `$search`.</span><span class="sxs-lookup"><span data-stu-id="256d5-124">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="256d5-125">Между добавлением или обновлением элемента и его появлением в индексе может возникать небольшая задержка.</span><span class="sxs-lookup"><span data-stu-id="256d5-125">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

<span data-ttu-id="256d5-126">Чтобы отфильтровать результаты по типу OData, например или , необходимо использовать расширенные `microsoft.graph.user` `microsoft.graph.group` [параметры запроса.](/graph/aad-advanced-queries)</span><span class="sxs-lookup"><span data-stu-id="256d5-126">To filter the results on the OData type, such as `microsoft.graph.user` or `microsoft.graph.group`, you must use the [advanced query parameters](/graph/aad-advanced-queries).</span></span> <span data-ttu-id="256d5-127">То есть **заглавная строка ConsistencyLevel** и `eventual` `$count=true` строка запроса.</span><span class="sxs-lookup"><span data-stu-id="256d5-127">That is, the **ConsistencyLevel** header set to `eventual` and the `$count=true` query string.</span></span>

## <a name="request-headers"></a><span data-ttu-id="256d5-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="256d5-128">Request headers</span></span>

| <span data-ttu-id="256d5-129">Имя</span><span class="sxs-lookup"><span data-stu-id="256d5-129">Name</span></span> | <span data-ttu-id="256d5-130">Описание</span><span class="sxs-lookup"><span data-stu-id="256d5-130">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="256d5-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="256d5-131">Authorization</span></span>  | <span data-ttu-id="256d5-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="256d5-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="256d5-134">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="256d5-134">ConsistencyLevel</span></span> | <span data-ttu-id="256d5-135">необязательный.</span><span class="sxs-lookup"><span data-stu-id="256d5-135">eventual.</span></span> <span data-ttu-id="256d5-136">Этот заголовок и `$count` требуются при использовании `$search`, `$filter`, `$orderby` или с параметрами запросов OData cast.</span><span class="sxs-lookup"><span data-stu-id="256d5-136">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="256d5-137">В нем используется индекс, который может не соответствовать последним изменениям объекта.</span><span class="sxs-lookup"><span data-stu-id="256d5-137">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="256d5-138">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="256d5-138">Request body</span></span>

<span data-ttu-id="256d5-139">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="256d5-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="256d5-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="256d5-140">Response</span></span>

<span data-ttu-id="256d5-141">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="256d5-141">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="256d5-142">Примеры</span><span class="sxs-lookup"><span data-stu-id="256d5-142">Examples</span></span>

### <a name="example-1-get-the-transitive-membership-of-a-group"></a><span data-ttu-id="256d5-143">Пример 1. Получить транзитное членство группы</span><span class="sxs-lookup"><span data-stu-id="256d5-143">Example 1: Get the transitive membership of a group</span></span>

#### <a name="request"></a><span data-ttu-id="256d5-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="256d5-144">Request</span></span>

<span data-ttu-id="256d5-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="256d5-145">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="256d5-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="256d5-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_transitivemembers"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMembers
```
# <a name="c"></a>[<span data-ttu-id="256d5-147">C#</span><span class="sxs-lookup"><span data-stu-id="256d5-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-transitivemembers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="256d5-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="256d5-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-transitivemembers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="256d5-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="256d5-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-transitivemembers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="256d5-150">Java</span><span class="sxs-lookup"><span data-stu-id="256d5-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-transitivemembers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="256d5-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="256d5-151">Response</span></span>

<span data-ttu-id="256d5-152">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="256d5-152">The following is an example of the response.</span></span>

><span data-ttu-id="256d5-153">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="256d5-153">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-get-only-a-count-of-transitive-membership"></a><span data-ttu-id="256d5-154">Пример 2. Получить только число транзитных членов</span><span class="sxs-lookup"><span data-stu-id="256d5-154">Example 2: Get only a count of transitive membership</span></span>

#### <a name="request"></a><span data-ttu-id="256d5-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="256d5-155">Request</span></span>

<span data-ttu-id="256d5-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="256d5-156">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="256d5-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="256d5-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "ignored",
  "name": "get_group_transitivemembers_count"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMembers/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="256d5-158">C#</span><span class="sxs-lookup"><span data-stu-id="256d5-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-transitivemembers-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="256d5-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="256d5-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-transitivemembers-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="256d5-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="256d5-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-transitivemembers-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="256d5-161">Java</span><span class="sxs-lookup"><span data-stu-id="256d5-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-transitivemembers-count-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="256d5-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="256d5-162">Response</span></span>

<span data-ttu-id="256d5-163">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="256d5-163">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain

893
```


### <a name="example-3-use-the-microsoftgraphgroup-odata-cast-to-get-only-members-that-are-groups"></a><span data-ttu-id="256d5-164">Пример 3. Использование литой OData microsoft.graph.group для получения только участников, которые являются группами.</span><span class="sxs-lookup"><span data-stu-id="256d5-164">Example 3: Use the microsoft.graph.group OData cast to get only members that are groups</span></span>

#### <a name="request"></a><span data-ttu-id="256d5-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="256d5-165">Request</span></span>

<span data-ttu-id="256d5-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="256d5-166">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="256d5-167">HTTP</span><span class="sxs-lookup"><span data-stu-id="256d5-167">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_transitivemembers_odataCast"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitivemembers/microsoft.graph.group?$count=true
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="256d5-168">C#</span><span class="sxs-lookup"><span data-stu-id="256d5-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-transitivemembers-odatacast-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="256d5-169">JavaScript</span><span class="sxs-lookup"><span data-stu-id="256d5-169">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-transitivemembers-odatacast-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="256d5-170">Objective-C</span><span class="sxs-lookup"><span data-stu-id="256d5-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-transitivemembers-odatacast-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="256d5-171">Java</span><span class="sxs-lookup"><span data-stu-id="256d5-171">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-transitivemembers-odatacast-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="256d5-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="256d5-172">Response</span></span>

<span data-ttu-id="256d5-173">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="256d5-173">The following is an example of the response.</span></span>

><span data-ttu-id="256d5-174">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="256d5-174">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups",
  "@odata.count": 2,
  "value": [
    {
      "@odata.id": "https://graph.microsoft.com/v2/927c6607-8060-4f4a-a5f8-34964ac78d70/directoryObjects/4d0ef681-e88f-42a3-a2db-e6bf1e249e10/Microsoft.DirectoryServices.Group",
      "id": "4d0ef681-e88f-42a3-a2db-e6bf1e249e10",
      "organizationId": "927c6607-8060-4f4a-a5f8-34964ac78d70",
      "description": null,
      "displayName": "Executives",
      "groupTypes": [],
      "mail": "Executives@contoso.com",
      "mailEnabled": true,
      "mailNickname": "Executives",
    },
    {
      "@odata.id": "https://graph.microsoft.com/v2/927c6607-8060-4f4a-a5f8-34964ac78d70/directoryObjects/d9fb0c47-c783-40a1-bce1-53b52ada51fc/Microsoft.DirectoryServices.Group",
      "id": "d9fb0c47-c783-40a1-bce1-53b52ada51fc",
      "organizationId": "927c6607-8060-4f4a-a5f8-34964ac78d70",
      "displayName": "Project Falcon",
      "groupTypes": [],
      "mail": "Falcon@contoso.com",
      "mailEnabled": true,
      "mailNickname": "Falcon",
    }
  ]
}
```

### <a name="example-4-use-odata-cast-and-search-to-get-membership-in-groups-with-display-names-that-contain-the-letters-tier-including-a-count-of-returned-objects"></a><span data-ttu-id="256d5-175">Пример 4. Использование литых и $search OData для получения членства в группах с отображаемой именами, которые содержат буквы "tier", включая количество возвращенных объектов</span><span class="sxs-lookup"><span data-stu-id="256d5-175">Example 4: Use OData cast and $search to get membership in groups with display names that contain the letters 'tier' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="256d5-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="256d5-176">Request</span></span>

<span data-ttu-id="256d5-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="256d5-177">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="256d5-178">HTTP</span><span class="sxs-lookup"><span data-stu-id="256d5-178">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tier_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMembers/microsoft.graph.user?$count=true&$orderBy=displayName&$search="displayName:tier"&$select=displayName,id
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="256d5-179">C#</span><span class="sxs-lookup"><span data-stu-id="256d5-179">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tier-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="256d5-180">JavaScript</span><span class="sxs-lookup"><span data-stu-id="256d5-180">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tier-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="256d5-181">Objective-C</span><span class="sxs-lookup"><span data-stu-id="256d5-181">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tier-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="256d5-182">Java</span><span class="sxs-lookup"><span data-stu-id="256d5-182">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-tier-count-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="256d5-183">Отклик</span><span class="sxs-lookup"><span data-stu-id="256d5-183">Response</span></span>

<span data-ttu-id="256d5-184">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="256d5-184">The following is an example of the response.</span></span>
><span data-ttu-id="256d5-185">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="256d5-185">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-5-use-odata-cast-and-filter-to-get-user-membership-in-groups-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="256d5-186">Пример 5. Использование литых и $filter OData для получения членства пользователя в группах с отображаемой именем, которая начинается с "A", включая количество возвращенных объектов</span><span class="sxs-lookup"><span data-stu-id="256d5-186">Example 5: Use OData cast and $filter to get user membership in groups with a display name that starts with 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="256d5-187">Запрос</span><span class="sxs-lookup"><span data-stu-id="256d5-187">Request</span></span>

<span data-ttu-id="256d5-188">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="256d5-188">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="256d5-189">HTTP</span><span class="sxs-lookup"><span data-stu-id="256d5-189">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMembers/microsoft.graph.user?$count=true&$orderBy=displayName&$filter=startswith(displayName, 'a')
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="256d5-190">C#</span><span class="sxs-lookup"><span data-stu-id="256d5-190">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-a-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="256d5-191">JavaScript</span><span class="sxs-lookup"><span data-stu-id="256d5-191">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-a-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="256d5-192">Objective-C</span><span class="sxs-lookup"><span data-stu-id="256d5-192">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-a-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="256d5-193">Java</span><span class="sxs-lookup"><span data-stu-id="256d5-193">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-a-count-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="256d5-194">Отклик</span><span class="sxs-lookup"><span data-stu-id="256d5-194">Response</span></span>

<span data-ttu-id="256d5-195">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="256d5-195">The following is an example of the response.</span></span>
><span data-ttu-id="256d5-196">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="256d5-196">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "description": "List transitive group members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


