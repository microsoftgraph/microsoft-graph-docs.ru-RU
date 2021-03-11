---
title: 'пользователь: revokeSignInSessions'
description: Недействительными признаны все маркеры обновления пользователя, выданные приложениям (а также cookie-файлы сеансов в браузере пользователя), сбросив свойство **signInSessionsValidFromDateTime** в текущее время даты.
localization_priority: Normal
author: jpettere
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 53d194ac1058652c06e673beca1fdd6aeb876719
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50719733"
---
# <a name="user-revokesigninsessions"></a><span data-ttu-id="2c849-103">пользователь: revokeSignInSessions</span><span class="sxs-lookup"><span data-stu-id="2c849-103">user: revokeSignInSessions</span></span>

<span data-ttu-id="2c849-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2c849-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2c849-105">Недействительными признаны все маркеры обновления, выданные приложениям для пользователя (а также cookie-файлы сеансов в браузере пользователя), сбросив свойство **signInSessionsValidFromDateTime** в текущее время даты.</span><span class="sxs-lookup"><span data-stu-id="2c849-105">Invalidates all the refresh tokens issued to applications for a user (as well as session cookies in a user's browser), by resetting the **signInSessionsValidFromDateTime** user property to the current date-time.</span></span> <span data-ttu-id="2c849-106">Обычно эта операция выполняется (пользователем или администратором), если у пользователя потеряно или украдено устройство.</span><span class="sxs-lookup"><span data-stu-id="2c849-106">Typically, this operation is performed (by the user or an administrator) if the user has a lost or stolen device.</span></span> <span data-ttu-id="2c849-107">Эта операция предотвращает доступ к данным организации с помощью приложений на устройстве, требуя от пользователя снова войти во все приложения, с которыми они ранее согласились, независимо от устройства.</span><span class="sxs-lookup"><span data-stu-id="2c849-107">This operation prevents access to the organization's data through applications on the device by requiring the user to sign in again to all applications that they have previously consented to, independent of device.</span></span>

<span data-ttu-id="2c849-108">Если приложение пытается выкупить делегированный маркер доступа для этого пользователя с помощью недействительных маркеров обновления, приложение получит ошибку.</span><span class="sxs-lookup"><span data-stu-id="2c849-108">If the application attempts to redeem a delegated access token for this user by using an invalidated refresh token, the application will get an error.</span></span> <span data-ttu-id="2c849-109">Если это произойдет, приложению потребуется приобрести новый маркер обновления, сделав запрос в конечную точку авторизации, что заставит пользователя войти.</span><span class="sxs-lookup"><span data-stu-id="2c849-109">If this happens, the application will need to acquire a new refresh token by making a request to the authorize endpoint, which will force the user to sign in.</span></span>

>[!NOTE]
><span data-ttu-id="2c849-110">После вызова **revokeSignInSessions** может возникнуть небольшая задержка в несколько минут до отзыва маркеров.</span><span class="sxs-lookup"><span data-stu-id="2c849-110">After calling **revokeSignInSessions**, there might be a small delay of a few minutes before tokens are revoked.</span></span>

## <a name="permissions"></a><span data-ttu-id="2c849-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2c849-111">Permissions</span></span>

<span data-ttu-id="2c849-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2c849-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2c849-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2c849-114">Permission type</span></span>                        | <span data-ttu-id="2c849-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2c849-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="2c849-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2c849-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="2c849-117">User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2c849-117">User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="2c849-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2c849-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2c849-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2c849-119">Not supported.</span></span> |
|<span data-ttu-id="2c849-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2c849-120">Application</span></span>                            | <span data-ttu-id="2c849-121">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c849-121">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2c849-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2c849-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/revokeSignInSessions
POST /users/{id | userPrincipalName}/revokeSignInSessions
```

## <a name="request-headers"></a><span data-ttu-id="2c849-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2c849-123">Request headers</span></span>
| <span data-ttu-id="2c849-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2c849-124">Header</span></span>       | <span data-ttu-id="2c849-125">Значение</span><span class="sxs-lookup"><span data-stu-id="2c849-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2c849-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2c849-126">Authorization</span></span>  | <span data-ttu-id="2c849-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2c849-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="2c849-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2c849-129">Content-Type</span></span>  | <span data-ttu-id="2c849-130">application/json</span><span class="sxs-lookup"><span data-stu-id="2c849-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2c849-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2c849-131">Request body</span></span>
<span data-ttu-id="2c849-132">Эта операция не имеет контента запроса.</span><span class="sxs-lookup"><span data-stu-id="2c849-132">This operation has no request content.</span></span>

## <a name="response"></a><span data-ttu-id="2c849-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="2c849-133">Response</span></span>

<span data-ttu-id="2c849-134">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="2c849-134">If successful, this method returns a `204 No Content` response code.</span></span>

>[!NOTE]
><span data-ttu-id="2c849-135">У этого API есть [известная проблема](/graph/known-issues#revoke-sign-in-sessions-returns-wrong-HTTP-code).</span><span class="sxs-lookup"><span data-stu-id="2c849-135">This API has a [known issue](/graph/known-issues#revoke-sign-in-sessions-returns-wrong-HTTP-code).</span></span> <span data-ttu-id="2c849-136">Он возвращает другой код ответа HTTP.</span><span class="sxs-lookup"><span data-stu-id="2c849-136">It returns a different HTTP response code.</span></span>

## <a name="example"></a><span data-ttu-id="2c849-137">Пример</span><span class="sxs-lookup"><span data-stu-id="2c849-137">Example</span></span>
<span data-ttu-id="2c849-138">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="2c849-138">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="2c849-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="2c849-139">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="2c849-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="2c849-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_revokesigninsessionss"
}-->
```http
POST https://graph.microsoft.com/beta/me/revokeSignInSessions
```
# <a name="c"></a>[<span data-ttu-id="2c849-141">C#</span><span class="sxs-lookup"><span data-stu-id="2c849-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-revokesigninsessionss-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2c849-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2c849-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-revokesigninsessionss-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2c849-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2c849-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-revokesigninsessionss-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2c849-144">Java</span><span class="sxs-lookup"><span data-stu-id="2c849-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-revokesigninsessionss-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="2c849-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="2c849-145">Response</span></span>
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
  "description": "user: revokeSignInSessions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


