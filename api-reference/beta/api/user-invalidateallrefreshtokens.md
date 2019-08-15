---
title: 'Пользователь: служебное invalidateallrefreshtokens'
description: Делает недействительными все маркеры обновления пользователя, выданные приложениям (а также файлам cookie сеанса в браузере пользователя), путем сброса свойства пользователя **refreshtokensvalidfromdatetime и указывая** к текущей дате и времени. Как правило, эта операция выполняется (пользователем или администратором), если пользователь имеет утерянное или украденное устройство.  Эта операция запрещает доступ к данным в Организации, доступ к которым осуществляется через приложения на устройстве, без необходимости первого входа пользователя в систему. В действительности эта операция приведет к принудительному входу пользователя в систему для всех приложений, для которых они ранее были отправлены, независимо от устройства.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e4efc33f3c0cb0f0ec4f4ef4026598d6d2f8a581
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36421091"
---
# <a name="user-invalidateallrefreshtokens"></a><span data-ttu-id="85622-106">Пользователь: служебное invalidateallrefreshtokens</span><span class="sxs-lookup"><span data-stu-id="85622-106">user: invalidateAllRefreshTokens</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="85622-107">Делает недействительными все маркеры обновления пользователя, выданные приложениям (а также файлам cookie сеанса в браузере пользователя), путем сброса свойства пользователя **refreshtokensvalidfromdatetime и указывая** к текущей дате и времени.</span><span class="sxs-lookup"><span data-stu-id="85622-107">Invalidates all of the user's refresh tokens issued to applications (as well as session cookies in a user's browser), by resetting the **refreshTokensValidFromDateTime** user property to the current date-time.</span></span> <span data-ttu-id="85622-108">Как правило, эта операция выполняется (пользователем или администратором), если пользователь имеет утерянное или украденное устройство.</span><span class="sxs-lookup"><span data-stu-id="85622-108">Typically, this operation is performed (by the user or an administrator) if the user has a lost or stolen device.</span></span>  <span data-ttu-id="85622-109">Эта операция запрещает доступ к данным в Организации, доступ к которым осуществляется через приложения на устройстве, без необходимости первого входа пользователя в систему.</span><span class="sxs-lookup"><span data-stu-id="85622-109">This operation would prevent access to any of the organization's data accessed through applications on the device without the user first being required to sign in again.</span></span> <span data-ttu-id="85622-110">В действительности эта операция приведет к принудительному входу пользователя в систему для всех приложений, для которых они ранее были отправлены, независимо от устройства.</span><span class="sxs-lookup"><span data-stu-id="85622-110">In fact, this operation would force the user to sign in again for all applications that they have previously consented to, independent of device.</span></span>

<span data-ttu-id="85622-111">Для разработчиков, если приложение пытается активировать маркер делегированного доступа для этого пользователя с помощью недействительного маркера обновления, приложение получит сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="85622-111">For developers, if the application attempts to redeem a delegated access token for this user by using an invalidated refresh token, the application will get an error.</span></span> <span data-ttu-id="85622-112">В этом случае приложению потребуется получить новый маркер обновления, выполнив запрос к конечной точке авторизации, которая вынуждает пользователя выполнить вход.</span><span class="sxs-lookup"><span data-stu-id="85622-112">If this happens, the application will need to acquire a new refresh token by making a request to the authorize endpoint, which will force the user to sign in.</span></span>

## <a name="permissions"></a><span data-ttu-id="85622-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="85622-113">Permissions</span></span>
<span data-ttu-id="85622-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85622-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

+ <span data-ttu-id="85622-116">Чтобы приложение, вошедшего в систему, не проверяло приложения, на которые они были отправлены: User. ReadWrite, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="85622-116">For an application to allow the signed in user to invalidate applications they've consented to: User.ReadWrite, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>
+ <span data-ttu-id="85622-117">Для приложения, позволяющего администратору сделать недействительными приложения, которые пользователь прослал: Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="85622-117">For an application to allow an administrator to invalidate applications a user has consented to: Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>

## <a name="http-request"></a><span data-ttu-id="85622-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="85622-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/invalidateAllRefreshTokens
POST /users/{id | userPrincipalName}/invalidateAllRefreshTokens
```
## <a name="request-headers"></a><span data-ttu-id="85622-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="85622-119">Request headers</span></span>
| <span data-ttu-id="85622-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="85622-120">Header</span></span>       | <span data-ttu-id="85622-121">Значение</span><span class="sxs-lookup"><span data-stu-id="85622-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="85622-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="85622-122">Authorization</span></span>  | <span data-ttu-id="85622-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="85622-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="85622-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="85622-125">Request body</span></span>
<span data-ttu-id="85622-126">В этой операции нет содержимого запроса.</span><span class="sxs-lookup"><span data-stu-id="85622-126">This operation has no request content.</span></span>

## <a name="response"></a><span data-ttu-id="85622-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="85622-127">Response</span></span>

<span data-ttu-id="85622-128">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="85622-128">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="85622-129">Пример</span><span class="sxs-lookup"><span data-stu-id="85622-129">Example</span></span>
<span data-ttu-id="85622-130">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="85622-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="85622-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="85622-131">Request</span></span>
<span data-ttu-id="85622-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="85622-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="85622-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="85622-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_invalidateallrefreshtokens"
}-->
```http
POST https://graph.microsoft.com/beta/me/invalidateAllRefreshTokens
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="85622-134">C#</span><span class="sxs-lookup"><span data-stu-id="85622-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-invalidateallrefreshtokens-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="85622-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="85622-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-invalidateallrefreshtokens-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="85622-136">Цель — C</span><span class="sxs-lookup"><span data-stu-id="85622-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-invalidateallrefreshtokens-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="85622-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="85622-137">Response</span></span>
<span data-ttu-id="85622-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="85622-138">Here is an example of the response.</span></span> 
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
