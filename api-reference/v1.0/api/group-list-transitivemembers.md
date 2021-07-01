---
title: Перечисление транзитивных участников группы
description: Получите список участников группы. В составе группы могут быть пользователи, устройства, организационные контакты и другие группы. Эта операция является транзитной и возвращает плоский список всех вложенных членов.
author: Jordanndahl
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: edef20f23978b7a9b98e4e78d87ba0546e6fd439
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53209464"
---
# <a name="list-group-transitive-members"></a><span data-ttu-id="6f66a-105">Перечисление транзитивных участников группы</span><span class="sxs-lookup"><span data-stu-id="6f66a-105">List group transitive members</span></span>

<span data-ttu-id="6f66a-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6f66a-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6f66a-107">Получите список участников группы.</span><span class="sxs-lookup"><span data-stu-id="6f66a-107">Get a list of the group's members.</span></span> <span data-ttu-id="6f66a-108">В составе группы могут быть пользователи, устройства, организационные контакты и другие группы.</span><span class="sxs-lookup"><span data-stu-id="6f66a-108">A group can have users, devices, organizational contacts, and other groups as members.</span></span> <span data-ttu-id="6f66a-109">Эта операция является транзитной и возвращает плоский список всех вложенных членов.</span><span class="sxs-lookup"><span data-stu-id="6f66a-109">This operation is transitive and returns a flat list of all nested members.</span></span>

## <a name="permissions"></a><span data-ttu-id="6f66a-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6f66a-110">Permissions</span></span>

<span data-ttu-id="6f66a-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f66a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f66a-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6f66a-113">Permission type</span></span>      | <span data-ttu-id="6f66a-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6f66a-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6f66a-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6f66a-115">Delegated (work or school account)</span></span> | <span data-ttu-id="6f66a-116">GroupMember.Read.All, Group.Read.All, GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6f66a-116">GroupMember.Read.All, Group.Read.All, GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="6f66a-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6f66a-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6f66a-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f66a-118">Not supported.</span></span>    |
|<span data-ttu-id="6f66a-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6f66a-119">Application</span></span> | <span data-ttu-id="6f66a-120">GroupMember.Read.All, Group.Read.All, GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="6f66a-120">GroupMember.Read.All, Group.Read.All, GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All</span></span> |

><span data-ttu-id="6f66a-121">**Примечание:** Чтобы перечислить членов скрытой группы членства, требуется разрешение *Member.Read.Hidden.*</span><span class="sxs-lookup"><span data-stu-id="6f66a-121">**Note:** To list the members of a hidden membership group, the *Member.Read.Hidden* permission is required.</span></span>

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="6f66a-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6f66a-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /groups/{id}/transitiveMembers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6f66a-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6f66a-123">Optional query parameters</span></span>

<span data-ttu-id="6f66a-124">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа, в том числе `$search`, `$count` і `$filter`.</span><span class="sxs-lookup"><span data-stu-id="6f66a-124">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="6f66a-125">Вы можете использовать `$search` в свойствах **displayName** и **description**.</span><span class="sxs-lookup"><span data-stu-id="6f66a-125">You can use `$search` on the **displayName** and **description** properties.</span></span> <span data-ttu-id="6f66a-126">Когда элементы добавляются или обновляются для этого ресурса, они специально индексируются для использования с помощью параметров `$count` и `$search`.</span><span class="sxs-lookup"><span data-stu-id="6f66a-126">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="6f66a-127">Между добавлением или обновлением элемента и его появлением в индексе может возникать небольшая задержка.</span><span class="sxs-lookup"><span data-stu-id="6f66a-127">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

<span data-ttu-id="6f66a-128">Чтобы отфильтровать результаты по типу OData, например или , необходимо использовать расширенные `microsoft.graph.user` `microsoft.graph.group` [параметры запроса.](/graph/aad-advanced-queries)</span><span class="sxs-lookup"><span data-stu-id="6f66a-128">To filter the results on the OData type, such as `microsoft.graph.user` or `microsoft.graph.group`, you must use the [advanced query parameters](/graph/aad-advanced-queries).</span></span> <span data-ttu-id="6f66a-129">То есть **заглавная строка ConsistencyLevel** и `eventual` `$count=true` строка запроса.</span><span class="sxs-lookup"><span data-stu-id="6f66a-129">That is, the **ConsistencyLevel** header set to `eventual` and the `$count=true` query string.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6f66a-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6f66a-130">Request headers</span></span>

| <span data-ttu-id="6f66a-131">Имя</span><span class="sxs-lookup"><span data-stu-id="6f66a-131">Name</span></span> | <span data-ttu-id="6f66a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="6f66a-132">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="6f66a-133">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6f66a-133">Authorization</span></span>  | <span data-ttu-id="6f66a-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6f66a-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6f66a-136">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="6f66a-136">ConsistencyLevel</span></span> | <span data-ttu-id="6f66a-137">необязательный.</span><span class="sxs-lookup"><span data-stu-id="6f66a-137">eventual.</span></span> <span data-ttu-id="6f66a-138">Этот заголовок и `$count` требуются при использовании `$search`, `$filter`, `$orderby` или с параметрами запросов OData cast.</span><span class="sxs-lookup"><span data-stu-id="6f66a-138">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="6f66a-139">В нем используется индекс, который может не соответствовать последним изменениям объекта.</span><span class="sxs-lookup"><span data-stu-id="6f66a-139">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6f66a-140">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6f66a-140">Request body</span></span>

<span data-ttu-id="6f66a-141">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6f66a-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6f66a-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="6f66a-142">Response</span></span>

<span data-ttu-id="6f66a-143">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6f66a-143">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6f66a-144">Примеры</span><span class="sxs-lookup"><span data-stu-id="6f66a-144">Examples</span></span>

### <a name="example-1-get-the-transitive-membership-of-a-group"></a><span data-ttu-id="6f66a-145">Пример 1. Получить транзитное членство группы</span><span class="sxs-lookup"><span data-stu-id="6f66a-145">Example 1: Get the transitive membership of a group</span></span>

#### <a name="request"></a><span data-ttu-id="6f66a-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="6f66a-146">Request</span></span>

<span data-ttu-id="6f66a-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6f66a-147">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6f66a-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="6f66a-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_transitivemembers"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/transitiveMembers
```
# <a name="c"></a>[<span data-ttu-id="6f66a-149">C#</span><span class="sxs-lookup"><span data-stu-id="6f66a-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-transitivemembers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6f66a-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6f66a-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-transitivemembers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6f66a-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6f66a-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-transitivemembers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6f66a-152">Java</span><span class="sxs-lookup"><span data-stu-id="6f66a-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-transitivemembers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="6f66a-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="6f66a-153">Response</span></span>

<span data-ttu-id="6f66a-154">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6f66a-154">The following is an example of the response.</span></span>

><span data-ttu-id="6f66a-155">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="6f66a-155">**Note**: The response object shown here might be shortened for readability.</span></span>

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
      "@odata.type": "#microsoft.graph.user",
      "id": "11111111-2222-3333-4444-555555555555",
      "mail": "group1@contoso.com"
    }
  ]
}
```

### <a name="example-2-get-only-a-count-of-transitive-membership"></a><span data-ttu-id="6f66a-156">Пример 2. Получить только число транзитных членов</span><span class="sxs-lookup"><span data-stu-id="6f66a-156">Example 2: Get only a count of transitive membership</span></span>

#### <a name="request"></a><span data-ttu-id="6f66a-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="6f66a-157">Request</span></span>

<span data-ttu-id="6f66a-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6f66a-158">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="6f66a-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="6f66a-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "ignored",
  "name": "get_group_transitivemembers_count"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/transitiveMembers/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="6f66a-160">C#</span><span class="sxs-lookup"><span data-stu-id="6f66a-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-transitivemembers-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6f66a-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6f66a-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-transitivemembers-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6f66a-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6f66a-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-transitivemembers-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6f66a-163">Java</span><span class="sxs-lookup"><span data-stu-id="6f66a-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-transitivemembers-count-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6f66a-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="6f66a-164">Response</span></span>

<span data-ttu-id="6f66a-165">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="6f66a-165">The following is an example of the response.</span></span>

><span data-ttu-id="6f66a-166">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="6f66a-166">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain


893
```

### <a name="example-3-use-the-microsoftgraphgroup-odata-cast-to-get-only-members-that-are-groups"></a><span data-ttu-id="6f66a-167">Пример 3. Использование литой OData microsoft.graph.group для получения только участников, которые являются группами.</span><span class="sxs-lookup"><span data-stu-id="6f66a-167">Example 3: Use the microsoft.graph.group OData cast to get only members that are groups</span></span>

#### <a name="request"></a><span data-ttu-id="6f66a-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="6f66a-168">Request</span></span>

<span data-ttu-id="6f66a-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6f66a-169">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="6f66a-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="6f66a-170">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_transitivemembers_odataCast"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/transitivemembers/microsoft.graph.group?$count=true
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="6f66a-171">C#</span><span class="sxs-lookup"><span data-stu-id="6f66a-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-transitivemembers-odatacast-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6f66a-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6f66a-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-transitivemembers-odatacast-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6f66a-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6f66a-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-transitivemembers-odatacast-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6f66a-174">Java</span><span class="sxs-lookup"><span data-stu-id="6f66a-174">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-transitivemembers-odatacast-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6f66a-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="6f66a-175">Response</span></span>

<span data-ttu-id="6f66a-176">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="6f66a-176">The following is an example of the response.</span></span>

><span data-ttu-id="6f66a-177">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="6f66a-177">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups",
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

### <a name="example-4-use-odata-cast-and-search-to-get-membership-in-groups-with-display-names-that-contain-the-letters-tier-including-a-count-of-returned-objects"></a><span data-ttu-id="6f66a-178">Пример 4. Использование литых и $search OData для получения членства в группах с отображаемой именами, которые содержат буквы "tier", включая количество возвращенных объектов</span><span class="sxs-lookup"><span data-stu-id="6f66a-178">Example 4: Use OData cast and $search to get membership in groups with display names that contain the letters 'tier' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="6f66a-179">Запрос</span><span class="sxs-lookup"><span data-stu-id="6f66a-179">Request</span></span>

<span data-ttu-id="6f66a-180">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6f66a-180">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="6f66a-181">HTTP</span><span class="sxs-lookup"><span data-stu-id="6f66a-181">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tier_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/transitiveMembers/microsoft.graph.user?$count=true&$orderBy=displayName&$search="displayName:tier"&$select=displayName,id
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="6f66a-182">C#</span><span class="sxs-lookup"><span data-stu-id="6f66a-182">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tier-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6f66a-183">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6f66a-183">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tier-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6f66a-184">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6f66a-184">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tier-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6f66a-185">Java</span><span class="sxs-lookup"><span data-stu-id="6f66a-185">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-tier-count-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6f66a-186">Отклик</span><span class="sxs-lookup"><span data-stu-id="6f66a-186">Response</span></span>

<span data-ttu-id="6f66a-187">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="6f66a-187">The following is an example of the response.</span></span>

><span data-ttu-id="6f66a-188">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="6f66a-188">**Note:** The response object shown here might be shortened for readability.</span></span>

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
    }
  ]
}
```


### <a name="example-5-use-odata-cast-and-filter-to-get-user-membership-in-groups-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="6f66a-189">Пример 5. Использование литых и $filter OData для получения членства пользователя в группах с отображаемой именем, которая начинается с "A", включая количество возвращенных объектов</span><span class="sxs-lookup"><span data-stu-id="6f66a-189">Example 5: Use OData cast and $filter to get user membership in groups with a display name that starts with 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="6f66a-190">Запрос</span><span class="sxs-lookup"><span data-stu-id="6f66a-190">Request</span></span>

<span data-ttu-id="6f66a-191">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6f66a-191">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="6f66a-192">HTTP</span><span class="sxs-lookup"><span data-stu-id="6f66a-192">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/transitiveMembers/microsoft.graph.user?$count=true&$orderBy=displayName&$filter=startswith(displayName, 'a')
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="6f66a-193">C#</span><span class="sxs-lookup"><span data-stu-id="6f66a-193">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-a-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6f66a-194">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6f66a-194">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-a-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6f66a-195">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6f66a-195">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-a-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6f66a-196">Java</span><span class="sxs-lookup"><span data-stu-id="6f66a-196">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-a-count-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6f66a-197">Отклик</span><span class="sxs-lookup"><span data-stu-id="6f66a-197">Response</span></span>

<span data-ttu-id="6f66a-198">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="6f66a-198">The following is an example of the response.</span></span>

><span data-ttu-id="6f66a-199">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="6f66a-199">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
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
  "description": "List transitive group members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
