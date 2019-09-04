---
title: Получение пользователя
description: Получение простого каталога **user**, который соответствует этому объекту **educationUser**.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 0c7c67d6bf8e913b6cff1fb6a523e30bdb8e232f
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36720279"
---
# <a name="get-user"></a><span data-ttu-id="f53cb-103">Получение пользователя</span><span class="sxs-lookup"><span data-stu-id="f53cb-103">Get user</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f53cb-104">Получение простого каталога **user**, который соответствует этому объекту **educationUser**.</span><span class="sxs-lookup"><span data-stu-id="f53cb-104">Retrieve the simple directory **user** that corresponds to this **educationUser**.</span></span>

><span data-ttu-id="f53cb-105">**Примечание.** Если используется делегированный маркер, участники могут видеть сведения только о своих учебных заведениях.</span><span class="sxs-lookup"><span data-stu-id="f53cb-105">**Note:** If the delegated token is used, members can only see information about their own schools.</span></span> <span data-ttu-id="f53cb-106">В данном случае используйте ресурс `...beta/education/me/schools`.</span><span class="sxs-lookup"><span data-stu-id="f53cb-106">Use the `...beta/education/me/schools` resource in this case.</span></span>

## <a name="permissions"></a><span data-ttu-id="f53cb-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f53cb-107">Permissions</span></span>
<span data-ttu-id="f53cb-108">Для вызова этого API требуется сочетание разрешений.</span><span class="sxs-lookup"><span data-stu-id="f53cb-108">A combination of permissions is required to call this API.</span></span> <span data-ttu-id="f53cb-109">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f53cb-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f53cb-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f53cb-110">Permission type</span></span>      | <span data-ttu-id="f53cb-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f53cb-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f53cb-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f53cb-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="f53cb-113">EduRoster.ReadBasic, EduRoster.Read или EduRoster.Write плюс Directory.Read.All или User.Read</span><span class="sxs-lookup"><span data-stu-id="f53cb-113">One from EduRoster.ReadBasic, EduRoster.Read, EduRoster.Write plus either Directory.Read.All or User.Read</span></span>|
|<span data-ttu-id="f53cb-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f53cb-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="f53cb-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f53cb-115">Not supported.</span></span>  |
|<span data-ttu-id="f53cb-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f53cb-116">Application</span></span> | <span data-ttu-id="f53cb-117">EduRoster.Read.All, EduRoster.ReadWrite.All и Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="f53cb-117">EduRoster.Read.All, EduRoster.ReadWrite.All plus Directory.Read.All</span></span>| 

## <a name="http-request"></a><span data-ttu-id="f53cb-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f53cb-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/me/user
GET /education/users/{id}/user
```
## <a name="request-headers"></a><span data-ttu-id="f53cb-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f53cb-119">Request headers</span></span>
| <span data-ttu-id="f53cb-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f53cb-120">Header</span></span>       | <span data-ttu-id="f53cb-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f53cb-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f53cb-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f53cb-122">Authorization</span></span>  | <span data-ttu-id="f53cb-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f53cb-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f53cb-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f53cb-125">Request body</span></span>
<span data-ttu-id="f53cb-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f53cb-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="f53cb-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="f53cb-127">Response</span></span>
<span data-ttu-id="f53cb-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [user](../resources/user.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f53cb-128">If successful, this method returns a `200 OK` response code and a [user](../resources/user.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f53cb-129">Пример</span><span class="sxs-lookup"><span data-stu-id="f53cb-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f53cb-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="f53cb-130">Request</span></span>
<span data-ttu-id="f53cb-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f53cb-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f53cb-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="f53cb-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationuser"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/me/user
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f53cb-133">C#</span><span class="sxs-lookup"><span data-stu-id="f53cb-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f53cb-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f53cb-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f53cb-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="f53cb-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f53cb-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="f53cb-136">Response</span></span>
<span data-ttu-id="f53cb-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f53cb-137">The following is an example of the response.</span></span> 

><span data-ttu-id="f53cb-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f53cb-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "Get user",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
