---
title: 'Пользователь: служебное invalidateallrefreshtokens'
description: Делает недействительными все маркеры обновления пользователя, выданные приложениям и файлам cookie сеанса в браузере пользователя.
localization_priority: Normal
author: krbain
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: e711a2979ef5861664f8d5f17fe98812654565e0
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48973836"
---
# <a name="user-invalidateallrefreshtokens"></a><span data-ttu-id="c8c8f-103">Пользователь: служебное invalidateallrefreshtokens</span><span class="sxs-lookup"><span data-stu-id="c8c8f-103">user: invalidateAllRefreshTokens</span></span>

<span data-ttu-id="c8c8f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c8c8f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c8c8f-105">Делает недействительными все маркеры обновления пользователя, выданные приложениям (а также файлам cookie сеанса в браузере пользователя), путем сброса свойства пользователя **refreshtokensvalidfromdatetime и указывая** к текущей дате и времени.</span><span class="sxs-lookup"><span data-stu-id="c8c8f-105">Invalidates all of the user's refresh tokens issued to applications (as well as session cookies in a user's browser), by resetting the **refreshTokensValidFromDateTime** user property to the current date-time.</span></span> <span data-ttu-id="c8c8f-106">Как правило, эта операция выполняется (пользователем или администратором), если пользователь имеет утерянное или украденное устройство.</span><span class="sxs-lookup"><span data-stu-id="c8c8f-106">Typically, this operation is performed (by the user or an administrator) if the user has a lost or stolen device.</span></span>  <span data-ttu-id="c8c8f-107">Эта операция запрещает доступ к данным в Организации, доступ к которым осуществляется через приложения на устройстве, без необходимости первого входа пользователя в систему.</span><span class="sxs-lookup"><span data-stu-id="c8c8f-107">This operation would prevent access to any of the organization's data accessed through applications on the device without the user first being required to sign in again.</span></span> <span data-ttu-id="c8c8f-108">В действительности эта операция приведет к принудительному входу пользователя в систему для всех приложений, для которых они ранее были отправлены, независимо от устройства.</span><span class="sxs-lookup"><span data-stu-id="c8c8f-108">In fact, this operation would force the user to sign in again for all applications that they have previously consented to, independent of device.</span></span>

<span data-ttu-id="c8c8f-109">Для разработчиков, если приложение пытается активировать маркер делегированного доступа для этого пользователя с помощью недействительного маркера обновления, приложение получит сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="c8c8f-109">For developers, if the application attempts to redeem a delegated access token for this user by using an invalidated refresh token, the application will get an error.</span></span> <span data-ttu-id="c8c8f-110">В этом случае приложению потребуется получить новый маркер обновления, выполнив запрос к конечной точке авторизации, которая вынуждает пользователя выполнить вход.</span><span class="sxs-lookup"><span data-stu-id="c8c8f-110">If this happens, the application will need to acquire a new refresh token by making a request to the authorize endpoint, which will force the user to sign in.</span></span>

## <a name="permissions"></a><span data-ttu-id="c8c8f-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c8c8f-111">Permissions</span></span>
<span data-ttu-id="c8c8f-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c8c8f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

+ <span data-ttu-id="c8c8f-114">Чтобы приложение, вошедшего в систему, не проверяло приложения, на которые они были отправлены: User. ReadWrite, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="c8c8f-114">For an application to allow the signed in user to invalidate applications they've consented to: User.ReadWrite, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>
+ <span data-ttu-id="c8c8f-115">Для приложения, позволяющего администратору сделать недействительными приложения, которые пользователь прослал: Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="c8c8f-115">For an application to allow an administrator to invalidate applications a user has consented to: Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>

## <a name="http-request"></a><span data-ttu-id="c8c8f-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c8c8f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/invalidateAllRefreshTokens
POST /users/{id | userPrincipalName}/invalidateAllRefreshTokens
```
## <a name="request-headers"></a><span data-ttu-id="c8c8f-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c8c8f-117">Request headers</span></span>
| <span data-ttu-id="c8c8f-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c8c8f-118">Header</span></span>       | <span data-ttu-id="c8c8f-119">Значение</span><span class="sxs-lookup"><span data-stu-id="c8c8f-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c8c8f-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c8c8f-120">Authorization</span></span>  | <span data-ttu-id="c8c8f-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c8c8f-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c8c8f-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c8c8f-123">Request body</span></span>
<span data-ttu-id="c8c8f-124">В этой операции нет содержимого запроса.</span><span class="sxs-lookup"><span data-stu-id="c8c8f-124">This operation has no request content.</span></span>

## <a name="response"></a><span data-ttu-id="c8c8f-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="c8c8f-125">Response</span></span>

<span data-ttu-id="c8c8f-126">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c8c8f-126">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c8c8f-127">Пример</span><span class="sxs-lookup"><span data-stu-id="c8c8f-127">Example</span></span>
<span data-ttu-id="c8c8f-128">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="c8c8f-128">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c8c8f-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="c8c8f-129">Request</span></span>
<span data-ttu-id="c8c8f-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c8c8f-130">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c8c8f-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="c8c8f-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_invalidateallrefreshtokens"
}-->
```http
POST https://graph.microsoft.com/beta/me/invalidateAllRefreshTokens
```
# <a name="c"></a>[<span data-ttu-id="c8c8f-132">C#</span><span class="sxs-lookup"><span data-stu-id="c8c8f-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-invalidateallrefreshtokens-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c8c8f-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c8c8f-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-invalidateallrefreshtokens-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c8c8f-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c8c8f-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-invalidateallrefreshtokens-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c8c8f-135">Java</span><span class="sxs-lookup"><span data-stu-id="c8c8f-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-invalidateallrefreshtokens-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c8c8f-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="c8c8f-136">Response</span></span>
<span data-ttu-id="c8c8f-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c8c8f-137">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "user: invalidateAllRefreshTokens",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


