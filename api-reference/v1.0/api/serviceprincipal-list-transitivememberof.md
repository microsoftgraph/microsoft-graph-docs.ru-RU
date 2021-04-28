---
title: Перечисление servicePrincipal transitive memberOf
description: Список групп и ролей каталога, участником которых является этот субъект-служба.
localization_priority: Priority
doc_type: apiPageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: b317c33f1c7f522fdee7e5b71eed63efa68a9852
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053820"
---
# <a name="list-serviceprincipal-transitive-memberof"></a><span data-ttu-id="56858-103">Перечисление servicePrincipal transitive memberOf</span><span class="sxs-lookup"><span data-stu-id="56858-103">List servicePrincipal transitive memberOf</span></span>

<span data-ttu-id="56858-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="56858-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="56858-105">Список групп и ролей каталога, участником которых является этот [субъект-служба](../resources/serviceprincipal.md).</span><span class="sxs-lookup"><span data-stu-id="56858-105">Get the groups and directory roles that this [servicePrincipal](../resources/serviceprincipal.md) is a member of.</span></span> <span data-ttu-id="56858-106">Эта операция является транзитивной и включает все группы, в которых состоит субъект-служба.</span><span class="sxs-lookup"><span data-stu-id="56858-106">This operation is transitive and will include all groups that this service principal is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="56858-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="56858-107">Permissions</span></span>
<span data-ttu-id="56858-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="56858-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56858-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="56858-110">Permission type</span></span>      | <span data-ttu-id="56858-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="56858-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="56858-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="56858-112">Delegated (work or school account)</span></span> | <span data-ttu-id="56858-113">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="56858-113">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="56858-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="56858-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="56858-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="56858-115">Not supported.</span></span>    |
|<span data-ttu-id="56858-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="56858-116">Application</span></span> | <span data-ttu-id="56858-117">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56858-117">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="56858-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="56858-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/transitiveMemberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="56858-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="56858-119">Optional query parameters</span></span>

<span data-ttu-id="56858-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа, в том числе `$search`, `$count` і `$filter`.</span><span class="sxs-lookup"><span data-stu-id="56858-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="56858-121">Кроме того, включено также приведение к OData, например, вы можете получить только directoryRoles, участником которых является пользователь.</span><span class="sxs-lookup"><span data-stu-id="56858-121">OData cast is also enabled, for example, you can cast to get just the directoryRoles the user is a member of.</span></span> <span data-ttu-id="56858-122">Вы можете использовать `$search` в свойствах **displayName** и **description**.</span><span class="sxs-lookup"><span data-stu-id="56858-122">You can use `$search` on the **displayName** and **description** properties.</span></span> <span data-ttu-id="56858-123">Когда элементы добавляются или обновляются для этого ресурса, они специально индексируются для использования с помощью параметров `$count` и `$search`.</span><span class="sxs-lookup"><span data-stu-id="56858-123">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="56858-124">Между добавлением или обновлением элемента и его появлением в индексе может возникать небольшая задержка.</span><span class="sxs-lookup"><span data-stu-id="56858-124">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="56858-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="56858-125">Request headers</span></span>
| <span data-ttu-id="56858-126">Имя</span><span class="sxs-lookup"><span data-stu-id="56858-126">Name</span></span>           | <span data-ttu-id="56858-127">Описание</span><span class="sxs-lookup"><span data-stu-id="56858-127">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="56858-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="56858-128">Authorization</span></span>  | <span data-ttu-id="56858-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="56858-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="56858-131">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="56858-131">ConsistencyLevel</span></span> | <span data-ttu-id="56858-132">необязательный.</span><span class="sxs-lookup"><span data-stu-id="56858-132">eventual.</span></span> <span data-ttu-id="56858-133">Этот заголовок и `$count` требуются при использовании `$search`, `$filter`, `$orderby` или с параметрами запросов OData cast.</span><span class="sxs-lookup"><span data-stu-id="56858-133">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="56858-134">В нем используется индекс, который может не соответствовать последним изменениям объекта.</span><span class="sxs-lookup"><span data-stu-id="56858-134">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="56858-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="56858-135">Request body</span></span>
<span data-ttu-id="56858-136">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="56858-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="56858-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="56858-137">Response</span></span>

<span data-ttu-id="56858-138">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="56858-138">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="56858-139">Примеры</span><span class="sxs-lookup"><span data-stu-id="56858-139">Examples</span></span>

### <a name="example-1-get-groups-and-directory-roles-that-the-service-principal-is-a-transitive-member-of"></a><span data-ttu-id="56858-140">Пример 1: Список групп и ролей каталога, транзитивным участником которых является этот субъект-служба</span><span class="sxs-lookup"><span data-stu-id="56858-140">Example 1: Get groups and directory roles that the service principal is a transitive member of</span></span>

#### <a name="request"></a><span data-ttu-id="56858-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="56858-141">Request</span></span>

<span data-ttu-id="56858-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="56858-142">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="56858-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="56858-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_serviceprincipal_tranitivememberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals/{id}/transitiveMemberOf
```
# <a name="c"></a>[<span data-ttu-id="56858-144">C#</span><span class="sxs-lookup"><span data-stu-id="56858-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-serviceprincipal-tranitivememberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="56858-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="56858-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-serviceprincipal-tranitivememberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="56858-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="56858-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-serviceprincipal-tranitivememberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="56858-147">Java</span><span class="sxs-lookup"><span data-stu-id="56858-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-serviceprincipal-tranitivememberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="56858-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="56858-148">Response</span></span>

<span data-ttu-id="56858-149">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="56858-149">The following is an example of the response.</span></span> 

> <span data-ttu-id="56858-150">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="56858-150">**Note:** The response object shown here might be shortened for readability.</span></span>

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
      "id": "id-value",
      "createdDateTime": null,
      "description": "All users at the company",
      "displayName": "All Users",
      "groupTypes": [],
      "mailEnabled": false,
      "securityEnabled": true,
    }
  ]
}
```

### <a name="example-2-get-only-a-count-of-all-transitive-membership"></a><span data-ttu-id="56858-151">Пример 2: Получение только количества транзитивных участников</span><span class="sxs-lookup"><span data-stu-id="56858-151">Example 2: Get only a count of all transitive membership</span></span>

#### <a name="request"></a><span data-ttu-id="56858-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="56858-152">Request</span></span>

<span data-ttu-id="56858-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="56858-153">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals/{id}/transitiveMemberOf/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="56858-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="56858-154">Response</span></span>

<span data-ttu-id="56858-155">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="56858-155">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

`294`

### <a name="example-3-use-odata-cast-to-get-only-a-count-of-transitive-membership-in-groups"></a><span data-ttu-id="56858-156">Пример 3. Использование OData cast для получения только количества транзитивных участников в группах</span><span class="sxs-lookup"><span data-stu-id="56858-156">Example 3: Use OData cast to get only a count of transitive membership in groups</span></span>

#### <a name="request"></a><span data-ttu-id="56858-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="56858-157">Request</span></span>

<span data-ttu-id="56858-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="56858-158">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals/{id}/transitiveMemberOf/microsoft.graph.group/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="56858-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="56858-159">Response</span></span>

<span data-ttu-id="56858-160">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="56858-160">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

`294`

### <a name="example-4-use-search-and-odata-cast-to-get-group-membership-with-display-names-that-contain-the-letters-video-including-a-count-of-returned-objects"></a><span data-ttu-id="56858-161">Пример 4: Использование параметра $search и OData cast для получения участия в группах с отображаемыми именами, содержащими буквы "Video", включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="56858-161">Example 4: Use $search and OData cast to get group membership with display names that contain the letters 'Video' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="56858-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="56858-162">Request</span></span>

<span data-ttu-id="56858-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="56858-163">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_tier_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderby=displayName&$search="displayName:Video"&$select=displayName,id
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="56858-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="56858-164">Response</span></span>

<span data-ttu-id="56858-165">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="56858-165">The following is an example of the response.</span></span>

><span data-ttu-id="56858-166">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="56858-166">**Note:** The response object shown here might be shortened for readability.</span></span>

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
      "displayName":"Contoso Videos",
      "id":"11111111-2222-3333-4444-555555555555"
    }
  ]
}
```

### <a name="example-5-use-filter-and-odata-cast-to-get-group-membership-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="56858-167">Пример 5: Использование параметра $search и OData cast для получения участия в группах с отображаемым именем, которое начинается на «а», включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="56858-167">Example 5: Use $filter and OData cast to get group membership with a display name that starts with 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="56858-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="56858-168">Request</span></span>

<span data-ttu-id="56858-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="56858-169">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderby=displayName&$filter=startswith(displayName, 'a')
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="56858-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="56858-170">Response</span></span>

<span data-ttu-id="56858-171">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="56858-171">The following is an example of the response.</span></span>

><span data-ttu-id="56858-172">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="56858-172">**Note:** The response object shown here might be shortened for readability.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "List servicePrincipal memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
