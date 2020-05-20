---
title: Список транзитивных членов группы
description: Получение списка членов группы. У группы могут быть пользователи, устройства, организационные контакты и другие группы в качестве участников. Эта операция является транзитивным и возвращает плоский список всех вложенных элементов.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: e1c4ec7765f40e2867ea39f8d5de4cc6cbd2bd4b
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2020
ms.locfileid: "44289427"
---
# <a name="list-group-transitive-members"></a><span data-ttu-id="ea370-105">Список транзитивных членов группы</span><span class="sxs-lookup"><span data-stu-id="ea370-105">List group transitive members</span></span>

<span data-ttu-id="ea370-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ea370-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ea370-107">Получение списка членов группы.</span><span class="sxs-lookup"><span data-stu-id="ea370-107">Get a list of the group's members.</span></span> <span data-ttu-id="ea370-108">У группы могут быть пользователи, устройства, организационные контакты и другие группы в качестве участников.</span><span class="sxs-lookup"><span data-stu-id="ea370-108">A group can have users, devices, organizational contacts, and other groups as members.</span></span> <span data-ttu-id="ea370-109">Эта операция является транзитивным и возвращает плоский список всех вложенных элементов.</span><span class="sxs-lookup"><span data-stu-id="ea370-109">This operation is transitive and returns a flat list of all nested members.</span></span>

## <a name="permissions"></a><span data-ttu-id="ea370-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ea370-110">Permissions</span></span>

<span data-ttu-id="ea370-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ea370-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea370-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ea370-113">Permission type</span></span>      | <span data-ttu-id="ea370-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ea370-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ea370-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ea370-115">Delegated (work or school account)</span></span> | <span data-ttu-id="ea370-116">Directory. Read. ALL, Directory. AccessAsUser. ALL, User. ReadBasic. ALL, User. Read. ALL, Application. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="ea370-116">Directory.Read.All, Directory.AccessAsUser.All, User.ReadBasic.All, User.Read.All, Application.Read.All</span></span>  |
|<span data-ttu-id="ea370-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ea370-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ea370-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea370-118">Not supported.</span></span>    |
|<span data-ttu-id="ea370-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ea370-119">Application</span></span> | <span data-ttu-id="ea370-120">Directory. Read. ALL, User. Read. ALL, Application. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="ea370-120">Directory.Read.All, User.Read.All, Application.Read.All</span></span> |

><span data-ttu-id="ea370-121">**Примечание:** Чтобы получить список членов скрытой группы членства, требуется разрешение Member. Read. Hidden.</span><span class="sxs-lookup"><span data-stu-id="ea370-121">**Note:** To list the members of a hidden membership group, the Member.Read.Hidden permission is required.</span></span>

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="ea370-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ea370-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /groups/{id}/transitiveMembers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ea370-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ea370-123">Optional query parameters</span></span>

<span data-ttu-id="ea370-124">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="ea370-124">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ea370-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ea370-125">Request headers</span></span>

| <span data-ttu-id="ea370-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ea370-126">Header</span></span>       | <span data-ttu-id="ea370-127">Значение</span><span class="sxs-lookup"><span data-stu-id="ea370-127">Value</span></span> |
|:-----------|:----------|
| <span data-ttu-id="ea370-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ea370-128">Authorization</span></span>  | <span data-ttu-id="ea370-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ea370-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ea370-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ea370-131">Request body</span></span>

<span data-ttu-id="ea370-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ea370-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ea370-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="ea370-133">Response</span></span>

<span data-ttu-id="ea370-134">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ea370-134">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea370-135">Пример</span><span class="sxs-lookup"><span data-stu-id="ea370-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="ea370-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="ea370-136">Request</span></span>

<span data-ttu-id="ea370-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ea370-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ea370-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="ea370-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_transitivemembers"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/transitiveMembers
```
# <a name="c"></a>[<span data-ttu-id="ea370-139">C#</span><span class="sxs-lookup"><span data-stu-id="ea370-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-transitivemembers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ea370-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ea370-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-transitivemembers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ea370-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ea370-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-transitivemembers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ea370-142">Java</span><span class="sxs-lookup"><span data-stu-id="ea370-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-transitivemembers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ea370-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="ea370-143">Response</span></span>

<span data-ttu-id="ea370-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ea370-144">The following is an example of the response.</span></span>
><span data-ttu-id="ea370-145">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ea370-145">**Note**: The response object shown here might be shortened for readability.</span></span> 
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
      "businessPhones": [
        "businessPhones-value"
      ],
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "jobTitle": "jobTitle-value",
      "mail": "mail-value",
      "mobilePhone": "mobilePhone-value",
      "officeLocation": "officeLocation-value",
      "preferredLanguage": "preferredLanguage-value",
      "surname": "surname-value",
      "userPrincipalName": "userPrincipalName-value",
      "id": "id-value"
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
