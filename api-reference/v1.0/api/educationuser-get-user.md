---
title: Получение educationUser
description: Получение простого каталога **user**, который соответствует этому объекту **educationUser**.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 728e848e07a176ad43e1ddea1edfee3218ae3764
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52231887"
---
# <a name="get-educationuser"></a><span data-ttu-id="f4a02-103">Получение educationUser</span><span class="sxs-lookup"><span data-stu-id="f4a02-103">Get educationUser</span></span>

<span data-ttu-id="f4a02-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4a02-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f4a02-105">Получение простого каталога **user**, который соответствует этому объекту **educationUser**.</span><span class="sxs-lookup"><span data-stu-id="f4a02-105">Retrieve the simple directory **user** that corresponds to this **educationUser**.</span></span>

><span data-ttu-id="f4a02-106">**Примечание.** Если используется делегированный маркер, участники могут видеть сведения только о своих учебных заведениях.</span><span class="sxs-lookup"><span data-stu-id="f4a02-106">**Note:** If the delegated token is used, members can only see information about their own schools.</span></span> <span data-ttu-id="f4a02-107">В данном случае используйте ресурс `...beta/education/me/schools`.</span><span class="sxs-lookup"><span data-stu-id="f4a02-107">Use the `...beta/education/me/schools` resource in this case.</span></span>

## <a name="permissions"></a><span data-ttu-id="f4a02-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f4a02-108">Permissions</span></span>
<span data-ttu-id="f4a02-109">Для вызова этого API требуется сочетание разрешений.</span><span class="sxs-lookup"><span data-stu-id="f4a02-109">A combination of permissions is required to call this API.</span></span> <span data-ttu-id="f4a02-110">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f4a02-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4a02-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f4a02-111">Permission type</span></span>      | <span data-ttu-id="f4a02-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f4a02-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f4a02-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f4a02-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="f4a02-114">EduRoster.ReadBasic, EduRoster.Read или EduRoster.Write плюс Directory.Read.All или User.Read</span><span class="sxs-lookup"><span data-stu-id="f4a02-114">One from EduRoster.ReadBasic, EduRoster.Read, EduRoster.Write plus either Directory.Read.All or User.Read</span></span>|
|<span data-ttu-id="f4a02-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f4a02-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="f4a02-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f4a02-116">Not supported.</span></span>  |
|<span data-ttu-id="f4a02-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="f4a02-117">Application</span></span> | <span data-ttu-id="f4a02-118">EduRoster.Read.All, EduRoster.ReadWrite.All и Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="f4a02-118">EduRoster.Read.All, EduRoster.ReadWrite.All plus Directory.Read.All</span></span>| 

## <a name="http-request"></a><span data-ttu-id="f4a02-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f4a02-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/me/user
GET /education/users/{id}/user
```
## <a name="request-headers"></a><span data-ttu-id="f4a02-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f4a02-120">Request headers</span></span>
| <span data-ttu-id="f4a02-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f4a02-121">Header</span></span>       | <span data-ttu-id="f4a02-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f4a02-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f4a02-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f4a02-123">Authorization</span></span>  | <span data-ttu-id="f4a02-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f4a02-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f4a02-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f4a02-126">Request body</span></span>
<span data-ttu-id="f4a02-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f4a02-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="f4a02-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="f4a02-128">Response</span></span>
<span data-ttu-id="f4a02-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [user](../resources/user.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f4a02-129">If successful, this method returns a `200 OK` response code and a [user](../resources/user.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f4a02-130">Пример</span><span class="sxs-lookup"><span data-stu-id="f4a02-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f4a02-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="f4a02-131">Request</span></span>
<span data-ttu-id="f4a02-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f4a02-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f4a02-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="f4a02-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationuser_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/me/user
```
# <a name="c"></a>[<span data-ttu-id="f4a02-134">C#</span><span class="sxs-lookup"><span data-stu-id="f4a02-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationuser-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f4a02-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f4a02-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationuser-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f4a02-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f4a02-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationuser-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f4a02-137">Java</span><span class="sxs-lookup"><span data-stu-id="f4a02-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationuser-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f4a02-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="f4a02-138">Response</span></span>
<span data-ttu-id="f4a02-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f4a02-139">The following is an example of the response.</span></span> 

><span data-ttu-id="f4a02-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f4a02-140">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
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
```

<!-- uuid: FC4AAF57-A0ED-4899-B104-A8B89B72AD5A
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get user",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

