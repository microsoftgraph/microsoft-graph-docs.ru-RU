---
title: Перечисление user memberOf
description: Получение групп, ролей каталогов и административных единиц, непосредственным участником которых является пользователь. Эта операция не является транзитивной.
localization_priority: Normal
author: krbain
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: cd6b8c9f1cc9fb051e88c4a47542c046a5d163fe
ms.sourcegitcommit: 186d738f04e5a558da423f2429165fb4fbe780aa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086790"
---
# <a name="list-user-memberof"></a><span data-ttu-id="23b3f-104">Перечисление user memberOf</span><span class="sxs-lookup"><span data-stu-id="23b3f-104">List user memberOf</span></span>

<span data-ttu-id="23b3f-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="23b3f-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="23b3f-106">Получение групп, ролей каталогов и административных единиц, непосредственным участником которых является пользователь.</span><span class="sxs-lookup"><span data-stu-id="23b3f-106">Get groups, directory roles and administrative units that the user is a direct member of.</span></span> <span data-ttu-id="23b3f-107">Эта операция не является транзитивной.</span><span class="sxs-lookup"><span data-stu-id="23b3f-107">This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="23b3f-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="23b3f-108">Permissions</span></span>

<span data-ttu-id="23b3f-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="23b3f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="23b3f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="23b3f-111">Permission type</span></span> | <span data-ttu-id="23b3f-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="23b3f-112">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="23b3f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="23b3f-113">Delegated (work or school account)</span></span> | <span data-ttu-id="23b3f-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="23b3f-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="23b3f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="23b3f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="23b3f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="23b3f-116">Not supported.</span></span> |
| <span data-ttu-id="23b3f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="23b3f-117">Application</span></span> | <span data-ttu-id="23b3f-118">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23b3f-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="23b3f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="23b3f-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/memberOf
or
GET /users/{id | userPrincipalName}/memberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="23b3f-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="23b3f-120">Optional query parameters</span></span>

<span data-ttu-id="23b3f-p104">Этот метод поддерживает [параметры запроса OData](/graph/query_parameters) для настройки отклика, в том числе `$search`, `$count` и `$filter`. Также включено приведение к OData, например, вы можете получить только directoryRoles, участником которых является пользователь. Вы можете использовать параметр `$search` в свойстве **displayName**. При добавлении или обновлении элементов для этого ресурса они индексируются для использования с параметрами запроса `$count` и `$search`. Между добавлением или обновлением элемента и его появлением в индексе может возникать небольшая задержка.</span><span class="sxs-lookup"><span data-stu-id="23b3f-p104">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`. OData cast is also enabled, for example, you can cast to get just the directoryRoles the user is a member of. You can use `$search` on the **displayName** property. When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters. There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="23b3f-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="23b3f-126">Request headers</span></span>

| <span data-ttu-id="23b3f-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="23b3f-127">Header</span></span> | <span data-ttu-id="23b3f-128">Значение</span><span class="sxs-lookup"><span data-stu-id="23b3f-128">Value</span></span> |
|:------ |:----- |
| <span data-ttu-id="23b3f-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="23b3f-129">Authorization</span></span>  | <span data-ttu-id="23b3f-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="23b3f-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="23b3f-132">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="23b3f-132">ConsistencyLevel</span></span> | <span data-ttu-id="23b3f-p106">необязательный. Этот заголовок и `$count` требуются при использовании `$search`, `$filter`, `$orderby` или параметров запросов для преобразования OData. В нем используется индекс, который может не соответствовать последним изменениям объекта.</span><span class="sxs-lookup"><span data-stu-id="23b3f-p106">eventual. This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters. It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="23b3f-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="23b3f-136">Request body</span></span>

<span data-ttu-id="23b3f-137">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="23b3f-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="23b3f-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="23b3f-138">Response</span></span>

<span data-ttu-id="23b3f-139">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="23b3f-139">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="23b3f-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="23b3f-140">Examples</span></span>

### <a name="example-1-get-groups-directory-roles-and-administrative-units-that-the-user-is-a-direct-member-of"></a><span data-ttu-id="23b3f-141">Пример 1. Получение групп, ролей каталогов и административных единиц, непосредственным участником которых является пользователь.</span><span class="sxs-lookup"><span data-stu-id="23b3f-141">Example 1: Get groups, directory roles, and administrative units that the user is a direct member of</span></span>

#### <a name="request"></a><span data-ttu-id="23b3f-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="23b3f-142">Request</span></span>

<span data-ttu-id="23b3f-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="23b3f-143">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="23b3f-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="23b3f-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_user_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/memberOf
```
# <a name="c"></a>[<span data-ttu-id="23b3f-145">C#</span><span class="sxs-lookup"><span data-stu-id="23b3f-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="23b3f-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="23b3f-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="23b3f-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="23b3f-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="23b3f-148">Java</span><span class="sxs-lookup"><span data-stu-id="23b3f-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-user-memberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="23b3f-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="23b3f-149">Response</span></span>

<span data-ttu-id="23b3f-150">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="23b3f-150">The following is an example of the response.</span></span>
><span data-ttu-id="23b3f-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="23b3f-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "displayName": "All Users",
      "mailEnabled": false,
      "securityEnabled": true
    }
  ]
}
```

### <a name="example-2-get-only-a-count-of-all-groups-directory-roles-and-administrative-units-that-the-user-is-a-direct-member-of"></a><span data-ttu-id="23b3f-153">Пример 2. Получение только количества всех групп, ролей каталогов и административных единиц, непосредственным участником которых является пользователь.</span><span class="sxs-lookup"><span data-stu-id="23b3f-153">Example 2: Get only a count of all groups, directory roles, and administrative units that the user is a direct member of</span></span>

#### <a name="request"></a><span data-ttu-id="23b3f-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="23b3f-154">Request</span></span>

<span data-ttu-id="23b3f-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="23b3f-155">Here is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_user_memberof_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/memberOf/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="23b3f-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="23b3f-156">Response</span></span>

<span data-ttu-id="23b3f-157">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="23b3f-157">The following is an example of the response.</span></span>
><span data-ttu-id="23b3f-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="23b3f-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-3-use-odata-cast-to-get-only-a-count-of-group-membership"></a><span data-ttu-id="23b3f-160">Пример 3. Использование OData cast для получения только количества участия в группах</span><span class="sxs-lookup"><span data-stu-id="23b3f-160">Example 3: Use OData cast to get only a count of group membership</span></span>

#### <a name="request"></a><span data-ttu-id="23b3f-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="23b3f-161">Request</span></span>

<span data-ttu-id="23b3f-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="23b3f-162">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/memberOf/microsoft.graph.group/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="23b3f-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="23b3f-163">Response</span></span>

<span data-ttu-id="23b3f-164">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="23b3f-164">The following is an example of the response.</span></span>

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

### <a name="example-4-use-search-and-odata-cast-to-get-membership-in-groups-with-display-names-that-contain-the-letters-tier-including-a-count-of-returned-objects"></a><span data-ttu-id="23b3f-165">Пример 4. Использование параметра $search и приведения к OData для получения участия пользователей в группах с отображаемыми именами, содержащими буквы «tier», включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="23b3f-165">Example 4: Use $search and OData cast to get membership in groups with display names that contain the letters 'tier' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="23b3f-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="23b3f-166">Request</span></span>

<span data-ttu-id="23b3f-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="23b3f-167">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_tier_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/memberOf/microsoft.graph.group?$count=true&$orderby=displayName&$search="displayName:tier"&$select=displayName,id
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="23b3f-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="23b3f-168">Response</span></span>

<span data-ttu-id="23b3f-169">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="23b3f-169">The following is an example of the response.</span></span>
><span data-ttu-id="23b3f-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="23b3f-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-5-use-filter-and-odata-cast-to-get-groups-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="23b3f-172">Пример 5. Использование параметра $filter и приведения к OData для получения групп с отображаемым именем, которое начинается на «а», включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="23b3f-172">Example 5: Use $filter and OData cast to get groups with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="23b3f-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="23b3f-173">Request</span></span>

<span data-ttu-id="23b3f-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="23b3f-174">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderby=displayName&$filter=startswith(displayName, 'a') 
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="23b3f-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="23b3f-175">Response</span></span>

<span data-ttu-id="23b3f-176">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="23b3f-176">The following is an example of the response.</span></span>
><span data-ttu-id="23b3f-p110">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="23b3f-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


