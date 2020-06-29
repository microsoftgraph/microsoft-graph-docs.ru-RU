---
title: Получение пользователя
description: Получение простого каталога **user**, который соответствует этому объекту **educationUser**.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 5e60c09210d649b57cef19099de25561eaa07c2a
ms.sourcegitcommit: 55e9497c8e003be389f8b5d641f80dae7bf6004b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2020
ms.locfileid: "44909590"
---
# <a name="get-user"></a><span data-ttu-id="85305-103">Получение пользователя</span><span class="sxs-lookup"><span data-stu-id="85305-103">Get user</span></span>

<span data-ttu-id="85305-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85305-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="85305-105">Получение простого каталога **user**, который соответствует этому объекту **educationUser**.</span><span class="sxs-lookup"><span data-stu-id="85305-105">Retrieve the simple directory **user** that corresponds to this **educationUser**.</span></span>

> [!NOTE]
> <span data-ttu-id="85305-106">Если используется делегированный маркер, участники могут видеть только сведения о своей учетной записи.</span><span class="sxs-lookup"><span data-stu-id="85305-106">If the delegated token is used, members can only see information about their own account.</span></span> <span data-ttu-id="85305-107">В данном случае используйте ресурс `beta/education/me/users`.</span><span class="sxs-lookup"><span data-stu-id="85305-107">Use the `beta/education/me/users` resource in this case.</span></span>

## <a name="permissions"></a><span data-ttu-id="85305-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="85305-108">Permissions</span></span>

<span data-ttu-id="85305-109">Для вызова этого API требуется сочетание разрешений.</span><span class="sxs-lookup"><span data-stu-id="85305-109">A combination of permissions is required to call this API.</span></span> <span data-ttu-id="85305-110">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85305-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="85305-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="85305-111">Permission type</span></span>                        | <span data-ttu-id="85305-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="85305-112">Permissions (from least to most privileged)</span></span>                                                               |
| :------------------------------------- | :-------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="85305-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="85305-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="85305-114">EduRoster.ReadBasic, EduRoster.Read или EduRoster.Write плюс Directory.Read.All или User.Read</span><span class="sxs-lookup"><span data-stu-id="85305-114">One from EduRoster.ReadBasic, EduRoster.Read, EduRoster.Write plus either Directory.Read.All or User.Read</span></span> |
| <span data-ttu-id="85305-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="85305-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="85305-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85305-116">Not supported.</span></span>                                                                                            |
| <span data-ttu-id="85305-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="85305-117">Application</span></span>                            | <span data-ttu-id="85305-118">EduRoster.Read.All, EduRoster.ReadWrite.All и Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="85305-118">EduRoster.Read.All, EduRoster.ReadWrite.All plus Directory.Read.All</span></span>                                       |

## <a name="http-request"></a><span data-ttu-id="85305-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="85305-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /education/me/user
GET /education/users/{id}/user
```

## <a name="request-headers"></a><span data-ttu-id="85305-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="85305-120">Request headers</span></span>

| <span data-ttu-id="85305-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="85305-121">Header</span></span>        | <span data-ttu-id="85305-122">Значение</span><span class="sxs-lookup"><span data-stu-id="85305-122">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="85305-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="85305-123">Authorization</span></span> | <span data-ttu-id="85305-124">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="85305-124">Bearer {token}.</span></span> <span data-ttu-id="85305-125">Required.</span><span class="sxs-lookup"><span data-stu-id="85305-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="85305-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="85305-126">Request body</span></span>

<span data-ttu-id="85305-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="85305-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="85305-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="85305-128">Response</span></span>

<span data-ttu-id="85305-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [user](../resources/user.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="85305-129">If successful, this method returns a `200 OK` response code and a [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85305-130">Пример</span><span class="sxs-lookup"><span data-stu-id="85305-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="85305-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="85305-131">Request</span></span>

<span data-ttu-id="85305-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="85305-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="85305-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="85305-133">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "get_educationuser"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/education/me/user
```

# <a name="c"></a>[<span data-ttu-id="85305-134">C#</span><span class="sxs-lookup"><span data-stu-id="85305-134">C#</span></span>](#tab/csharp)

[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="85305-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="85305-135">JavaScript</span></span>](#tab/javascript)

[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="85305-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="85305-136">Objective-C</span></span>](#tab/objc)

[!INCLUDE [sample-code](../includes/snippets/objc/get-educationuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="85305-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="85305-137">Response</span></span>

<span data-ttu-id="85305-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="85305-138">The following is an example of the response.</span></span>

> <span data-ttu-id="85305-139">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="85305-139">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="85305-140">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="85305-140">All the properties will be returned from an actual call.</span></span>

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
