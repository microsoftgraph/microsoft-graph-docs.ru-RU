---
title: Перечисление user transitive memberOf
description: Получение групп, ролей каталогов, участником которых является пользователь. Этот запрос API является транзитивным и также возвращает все группы, в которых пользователь является вложенным.
author: krbain
localization_priority: Normal
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: dc536c49c02d88827ccae633cd018cd2c5ff7d29
ms.sourcegitcommit: 577bfd3bb8a2e2679ef1c5942a4a496c2aa3a277
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/17/2020
ms.locfileid: "48582074"
---
# <a name="list-user-transitive-memberof"></a><span data-ttu-id="dda8d-104">Перечисление user transitive memberOf</span><span class="sxs-lookup"><span data-stu-id="dda8d-104">List user transitive memberOf</span></span>

<span data-ttu-id="dda8d-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dda8d-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="dda8d-106">Получение групп, ролей каталогов, участником которых является пользователь.</span><span class="sxs-lookup"><span data-stu-id="dda8d-106">Get groups, directory roles that the user is a member of.</span></span> <span data-ttu-id="dda8d-107">Этот запрос API является транзитивным и также возвращает все группы, в которых пользователь является вложенным.</span><span class="sxs-lookup"><span data-stu-id="dda8d-107">This API request is transitive, and will also return all groups the user is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="dda8d-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dda8d-108">Permissions</span></span>

<span data-ttu-id="dda8d-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dda8d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dda8d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dda8d-111">Permission type</span></span>      | <span data-ttu-id="dda8d-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dda8d-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dda8d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dda8d-113">Delegated (work or school account)</span></span> | <span data-ttu-id="dda8d-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="dda8d-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="dda8d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dda8d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dda8d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dda8d-116">Not supported.</span></span>    |
|<span data-ttu-id="dda8d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dda8d-117">Application</span></span> | <span data-ttu-id="dda8d-118">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dda8d-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="dda8d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dda8d-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /users/{id | userPrincipalName}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dda8d-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="dda8d-120">Optional query parameters</span></span>

<span data-ttu-id="dda8d-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="dda8d-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dda8d-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dda8d-122">Request headers</span></span>

| <span data-ttu-id="dda8d-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dda8d-123">Header</span></span>       | <span data-ttu-id="dda8d-124">Значение</span><span class="sxs-lookup"><span data-stu-id="dda8d-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="dda8d-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dda8d-125">Authorization</span></span>  | <span data-ttu-id="dda8d-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dda8d-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="dda8d-128">Accept</span><span class="sxs-lookup"><span data-stu-id="dda8d-128">Accept</span></span>  | <span data-ttu-id="dda8d-129">application/json</span><span class="sxs-lookup"><span data-stu-id="dda8d-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dda8d-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dda8d-130">Request body</span></span>

<span data-ttu-id="dda8d-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dda8d-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dda8d-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="dda8d-132">Response</span></span>

<span data-ttu-id="dda8d-133">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="dda8d-133">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dda8d-134">Пример</span><span class="sxs-lookup"><span data-stu-id="dda8d-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="dda8d-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="dda8d-135">Request</span></span>

<span data-ttu-id="dda8d-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dda8d-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="dda8d-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="dda8d-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_transitivememberof"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/transitiveMemberOf
```
# <a name="c"></a>[<span data-ttu-id="dda8d-138">C#</span><span class="sxs-lookup"><span data-stu-id="dda8d-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-transitivememberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dda8d-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dda8d-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-transitivememberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dda8d-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dda8d-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-transitivememberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dda8d-141">Java</span><span class="sxs-lookup"><span data-stu-id="dda8d-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-transitivememberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="dda8d-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="dda8d-142">Response</span></span>

<span data-ttu-id="dda8d-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dda8d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List transitiveMsemberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->