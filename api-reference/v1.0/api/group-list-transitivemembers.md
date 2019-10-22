---
title: Список транзитивных членов группы
description: Получение списка членов группы. У группы могут быть пользователи, устройства, организационные контакты и другие группы в качестве участников. Эта операция является транзитивным и возвращает плоский список всех вложенных элементов.
author: anchanda
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 23c051caceff6be68e3b550c06f50c397a5c5d97
ms.sourcegitcommit: c9b9ff2c862f8d96d282a7bdf641cdb9c53a4600
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2019
ms.locfileid: "37621647"
---
# <a name="list-group-transitive-members"></a><span data-ttu-id="742d5-105">Список транзитивных членов группы</span><span class="sxs-lookup"><span data-stu-id="742d5-105">List group transitive members</span></span>

<span data-ttu-id="742d5-106">Получение списка членов группы.</span><span class="sxs-lookup"><span data-stu-id="742d5-106">Get a list of the group's members.</span></span> <span data-ttu-id="742d5-107">У группы могут быть пользователи, устройства, организационные контакты и другие группы в качестве участников.</span><span class="sxs-lookup"><span data-stu-id="742d5-107">A group can have users, devices, organizational contacts, and other groups as members.</span></span> <span data-ttu-id="742d5-108">Эта операция является транзитивным и возвращает плоский список всех вложенных элементов.</span><span class="sxs-lookup"><span data-stu-id="742d5-108">This operation is transitive and returns a flat list of all nested members.</span></span>

## <a name="permissions"></a><span data-ttu-id="742d5-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="742d5-109">Permissions</span></span>

<span data-ttu-id="742d5-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="742d5-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="742d5-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="742d5-112">Permission type</span></span>      | <span data-ttu-id="742d5-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="742d5-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="742d5-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="742d5-114">Delegated (work or school account)</span></span> | <span data-ttu-id="742d5-115">Directory. Read. ALL, Directory. AccessAsUser. ALL, User. ReadBasic. ALL, User. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="742d5-115">Directory.Read.All, Directory.AccessAsUser.All, User.ReadBasic.All, User.Read.All</span></span>    |
|<span data-ttu-id="742d5-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="742d5-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="742d5-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="742d5-117">Not supported.</span></span>    |
|<span data-ttu-id="742d5-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="742d5-118">Application</span></span> | <span data-ttu-id="742d5-119">Directory. Read. ALL, User. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="742d5-119">Directory.Read.All, User.Read.All</span></span> |

><span data-ttu-id="742d5-120">**Примечание:** Чтобы получить список членов скрытой группы членства, требуется разрешение Member. Read. Hidden.</span><span class="sxs-lookup"><span data-stu-id="742d5-120">**Note:** To list the members of a hidden membership group, the Member.Read.Hidden permission is required.</span></span>

## <a name="http-request"></a><span data-ttu-id="742d5-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="742d5-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /groups/{id}/transitiveMembers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="742d5-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="742d5-122">Optional query parameters</span></span>

<span data-ttu-id="742d5-123">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="742d5-123">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="742d5-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="742d5-124">Request headers</span></span>

| <span data-ttu-id="742d5-125">Заголовок</span><span class="sxs-lookup"><span data-stu-id="742d5-125">Header</span></span>       | <span data-ttu-id="742d5-126">Значение</span><span class="sxs-lookup"><span data-stu-id="742d5-126">Value</span></span> |
|:-----------|:----------|
| <span data-ttu-id="742d5-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="742d5-127">Authorization</span></span>  | <span data-ttu-id="742d5-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="742d5-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="742d5-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="742d5-130">Request body</span></span>

<span data-ttu-id="742d5-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="742d5-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="742d5-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="742d5-132">Response</span></span>

<span data-ttu-id="742d5-133">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="742d5-133">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="742d5-134">Пример</span><span class="sxs-lookup"><span data-stu-id="742d5-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="742d5-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="742d5-135">Request</span></span>

<span data-ttu-id="742d5-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="742d5-136">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="742d5-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="742d5-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_transitivemembers"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/transitiveMembers
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="742d5-138">C#</span><span class="sxs-lookup"><span data-stu-id="742d5-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-transitivemembers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="742d5-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="742d5-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-transitivemembers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="742d5-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="742d5-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-transitivemembers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="742d5-141">Java</span><span class="sxs-lookup"><span data-stu-id="742d5-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-transitivemembers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="742d5-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="742d5-142">Response</span></span>

<span data-ttu-id="742d5-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="742d5-143">The following is an example of the response.</span></span>
><span data-ttu-id="742d5-144">**Note**: объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="742d5-144">**Note**: The response object shown here might be shortened for readability.</span></span> 
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
