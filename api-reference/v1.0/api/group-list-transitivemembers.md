---
title: Перечисление транзитивных участников группы
description: Получение списка членов группы. У группы могут быть пользователи, устройства, организационные контакты и другие группы в качестве участников. Эта операция является транзитивным и возвращает плоский список всех вложенных элементов.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 9566b3dea679b1b96566c4960e939079b8d89634
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/04/2020
ms.locfileid: "48904839"
---
# <a name="list-group-transitive-members"></a><span data-ttu-id="551e6-105">Перечисление транзитивных участников группы</span><span class="sxs-lookup"><span data-stu-id="551e6-105">List group transitive members</span></span>

<span data-ttu-id="551e6-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="551e6-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="551e6-107">Получение списка членов группы.</span><span class="sxs-lookup"><span data-stu-id="551e6-107">Get a list of the group's members.</span></span> <span data-ttu-id="551e6-108">У группы могут быть пользователи, устройства, организационные контакты и другие группы в качестве участников.</span><span class="sxs-lookup"><span data-stu-id="551e6-108">A group can have users, devices, organizational contacts, and other groups as members.</span></span> <span data-ttu-id="551e6-109">Эта операция является транзитивным и возвращает плоский список всех вложенных элементов.</span><span class="sxs-lookup"><span data-stu-id="551e6-109">This operation is transitive and returns a flat list of all nested members.</span></span>

## <a name="permissions"></a><span data-ttu-id="551e6-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="551e6-110">Permissions</span></span>

<span data-ttu-id="551e6-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="551e6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="551e6-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="551e6-113">Permission type</span></span>      | <span data-ttu-id="551e6-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="551e6-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="551e6-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="551e6-115">Delegated (work or school account)</span></span> | <span data-ttu-id="551e6-116">Directory. Read. ALL, Directory. AccessAsUser. ALL, User. ReadBasic. ALL, User. Read. ALL, Application. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="551e6-116">Directory.Read.All, Directory.AccessAsUser.All, User.ReadBasic.All, User.Read.All, Application.Read.All</span></span>  |
|<span data-ttu-id="551e6-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="551e6-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="551e6-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="551e6-118">Not supported.</span></span>    |
|<span data-ttu-id="551e6-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="551e6-119">Application</span></span> | <span data-ttu-id="551e6-120">Directory. Read. ALL, User. Read. ALL, Application. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="551e6-120">Directory.Read.All, User.Read.All, Application.Read.All</span></span> |

><span data-ttu-id="551e6-121">**Примечание:** Чтобы получить список членов скрытой группы членства, требуется разрешение Member. Read. Hidden.</span><span class="sxs-lookup"><span data-stu-id="551e6-121">**Note:** To list the members of a hidden membership group, the Member.Read.Hidden permission is required.</span></span>

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="551e6-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="551e6-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /groups/{id}/transitiveMembers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="551e6-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="551e6-123">Optional query parameters</span></span>

<span data-ttu-id="551e6-124">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа, в том числе `$search`, `$count` і `$filter`.</span><span class="sxs-lookup"><span data-stu-id="551e6-124">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="551e6-125">Вы можете использовать `$search` в свойствах **displayName** и **description**.</span><span class="sxs-lookup"><span data-stu-id="551e6-125">You can use `$search` on the **displayName** and **description** properties.</span></span> <span data-ttu-id="551e6-126">Когда элементы добавляются или обновляются для этого ресурса, они специально индексируются для использования с помощью параметров `$count` и `$search`.</span><span class="sxs-lookup"><span data-stu-id="551e6-126">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="551e6-127">Между добавлением или обновлением элемента и его появлением в индексе может возникать небольшая задержка.</span><span class="sxs-lookup"><span data-stu-id="551e6-127">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="551e6-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="551e6-128">Request headers</span></span>

| <span data-ttu-id="551e6-129">Имя</span><span class="sxs-lookup"><span data-stu-id="551e6-129">Name</span></span> | <span data-ttu-id="551e6-130">Описание</span><span class="sxs-lookup"><span data-stu-id="551e6-130">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="551e6-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="551e6-131">Authorization</span></span>  | <span data-ttu-id="551e6-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="551e6-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="551e6-134">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="551e6-134">ConsistencyLevel</span></span> | <span data-ttu-id="551e6-135">необязательный.</span><span class="sxs-lookup"><span data-stu-id="551e6-135">eventual.</span></span> <span data-ttu-id="551e6-136">Этот заголовок и `$count` требуются при использовании `$search`, `$filter`, `$orderby` или с параметрами запросов OData cast.</span><span class="sxs-lookup"><span data-stu-id="551e6-136">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="551e6-137">В нем используется индекс, который может не соответствовать последним изменениям объекта.</span><span class="sxs-lookup"><span data-stu-id="551e6-137">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="551e6-138">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="551e6-138">Request body</span></span>

<span data-ttu-id="551e6-139">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="551e6-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="551e6-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="551e6-140">Response</span></span>

<span data-ttu-id="551e6-141">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="551e6-141">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="551e6-142">Примеры</span><span class="sxs-lookup"><span data-stu-id="551e6-142">Examples</span></span>

### <a name="example-1-get-the-transitive-membership-of-a-group"></a><span data-ttu-id="551e6-143">Пример 1: получение транзитивного членства в группе</span><span class="sxs-lookup"><span data-stu-id="551e6-143">Example 1: Get the transitive membership of a group</span></span>

#### <a name="request"></a><span data-ttu-id="551e6-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="551e6-144">Request</span></span>

<span data-ttu-id="551e6-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="551e6-145">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="551e6-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="551e6-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_transitivemembers"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/transitiveMembers
```
# <a name="c"></a>[<span data-ttu-id="551e6-147">C#</span><span class="sxs-lookup"><span data-stu-id="551e6-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-transitivemembers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="551e6-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="551e6-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-transitivemembers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="551e6-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="551e6-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-transitivemembers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="551e6-150">Java</span><span class="sxs-lookup"><span data-stu-id="551e6-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-transitivemembers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="551e6-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="551e6-151">Response</span></span>

<span data-ttu-id="551e6-152">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="551e6-152">The following is an example of the response.</span></span>

><span data-ttu-id="551e6-153">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="551e6-153">**Note** : The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-get-only-a-count-of-transitive-membership"></a><span data-ttu-id="551e6-154">Пример 2: получение только числа транзитивных участников</span><span class="sxs-lookup"><span data-stu-id="551e6-154">Example 2: Get only a count of transitive membership</span></span>

#### <a name="request"></a><span data-ttu-id="551e6-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="551e6-155">Request</span></span>

<span data-ttu-id="551e6-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="551e6-156">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="551e6-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="551e6-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_transitivemembers_count"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/transitiveMembers/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="551e6-158">C#</span><span class="sxs-lookup"><span data-stu-id="551e6-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-transitivemembers-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="551e6-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="551e6-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-transitivemembers-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="551e6-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="551e6-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-transitivemembers-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="551e6-161">Java</span><span class="sxs-lookup"><span data-stu-id="551e6-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-transitivemembers-count-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="551e6-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="551e6-162">Response</span></span>

<span data-ttu-id="551e6-163">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="551e6-163">The following is an example of the response.</span></span>

><span data-ttu-id="551e6-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="551e6-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

`893`

### <a name="example-3-use-odata-cast-and-search-to-get-membership-in-groups-with-display-names-that-contain-the-letters-tier-including-a-count-of-returned-objects"></a><span data-ttu-id="551e6-166">Пример 3: использование функции CAST и $search для получения членства в группах с отображаемыми именами, содержащими уровень, включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="551e6-166">Example 3: Use OData cast and $search to get membership in groups with display names that contain the letters 'tier' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="551e6-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="551e6-167">Request</span></span>

<span data-ttu-id="551e6-168">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="551e6-168">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="551e6-169">HTTP</span><span class="sxs-lookup"><span data-stu-id="551e6-169">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tier_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/transitiveMembers/microsoft.graph.user?$count=true&$orderBy=displayName&$search="displayName:tier"&$select=displayName,id
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="551e6-170">C#</span><span class="sxs-lookup"><span data-stu-id="551e6-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tier-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="551e6-171">JavaScript</span><span class="sxs-lookup"><span data-stu-id="551e6-171">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tier-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="551e6-172">Objective-C</span><span class="sxs-lookup"><span data-stu-id="551e6-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tier-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="551e6-173">Java</span><span class="sxs-lookup"><span data-stu-id="551e6-173">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-tier-count-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="551e6-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="551e6-174">Response</span></span>

<span data-ttu-id="551e6-175">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="551e6-175">The following is an example of the response.</span></span>

><span data-ttu-id="551e6-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="551e6-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-4-use-odata-cast-and-filter-to-get-user-membership-in-groups-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="551e6-178">Пример 4: использование функции CAST и $filter для получения членства пользователя в группах с отображаемым именем, начинающимся с "A", включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="551e6-178">Example 4: Use OData cast and $filter to get user membership in groups with a display name that starts with 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="551e6-179">Запрос</span><span class="sxs-lookup"><span data-stu-id="551e6-179">Request</span></span>

<span data-ttu-id="551e6-180">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="551e6-180">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="551e6-181">HTTP</span><span class="sxs-lookup"><span data-stu-id="551e6-181">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/transitiveMembers/microsoft.graph.users?$count=true&$orderBy=displayName&$filter=startswith(displayName, 'a')
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="551e6-182">C#</span><span class="sxs-lookup"><span data-stu-id="551e6-182">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-a-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="551e6-183">JavaScript</span><span class="sxs-lookup"><span data-stu-id="551e6-183">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-a-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="551e6-184">Objective-C</span><span class="sxs-lookup"><span data-stu-id="551e6-184">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-a-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="551e6-185">Java</span><span class="sxs-lookup"><span data-stu-id="551e6-185">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-a-count-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="551e6-186">Отклик</span><span class="sxs-lookup"><span data-stu-id="551e6-186">Response</span></span>

<span data-ttu-id="551e6-187">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="551e6-187">The following is an example of the response.</span></span>

><span data-ttu-id="551e6-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="551e6-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
