---
title: 'пользователь: invalidateAllRefreshTokens'
description: Недействительными признаны все маркеры обновления пользователя, выданные приложениям и cookie-файлам сеансов в браузере пользователя.
localization_priority: Normal
author: jpettere
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: a13982cb924c5c9b82c3248aefc13a54ec44bb2e
ms.sourcegitcommit: 4888ac7504533344c4fc6828e2a06a002a1d72d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2021
ms.locfileid: "53351050"
---
# <a name="user-invalidateallrefreshtokens"></a><span data-ttu-id="4ad5c-103">пользователь: invalidateAllRefreshTokens</span><span class="sxs-lookup"><span data-stu-id="4ad5c-103">user: invalidateAllRefreshTokens</span></span>

<span data-ttu-id="4ad5c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ad5c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4ad5c-105">Недействительными признаны все маркеры обновления пользователя, выданные приложениям (а также cookie-файлы сеансов в браузере пользователя), сбросив свойство **refreshTokensValidFromDateTime** в текущее время даты.</span><span class="sxs-lookup"><span data-stu-id="4ad5c-105">Invalidates all of the user's refresh tokens issued to applications (as well as session cookies in a user's browser), by resetting the **refreshTokensValidFromDateTime** user property to the current date-time.</span></span> <span data-ttu-id="4ad5c-106">Обычно эта операция выполняется (пользователем или администратором), если у пользователя потеряно или украдено устройство.</span><span class="sxs-lookup"><span data-stu-id="4ad5c-106">Typically, this operation is performed (by the user or an administrator) if the user has a lost or stolen device.</span></span>  <span data-ttu-id="4ad5c-107">Эта операция предотвратит доступ к любым данным организации, которые будут доступны через приложения на устройстве, без необходимости повторного входного доступа к пользователю.</span><span class="sxs-lookup"><span data-stu-id="4ad5c-107">This operation would prevent access to any of the organization's data accessed through applications on the device without the user first being required to sign in again.</span></span> <span data-ttu-id="4ad5c-108">На самом деле эта операция заставит пользователя снова войти для всех приложений, с чем они ранее согласились, независимо от устройства.</span><span class="sxs-lookup"><span data-stu-id="4ad5c-108">In fact, this operation would force the user to sign in again for all applications that they have previously consented to, independent of device.</span></span>

<span data-ttu-id="4ad5c-109">Для разработчиков, если приложение пытается выкупить делегированный маркер доступа для этого пользователя с помощью недействительных маркеров обновления, приложение получит ошибку.</span><span class="sxs-lookup"><span data-stu-id="4ad5c-109">For developers, if the application attempts to redeem a delegated access token for this user by using an invalidated refresh token, the application will get an error.</span></span> <span data-ttu-id="4ad5c-110">Если это произойдет, приложению потребуется приобрести новый маркер обновления, сделав запрос в конечную точку авторизации, что заставит пользователя войти.</span><span class="sxs-lookup"><span data-stu-id="4ad5c-110">If this happens, the application will need to acquire a new refresh token by making a request to the authorize endpoint, which will force the user to sign in.</span></span>

## <a name="permissions"></a><span data-ttu-id="4ad5c-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4ad5c-111">Permissions</span></span>
<span data-ttu-id="4ad5c-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ad5c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

+ <span data-ttu-id="4ad5c-114">Чтобы приложение разрешило подписанному пользователю признать недействительными приложения, на которые они согласились: User.ReadWrite, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4ad5c-114">For an application to allow the signed in user to invalidate applications they've consented to: User.ReadWrite, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>
+ <span data-ttu-id="4ad5c-115">Чтобы приложение разрешило администратору признать приложения недействительными, пользователь дал согласие: Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4ad5c-115">For an application to allow an administrator to invalidate applications a user has consented to: Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>

## <a name="http-request"></a><span data-ttu-id="4ad5c-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4ad5c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/invalidateAllRefreshTokens
POST /users/{id | userPrincipalName}/invalidateAllRefreshTokens
```
## <a name="request-headers"></a><span data-ttu-id="4ad5c-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4ad5c-117">Request headers</span></span>
| <span data-ttu-id="4ad5c-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4ad5c-118">Header</span></span>       | <span data-ttu-id="4ad5c-119">Значение</span><span class="sxs-lookup"><span data-stu-id="4ad5c-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4ad5c-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4ad5c-120">Authorization</span></span>  | <span data-ttu-id="4ad5c-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4ad5c-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4ad5c-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4ad5c-123">Request body</span></span>
<span data-ttu-id="4ad5c-124">Эта операция не имеет контента запроса.</span><span class="sxs-lookup"><span data-stu-id="4ad5c-124">This operation has no request content.</span></span>

## <a name="response"></a><span data-ttu-id="4ad5c-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="4ad5c-125">Response</span></span>

<span data-ttu-id="4ad5c-126">При успешном выполнении этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="4ad5c-126">If successful, this method returns `204 No Content` response code.</span></span>

>[!NOTE]
><span data-ttu-id="4ad5c-127">Этот API возвращает другой код ответа HTTP, аналогичный действию [revokeSignInSessions.](user-revokesigninsessions.md)</span><span class="sxs-lookup"><span data-stu-id="4ad5c-127">This API returns a different HTTP response code, similar to the [revokeSignInSessions](user-revokesigninsessions.md) action.</span></span> <span data-ttu-id="4ad5c-128">Подробнее см. в [материале "Известная проблема".](/graph/known-issues#revoke-sign-in-sessions-returns-wrong-HTTP-code)</span><span class="sxs-lookup"><span data-stu-id="4ad5c-128">For details, see [known issue](/graph/known-issues#revoke-sign-in-sessions-returns-wrong-HTTP-code).</span></span> 

## <a name="example"></a><span data-ttu-id="4ad5c-129">Пример</span><span class="sxs-lookup"><span data-stu-id="4ad5c-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="4ad5c-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="4ad5c-130">Request</span></span>
<span data-ttu-id="4ad5c-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4ad5c-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4ad5c-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="4ad5c-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_invalidateallrefreshtokens"
}-->
```http
POST https://graph.microsoft.com/beta/me/invalidateAllRefreshTokens
```
# <a name="c"></a>[<span data-ttu-id="4ad5c-133">C#</span><span class="sxs-lookup"><span data-stu-id="4ad5c-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-invalidateallrefreshtokens-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4ad5c-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4ad5c-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-invalidateallrefreshtokens-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4ad5c-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4ad5c-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-invalidateallrefreshtokens-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4ad5c-136">Java</span><span class="sxs-lookup"><span data-stu-id="4ad5c-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-invalidateallrefreshtokens-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4ad5c-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="4ad5c-137">Response</span></span>
<span data-ttu-id="4ad5c-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="4ad5c-138">The following is an example of the response.</span></span> 
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


