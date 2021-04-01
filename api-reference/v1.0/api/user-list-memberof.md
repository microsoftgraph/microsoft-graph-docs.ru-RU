---
title: Список memberOf
description: 'Получение групп и ролей каталога, непосредственным участником которых является пользователь. '
author: jpettere
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 4dde83056bed84fdbb2b2dd33d23deb5ea9d4b2d
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473971"
---
# <a name="list-memberof"></a><span data-ttu-id="93d3b-103">Список memberOf</span><span class="sxs-lookup"><span data-stu-id="93d3b-103">List memberOf</span></span>

<span data-ttu-id="93d3b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="93d3b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="93d3b-105">Получение [групп](../resources/group.md) и [ролей каталога](../resources/directoryrole.md), непосредственным членом которых является пользователь.</span><span class="sxs-lookup"><span data-stu-id="93d3b-105">Get [groups](../resources/group.md) and [directory roles](../resources/directoryrole.md) that the user is a direct member of.</span></span> 

## <a name="permissions"></a><span data-ttu-id="93d3b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="93d3b-106">Permissions</span></span>
<span data-ttu-id="93d3b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="93d3b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="93d3b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="93d3b-109">Permission type</span></span>      | <span data-ttu-id="93d3b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="93d3b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="93d3b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="93d3b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="93d3b-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="93d3b-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="93d3b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="93d3b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="93d3b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="93d3b-114">Not supported.</span></span>    |
|<span data-ttu-id="93d3b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="93d3b-115">Application</span></span> | <span data-ttu-id="93d3b-116">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93d3b-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="93d3b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="93d3b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/memberOf
GET /users/{id | userPrincipalName}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="93d3b-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="93d3b-118">Optional query parameters</span></span>

<span data-ttu-id="93d3b-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа, в том числе `$search`, `$count` і `$filter`.</span><span class="sxs-lookup"><span data-stu-id="93d3b-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="93d3b-120">Кроме того, включено также приведение к OData, например, вы можете получить только directoryRoles, участником которых является пользователь.</span><span class="sxs-lookup"><span data-stu-id="93d3b-120">OData cast is also enabled, for example, you can cast to get just the directoryRoles the user is a member of.</span></span> <span data-ttu-id="93d3b-121">`$search` можно использовать в свойстве **displayName**.</span><span class="sxs-lookup"><span data-stu-id="93d3b-121">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="93d3b-122">Когда элементы добавляются или обновляются для этого ресурса, они специально индексируются для использования с помощью параметров `$count` и `$search`.</span><span class="sxs-lookup"><span data-stu-id="93d3b-122">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="93d3b-123">Между добавлением или обновлением элемента и его появлением в индексе может возникать небольшая задержка.</span><span class="sxs-lookup"><span data-stu-id="93d3b-123">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="93d3b-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="93d3b-124">Request headers</span></span>
| <span data-ttu-id="93d3b-125">Заголовок</span><span class="sxs-lookup"><span data-stu-id="93d3b-125">Header</span></span>       | <span data-ttu-id="93d3b-126">Значение</span><span class="sxs-lookup"><span data-stu-id="93d3b-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="93d3b-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="93d3b-127">Authorization</span></span>  | <span data-ttu-id="93d3b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="93d3b-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="93d3b-130">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="93d3b-130">ConsistencyLevel</span></span> | <span data-ttu-id="93d3b-131">необязательный.</span><span class="sxs-lookup"><span data-stu-id="93d3b-131">eventual.</span></span> <span data-ttu-id="93d3b-132">Этот заголовок и `$count` требуются при использовании `$search`, `$filter`, `$orderby` или с параметрами запросов OData cast.</span><span class="sxs-lookup"><span data-stu-id="93d3b-132">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="93d3b-133">В нем используется индекс, который может не соответствовать последним изменениям объекта.</span><span class="sxs-lookup"><span data-stu-id="93d3b-133">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="93d3b-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="93d3b-134">Request body</span></span>
<span data-ttu-id="93d3b-135">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="93d3b-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="93d3b-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="93d3b-136">Response</span></span>

<span data-ttu-id="93d3b-137">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="93d3b-137">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="93d3b-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="93d3b-138">Examples</span></span>

### <a name="example-1-get-groups-directory-roles-and-administrative-units-that-the-user-is-a-direct-member-of"></a><span data-ttu-id="93d3b-139">Пример 1. Получение групп, ролей каталогов и административных единиц, непосредственным участником которых является пользователь.</span><span class="sxs-lookup"><span data-stu-id="93d3b-139">Example 1: Get groups, directory roles, and administrative units that the user is a direct member of</span></span>

#### <a name="request"></a><span data-ttu-id="93d3b-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="93d3b-140">Request</span></span>

<span data-ttu-id="93d3b-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="93d3b-141">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="93d3b-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="93d3b-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_get_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{id}/memberOf
```
# <a name="c"></a>[<span data-ttu-id="93d3b-143">C#</span><span class="sxs-lookup"><span data-stu-id="93d3b-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-get-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="93d3b-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="93d3b-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-get-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="93d3b-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="93d3b-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-get-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="93d3b-146">Java</span><span class="sxs-lookup"><span data-stu-id="93d3b-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-get-memberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="93d3b-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="93d3b-147">Response</span></span>

<span data-ttu-id="93d3b-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="93d3b-148">The following is an example of the response.</span></span>

><span data-ttu-id="93d3b-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="93d3b-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-only-a-count-of-all-groups-directory-roles-and-administrative-units-that-the-user-is-a-direct-member-of"></a><span data-ttu-id="93d3b-151">Пример 2. Получение только количества всех групп, ролей каталогов и административных единиц, непосредственным участником которых является пользователь.</span><span class="sxs-lookup"><span data-stu-id="93d3b-151">Example 2: Get only a count of all groups, directory roles, and administrative units that the user is a direct member of</span></span>

#### <a name="request"></a><span data-ttu-id="93d3b-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="93d3b-152">Request</span></span>

<span data-ttu-id="93d3b-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="93d3b-153">Here is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_user_memberof_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{id}/memberOf/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="93d3b-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="93d3b-154">Response</span></span>

<span data-ttu-id="93d3b-155">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="93d3b-155">The following is an example of the response.</span></span>

><span data-ttu-id="93d3b-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="93d3b-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain

17
```

### <a name="example-3-use-odata-cast-to-get-only-a-count-of-group-membership"></a><span data-ttu-id="93d3b-158">Пример 3. Использование OData cast для получения только количества участия в группах</span><span class="sxs-lookup"><span data-stu-id="93d3b-158">Example 3: Use OData cast to get only a count of group membership</span></span>

#### <a name="request"></a><span data-ttu-id="93d3b-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="93d3b-159">Request</span></span>

<span data-ttu-id="93d3b-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="93d3b-160">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{id}/memberOf/microsoft.graph.group/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="93d3b-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="93d3b-161">Response</span></span>

<span data-ttu-id="93d3b-162">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="93d3b-162">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain

16
```

### <a name="example-4-use-search-and-odata-cast-to-get-membership-in-groups-with-display-names-that-contain-the-letters-tier-including-a-count-of-returned-objects"></a><span data-ttu-id="93d3b-163">Пример 4. Использование параметра $search и приведения к OData для получения участия пользователей в группах с отображаемыми именами, содержащими буквы «tier», включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="93d3b-163">Example 4: Use $search and OData cast to get membership in groups with display names that contain the letters 'tier' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="93d3b-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="93d3b-164">Request</span></span>

<span data-ttu-id="93d3b-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="93d3b-165">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_tier_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{id}/memberOf/microsoft.graph.group?$count=true&$orderby=displayName&$search="displayName:tier"&$select=displayName,id
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="93d3b-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="93d3b-166">Response</span></span>

<span data-ttu-id="93d3b-167">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="93d3b-167">The following is an example of the response.</span></span>

><span data-ttu-id="93d3b-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="93d3b-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-5-use-filter-and-odata-cast-to-get-groups-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="93d3b-170">Пример 5. Использование параметра $filter и приведения к OData для получения групп с отображаемым именем, которое начинается на «а», включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="93d3b-170">Example 5: Use $filter and OData cast to get groups with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="93d3b-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="93d3b-171">Request</span></span>

<span data-ttu-id="93d3b-172">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="93d3b-172">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{id}/memberOf/microsoft.graph.group?$count=true&$orderby=displayName&$filter=startswith(displayName, 'a') 
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="93d3b-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="93d3b-173">Response</span></span>

<span data-ttu-id="93d3b-174">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="93d3b-174">The following is an example of the response.</span></span>

><span data-ttu-id="93d3b-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="93d3b-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
