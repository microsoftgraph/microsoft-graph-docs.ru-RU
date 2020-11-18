---
title: Список memberOf
description: 'Получение групп и ролей каталога, непосредственным участником которых является пользователь. '
author: krbain
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: ee2290f6dd850fc198bcc5edf478ff06091e80c9
ms.sourcegitcommit: 186d738f04e5a558da423f2429165fb4fbe780aa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086776"
---
# <a name="list-memberof"></a><span data-ttu-id="fc346-103">Список memberOf</span><span class="sxs-lookup"><span data-stu-id="fc346-103">List memberOf</span></span>

<span data-ttu-id="fc346-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fc346-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fc346-105">Получение [групп](../resources/group.md) и [ролей каталога](../resources/directoryrole.md), непосредственным членом которых является пользователь.</span><span class="sxs-lookup"><span data-stu-id="fc346-105">Get [groups](../resources/group.md) and [directory roles](../resources/directoryrole.md) that the user is a direct member of.</span></span> 

## <a name="permissions"></a><span data-ttu-id="fc346-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fc346-106">Permissions</span></span>
<span data-ttu-id="fc346-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc346-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc346-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fc346-109">Permission type</span></span>      | <span data-ttu-id="fc346-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fc346-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fc346-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fc346-111">Delegated (work or school account)</span></span> | <span data-ttu-id="fc346-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fc346-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="fc346-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fc346-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fc346-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc346-114">Not supported.</span></span>    |
|<span data-ttu-id="fc346-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fc346-115">Application</span></span> | <span data-ttu-id="fc346-116">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc346-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="fc346-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fc346-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/memberOf
GET /users/{id | userPrincipalName}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="fc346-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="fc346-118">Optional query parameters</span></span>

<span data-ttu-id="fc346-p102">Этот метод поддерживает [параметры запроса OData](/graph/query-parameters) для настройки отклика, в том числе `$search`, `$count` и `$filter`. Также включено приведение к OData, например, вы можете получить только directoryRoles, участником которых является пользователь. Вы можете использовать параметр `$search` в свойстве **displayName**. При добавлении или обновлении элементов для этого ресурса они индексируются для использования с параметрами запроса `$count` и `$search`. Между добавлением или обновлением элемента и его появлением в индексе может возникать небольшая задержка.</span><span class="sxs-lookup"><span data-stu-id="fc346-p102">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`. OData cast is also enabled, for example, you can cast to get just the directoryRoles the user is a member of. You can use `$search` on the **displayName** property. When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters. There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="fc346-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fc346-124">Request headers</span></span>
| <span data-ttu-id="fc346-125">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fc346-125">Header</span></span>       | <span data-ttu-id="fc346-126">Значение</span><span class="sxs-lookup"><span data-stu-id="fc346-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fc346-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fc346-127">Authorization</span></span>  | <span data-ttu-id="fc346-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fc346-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="fc346-130">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="fc346-130">ConsistencyLevel</span></span> | <span data-ttu-id="fc346-p104">необязательный. Этот заголовок и `$count` требуются при использовании `$search`, `$filter`, `$orderby` или параметров запросов для преобразования OData. В нем используется индекс, который может не соответствовать последним изменениям объекта.</span><span class="sxs-lookup"><span data-stu-id="fc346-p104">eventual. This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters. It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fc346-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fc346-134">Request body</span></span>
<span data-ttu-id="fc346-135">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fc346-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fc346-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="fc346-136">Response</span></span>

<span data-ttu-id="fc346-137">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fc346-137">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fc346-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="fc346-138">Examples</span></span>

### <a name="example-1-get-groups-directory-roles-and-administrative-units-that-the-user-is-a-direct-member-of"></a><span data-ttu-id="fc346-139">Пример 1. Получение групп, ролей каталогов и административных единиц, непосредственным участником которых является пользователь.</span><span class="sxs-lookup"><span data-stu-id="fc346-139">Example 1: Get groups, directory roles, and administrative units that the user is a direct member of</span></span>

#### <a name="request"></a><span data-ttu-id="fc346-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="fc346-140">Request</span></span>

<span data-ttu-id="fc346-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fc346-141">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="fc346-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="fc346-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_get_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{id}/memberOf
```
# <a name="c"></a>[<span data-ttu-id="fc346-143">C#</span><span class="sxs-lookup"><span data-stu-id="fc346-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-get-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fc346-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fc346-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-get-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fc346-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fc346-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-get-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fc346-146">Java</span><span class="sxs-lookup"><span data-stu-id="fc346-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-get-memberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="fc346-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="fc346-147">Response</span></span>

<span data-ttu-id="fc346-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fc346-148">The following is an example of the response.</span></span>

><span data-ttu-id="fc346-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fc346-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-only-a-count-of-all-groups-directory-roles-and-administrative-units-that-the-user-is-a-direct-member-of"></a><span data-ttu-id="fc346-151">Пример 2. Получение только количества всех групп, ролей каталогов и административных единиц, непосредственным участником которых является пользователь.</span><span class="sxs-lookup"><span data-stu-id="fc346-151">Example 2: Get only a count of all groups, directory roles, and administrative units that the user is a direct member of</span></span>

#### <a name="request"></a><span data-ttu-id="fc346-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="fc346-152">Request</span></span>

<span data-ttu-id="fc346-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fc346-153">Here is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_user_memberof_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{id}/memberOf/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="fc346-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="fc346-154">Response</span></span>

<span data-ttu-id="fc346-155">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fc346-155">The following is an example of the response.</span></span>

><span data-ttu-id="fc346-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fc346-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

### <a name="example-3-use-odata-cast-to-get-only-a-count-of-group-membership"></a><span data-ttu-id="fc346-158">Пример 3. Использование OData cast для получения только количества участия в группах</span><span class="sxs-lookup"><span data-stu-id="fc346-158">Example 3: Use OData cast to get only a count of group membership</span></span>

#### <a name="request"></a><span data-ttu-id="fc346-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="fc346-159">Request</span></span>

<span data-ttu-id="fc346-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fc346-160">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{id}/memberOf/microsoft.graph.group/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="fc346-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="fc346-161">Response</span></span>

<span data-ttu-id="fc346-162">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fc346-162">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

### <a name="example-4-use-search-and-odata-cast-to-get-membership-in-groups-with-display-names-that-contain-the-letters-tier-including-a-count-of-returned-objects"></a><span data-ttu-id="fc346-163">Пример 4. Использование параметра $search и приведения к OData для получения участия пользователей в группах с отображаемыми именами, содержащими буквы «tier», включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="fc346-163">Example 4: Use $search and OData cast to get membership in groups with display names that contain the letters 'tier' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="fc346-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="fc346-164">Request</span></span>

<span data-ttu-id="fc346-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fc346-165">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_tier_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{id}/memberOf/microsoft.graph.group?$count=true&$orderby=displayName&$search="displayName:tier"&$select=displayName,id
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="fc346-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="fc346-166">Response</span></span>

<span data-ttu-id="fc346-167">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fc346-167">The following is an example of the response.</span></span>

><span data-ttu-id="fc346-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fc346-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-5-use-filter-and-odata-cast-to-get-groups-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="fc346-170">Пример 5. Использование параметра $filter и приведения к OData для получения групп с отображаемым именем, которое начинается на «а», включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="fc346-170">Example 5: Use $filter and OData cast to get groups with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="fc346-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="fc346-171">Request</span></span>

<span data-ttu-id="fc346-172">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fc346-172">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{id}/memberOf/microsoft.graph.group?$count=true&$orderby=displayName&$filter=startswith(displayName, 'a') 
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="fc346-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="fc346-173">Response</span></span>

<span data-ttu-id="fc346-174">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fc346-174">The following is an example of the response.</span></span>

><span data-ttu-id="fc346-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fc346-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
