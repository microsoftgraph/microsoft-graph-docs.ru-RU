---
title: Получение руководителя
description: Получение руководителя пользователя. Возвращает пользователя или контакт, назначенный в качестве руководителя пользователя.
localization_priority: Normal
author: krbain
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 1f04dc23b777906a3ee36bbcefea035e1e8d2422
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49524446"
---
# <a name="list-manager"></a><span data-ttu-id="df766-104">Получение руководителя</span><span class="sxs-lookup"><span data-stu-id="df766-104">List manager</span></span>

<span data-ttu-id="df766-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="df766-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="df766-106">Возвращает пользователя или контакт организации, назначенный в качестве руководителя пользователя.</span><span class="sxs-lookup"><span data-stu-id="df766-106">Returns the user or organizational contact assigned as the user's manager.</span></span> <span data-ttu-id="df766-107">Кроме того, вы можете развернуть цепочку руководителя вплоть до корневого узла.</span><span class="sxs-lookup"><span data-stu-id="df766-107">Optionally, you can expand the manager's chain up to the root node.</span></span>

## <a name="permissions"></a><span data-ttu-id="df766-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="df766-108">Permissions</span></span>

<span data-ttu-id="df766-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="df766-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="df766-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="df766-111">Permission type</span></span>      | <span data-ttu-id="df766-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="df766-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="df766-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="df766-113">Delegated (work or school account)</span></span> | <span data-ttu-id="df766-114">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="df766-114">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="df766-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="df766-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="df766-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="df766-116">Not supported.</span></span>    |
|<span data-ttu-id="df766-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="df766-117">Application</span></span> | <span data-ttu-id="df766-118">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df766-118">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="df766-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="df766-119">HTTP request</span></span>

<span data-ttu-id="df766-120">Получение руководителя:</span><span class="sxs-lookup"><span data-stu-id="df766-120">Get the manager:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/manager
GET /users/{id | userPrincipalName}/manager
```
<span data-ttu-id="df766-121">Получение цепочки управления:</span><span class="sxs-lookup"><span data-stu-id="df766-121">Get the management chain:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me?$expand=manager
GET /users?$expand=manager($levels=n)
GET /users/{id | userPrincipalName}/?$expand=manager($levels=n)
```

## <a name="optional-query-parameters"></a><span data-ttu-id="df766-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="df766-122">Optional query parameters</span></span>

<span data-ttu-id="df766-123">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="df766-123">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>  

<span data-ttu-id="df766-124">Если запрос содержит `$expand=manager($levels=n)` параметр для получения цепочки руководителя, необходимо также указать следующее:</span><span class="sxs-lookup"><span data-stu-id="df766-124">If your request includes the `$expand=manager($levels=n)` parameter to get the manager's chain, you must also include the following:</span></span>

- <span data-ttu-id="df766-125">`$count=true` параметр строки запроса</span><span class="sxs-lookup"><span data-stu-id="df766-125">`$count=true` query string parameter</span></span>
- <span data-ttu-id="df766-126">`ConsistencyLevel=eventual` заголовок запроса</span><span class="sxs-lookup"><span data-stu-id="df766-126">`ConsistencyLevel=eventual` request header</span></span>

><span data-ttu-id="df766-127">**Note:** `n` значение `$levels` может быть `max` (для возврата всех руководителей) или число от 1 до 1000.</span><span class="sxs-lookup"><span data-stu-id="df766-127">**Note:** the `n` value of `$levels` can be `max` (to return all managers) or a number between 1 and 1000.</span></span>  
> <span data-ttu-id="df766-128">Если `$level` параметр не указан, возвращается только диспетчер immediate.</span><span class="sxs-lookup"><span data-stu-id="df766-128">When the `$level` parameter is not specified, only the immediate manager is returned.</span></span>  
> <span data-ttu-id="df766-129">Вы можете указать `$select` внутри `$expand` , чтобы выбрать свойства отдельного руководителя: `$expand=manager($levels=max;$select=id,displayName)`</span><span class="sxs-lookup"><span data-stu-id="df766-129">You can specify `$select` inside `$expand` to select the individual manager's properties: `$expand=manager($levels=max;$select=id,displayName)`</span></span>

## <a name="request-headers"></a><span data-ttu-id="df766-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="df766-130">Request headers</span></span>

| <span data-ttu-id="df766-131">Заголовок</span><span class="sxs-lookup"><span data-stu-id="df766-131">Header</span></span>       | <span data-ttu-id="df766-132">Значение</span><span class="sxs-lookup"><span data-stu-id="df766-132">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="df766-133">Авторизация</span><span class="sxs-lookup"><span data-stu-id="df766-133">Authorization</span></span>  | <span data-ttu-id="df766-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="df766-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="df766-136">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="df766-136">ConsistencyLevel</span></span> | <span data-ttu-id="df766-137">необязательный.</span><span class="sxs-lookup"><span data-stu-id="df766-137">eventual.</span></span> <span data-ttu-id="df766-138">Является обязательным, если запрос содержит `$expand=manager($levels=max)` параметр.</span><span class="sxs-lookup"><span data-stu-id="df766-138">Required when the request includes the `$expand=manager($levels=max)` parameter.</span></span> |

## <a name="request-body"></a><span data-ttu-id="df766-139">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="df766-139">Request body</span></span>

<span data-ttu-id="df766-140">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="df766-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="df766-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="df766-141">Response</span></span>

<span data-ttu-id="df766-142">В случае успеха этот метод возвращает код отклика `200 OK` и объект [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="df766-142">If successful, this method returns a `200 OK` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="df766-143">Примеры</span><span class="sxs-lookup"><span data-stu-id="df766-143">Examples</span></span>

### <a name="example-1-get-manager"></a><span data-ttu-id="df766-144">Пример 1: Get Manager</span><span class="sxs-lookup"><span data-stu-id="df766-144">Example 1: Get manager</span></span>

<span data-ttu-id="df766-145">В приведенном ниже примере показан запрос на получение диспетчера.</span><span class="sxs-lookup"><span data-stu-id="df766-145">The following example shows a request to get the manager.</span></span>

#### <a name="request"></a><span data-ttu-id="df766-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="df766-146">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="df766-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="df766-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_manager"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id|userPrincipalName}/manager
```
# <a name="c"></a>[<span data-ttu-id="df766-148">C#</span><span class="sxs-lookup"><span data-stu-id="df766-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-manager-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="df766-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="df766-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-manager-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="df766-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="df766-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-manager-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="df766-151">Java</span><span class="sxs-lookup"><span data-stu-id="df766-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-manager-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="df766-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="df766-152">Response</span></span>

<span data-ttu-id="df766-153">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="df766-153">The following is an example of the response.</span></span>
><span data-ttu-id="df766-154">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="df766-154">**Note**: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "<user-id>",
  "displayName": "Sara Davis",
  "jobTitle": "Finance VP",
  "mail": "SaraD@contoso.onmicrosoft.com",
  "userPrincipalName": "SaraD@contoso.onmicrosoft.com"
}
```

### <a name="example-2-get-manager-chain-up-to-the-root-level"></a><span data-ttu-id="df766-155">Пример 2: получение цепочки диспетчера вплоть до корневого уровня</span><span class="sxs-lookup"><span data-stu-id="df766-155">Example 2: Get manager chain up to the root level</span></span>

<span data-ttu-id="df766-156">В приведенном ниже примере показан запрос на получение цепочки диспетчера до корневого уровня.</span><span class="sxs-lookup"><span data-stu-id="df766-156">The following example shows a request to get the manager chain up to the root level.</span></span>

#### <a name="request"></a><span data-ttu-id="df766-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="df766-157">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_transitive_managers"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me?$expand=manager($levels=max;$select=id,displayName)&$select=id,displayName&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="df766-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="df766-158">Response</span></span>

<span data-ttu-id="df766-159">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="df766-159">The following is an example of the response.</span></span> <span data-ttu-id="df766-160">Транзитивные руководители отображаются в иерархическом порядке.</span><span class="sxs-lookup"><span data-stu-id="df766-160">Transitive managers are displayed hierarchically.</span></span>

><span data-ttu-id="df766-161">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="df766-161">**Note**: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "<user1-id>",
    "displayName": "Individual Contributor",
    "manager": {
        "id": "<manager1-id>",
        "displayName": "Manager 1",
        "manager": {
            "id": "<manager2-id>",
            "displayName": "Manager 2",
            "manager": {
                "id": "<manager3-id>",
                "displayName": "Manager 3"
            }
        }
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List directReports",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
