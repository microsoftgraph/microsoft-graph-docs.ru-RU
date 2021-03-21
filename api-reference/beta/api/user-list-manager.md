---
title: Получение руководителя
description: Получение руководителя пользователя. Возвращает пользователя или контакт, назначенный в качестве руководителя пользователя.
localization_priority: Normal
author: jpettere
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 33865876b1750c13c6f2eec77aa09f4fa57191d2
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50957129"
---
# <a name="list-manager"></a><span data-ttu-id="1c5df-104">Получение руководителя</span><span class="sxs-lookup"><span data-stu-id="1c5df-104">List manager</span></span>

<span data-ttu-id="1c5df-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1c5df-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1c5df-106">Возвращает пользователя или контакт организации, назначенный в качестве руководителя пользователя.</span><span class="sxs-lookup"><span data-stu-id="1c5df-106">Returns the user or organizational contact assigned as the user's manager.</span></span> <span data-ttu-id="1c5df-107">Кроме того, вы можете развернуть цепочку руководителей до корневого узла.</span><span class="sxs-lookup"><span data-stu-id="1c5df-107">Optionally, you can expand the manager's chain up to the root node.</span></span>

## <a name="permissions"></a><span data-ttu-id="1c5df-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1c5df-108">Permissions</span></span>

<span data-ttu-id="1c5df-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c5df-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c5df-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1c5df-111">Permission type</span></span>      | <span data-ttu-id="1c5df-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1c5df-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1c5df-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1c5df-113">Delegated (work or school account)</span></span> | <span data-ttu-id="1c5df-114">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1c5df-114">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1c5df-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1c5df-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1c5df-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1c5df-116">Not supported.</span></span>    |
|<span data-ttu-id="1c5df-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1c5df-117">Application</span></span> | <span data-ttu-id="1c5df-118">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c5df-118">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="1c5df-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1c5df-119">HTTP request</span></span>

<span data-ttu-id="1c5df-120">Получение руководителя:</span><span class="sxs-lookup"><span data-stu-id="1c5df-120">Get the manager:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/manager
GET /users/{id | userPrincipalName}/manager
```
<span data-ttu-id="1c5df-121">Получение цепочки управления:</span><span class="sxs-lookup"><span data-stu-id="1c5df-121">Get the management chain:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me?$expand=manager
GET /users?$expand=manager($levels=n)
GET /users/{id | userPrincipalName}/?$expand=manager($levels=n)
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1c5df-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1c5df-122">Optional query parameters</span></span>

<span data-ttu-id="1c5df-123">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$select` и `$expand` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="1c5df-123">This method supports the `$select` and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>  

><span data-ttu-id="1c5df-124">**Примечание:**</span><span class="sxs-lookup"><span data-stu-id="1c5df-124">**Note:**</span></span> 
> + <span data-ttu-id="1c5df-125">Значение может быть (для возврата всех менеджеров) или числом от 1 до `n` `$levels` `max` 1000.</span><span class="sxs-lookup"><span data-stu-id="1c5df-125">The `n` value of `$levels` can be `max` (to return all managers) or a number between 1 and 1000.</span></span>  
> + <span data-ttu-id="1c5df-126">Если параметр `$levels` не указан, возвращается только непосредственный руководитель.</span><span class="sxs-lookup"><span data-stu-id="1c5df-126">When the `$levels` parameter is not specified, only the immediate manager is returned.</span></span>  
> + <span data-ttu-id="1c5df-127">Вы можете `$select` указать внутри, чтобы выбрать свойства `$expand` отдельного менеджера.</span><span class="sxs-lookup"><span data-stu-id="1c5df-127">You can specify `$select` inside `$expand` to select the individual manager's properties.</span></span> <span data-ttu-id="1c5df-128">Параметр `$levels` необходим: `$expand=manager($levels=max;$select=id,displayName)`</span><span class="sxs-lookup"><span data-stu-id="1c5df-128">The `$levels` parameter is required: `$expand=manager($levels=max;$select=id,displayName)`</span></span>

## <a name="request-headers"></a><span data-ttu-id="1c5df-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1c5df-129">Request headers</span></span>

| <span data-ttu-id="1c5df-130">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1c5df-130">Header</span></span>       | <span data-ttu-id="1c5df-131">Значение</span><span class="sxs-lookup"><span data-stu-id="1c5df-131">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="1c5df-132">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1c5df-132">Authorization</span></span>  | <span data-ttu-id="1c5df-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1c5df-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="1c5df-135">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="1c5df-135">ConsistencyLevel</span></span> | <span data-ttu-id="1c5df-136">необязательный.</span><span class="sxs-lookup"><span data-stu-id="1c5df-136">eventual.</span></span> <span data-ttu-id="1c5df-137">Требуется, если запрос содержит параметр `$expand=manager($levels=max)`.</span><span class="sxs-lookup"><span data-stu-id="1c5df-137">Required when the request includes the `$expand=manager($levels=max)` parameter.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1c5df-138">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1c5df-138">Request body</span></span>

<span data-ttu-id="1c5df-139">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1c5df-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1c5df-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="1c5df-140">Response</span></span>

<span data-ttu-id="1c5df-141">В случае успеха этот метод возвращает код отклика `200 OK` и объект [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1c5df-141">If successful, this method returns a `200 OK` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1c5df-142">Примеры</span><span class="sxs-lookup"><span data-stu-id="1c5df-142">Examples</span></span>

### <a name="example-1-get-manager"></a><span data-ttu-id="1c5df-143">Пример 1. Получение руководителя</span><span class="sxs-lookup"><span data-stu-id="1c5df-143">Example 1: Get manager</span></span>

<span data-ttu-id="1c5df-144">Ниже показан пример запроса для получения руководителя.</span><span class="sxs-lookup"><span data-stu-id="1c5df-144">The following example shows a request to get the manager.</span></span>

#### <a name="request"></a><span data-ttu-id="1c5df-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="1c5df-145">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="1c5df-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="1c5df-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_manager_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id|userPrincipalName}/manager
```
# <a name="c"></a>[<span data-ttu-id="1c5df-147">C#</span><span class="sxs-lookup"><span data-stu-id="1c5df-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-manager-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1c5df-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1c5df-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-manager-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1c5df-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1c5df-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-manager-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1c5df-150">Java</span><span class="sxs-lookup"><span data-stu-id="1c5df-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-manager-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1c5df-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="1c5df-151">Response</span></span>

<span data-ttu-id="1c5df-152">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1c5df-152">The following is an example of the response.</span></span>
><span data-ttu-id="1c5df-153">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="1c5df-153">**Note**: The response object shown here might be shortened for readability.</span></span>
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

### <a name="example-2-get-manager-chain-up-to-the-root-level"></a><span data-ttu-id="1c5df-154">Пример 2. Получение цепочкой руководителей до корневого уровня</span><span class="sxs-lookup"><span data-stu-id="1c5df-154">Example 2: Get manager chain up to the root level</span></span>

<span data-ttu-id="1c5df-155">Ниже показан пример запроса для получения цепочки руководителей до корневого уровня.</span><span class="sxs-lookup"><span data-stu-id="1c5df-155">The following example shows a request to get the manager chain up to the root level.</span></span>

#### <a name="request"></a><span data-ttu-id="1c5df-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="1c5df-156">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_transitive_managers"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me?$expand=manager($levels=max;$select=id,displayName)&$select=id,displayName&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="1c5df-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="1c5df-157">Response</span></span>

<span data-ttu-id="1c5df-158">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="1c5df-158">The following is an example of the response.</span></span> <span data-ttu-id="1c5df-159">Промежуточные руководители отображаются иерархически.</span><span class="sxs-lookup"><span data-stu-id="1c5df-159">Transitive managers are displayed hierarchically.</span></span>

><span data-ttu-id="1c5df-160">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="1c5df-160">**Note**: The response object shown here might be shortened for readability.</span></span>
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
