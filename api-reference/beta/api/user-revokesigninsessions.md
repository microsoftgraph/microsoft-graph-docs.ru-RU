---
title: 'Пользователь: Ревокесигнинсессионс'
description: Делает недействительным все маркеры обновления пользователя, выданные приложениям (а также файлам cookie сеанса в браузере пользователя), путем сброса свойства пользователя **сигнинсессионсвалидфромдатетиме** к текущей дате и времени.
localization_priority: Normal
author: krbain
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: a11fcdff43312eaeae7c94a815b5264f17f533ce
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48064460"
---
# <a name="user-revokesigninsessions"></a><span data-ttu-id="35981-103">Пользователь: Ревокесигнинсессионс</span><span class="sxs-lookup"><span data-stu-id="35981-103">user: revokeSignInSessions</span></span>

<span data-ttu-id="35981-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="35981-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="35981-105">Делает недействительными все маркеры обновления, выданные приложениям для пользователя (а также файлы cookie сеансов в браузере пользователя), путем сброса свойства пользователя **сигнинсессионсвалидфромдатетиме** к текущей дате и времени.</span><span class="sxs-lookup"><span data-stu-id="35981-105">Invalidates all the refresh tokens issued to applications for a user (as well as session cookies in a user's browser), by resetting the **signInSessionsValidFromDateTime** user property to the current date-time.</span></span> <span data-ttu-id="35981-106">Как правило, эта операция выполняется (пользователем или администратором), если пользователь имеет утерянное или украденное устройство.</span><span class="sxs-lookup"><span data-stu-id="35981-106">Typically, this operation is performed (by the user or an administrator) if the user has a lost or stolen device.</span></span> <span data-ttu-id="35981-107">Эта операция запрещает доступ к данным Организации через приложения на устройстве, требуя от пользователя повторного входа во все приложения, которые ранее были отосланы, независимо от устройства.</span><span class="sxs-lookup"><span data-stu-id="35981-107">This operation prevents access to the organization's data through applications on the device by requiring the user to sign in again to all applications that they have previously consented to, independent of device.</span></span>

<span data-ttu-id="35981-108">Если приложение пытается активировать маркер делегированного доступа для этого пользователя с помощью недействительного маркера обновления, приложение получит ошибку.</span><span class="sxs-lookup"><span data-stu-id="35981-108">If the application attempts to redeem a delegated access token for this user by using an invalidated refresh token, the application will get an error.</span></span> <span data-ttu-id="35981-109">В этом случае приложению потребуется получить новый маркер обновления, выполнив запрос к конечной точке авторизации, которая вынуждает пользователя выполнить вход.</span><span class="sxs-lookup"><span data-stu-id="35981-109">If this happens, the application will need to acquire a new refresh token by making a request to the authorize endpoint, which will force the user to sign in.</span></span>

>[!NOTE]
><span data-ttu-id="35981-110">После вызова **ревокесигнинсессионс**может возникнуть небольшая задержка в несколько минут до отзыва маркеров.</span><span class="sxs-lookup"><span data-stu-id="35981-110">After calling **revokeSignInSessions**, there might be a small delay of a few minutes before tokens are revoked.</span></span>

## <a name="permissions"></a><span data-ttu-id="35981-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="35981-111">Permissions</span></span>

<span data-ttu-id="35981-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="35981-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="35981-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="35981-114">Permission type</span></span>                        | <span data-ttu-id="35981-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="35981-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="35981-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="35981-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="35981-117">User. ReadWrite, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="35981-117">User.ReadWrite, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="35981-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="35981-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="35981-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="35981-119">Not supported.</span></span> |
|<span data-ttu-id="35981-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="35981-120">Application</span></span>                            | <span data-ttu-id="35981-121">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="35981-121">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="35981-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="35981-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/revokeSignInSessions
POST /users/{id | userPrincipalName}/revokeSignInSessions
```

## <a name="request-headers"></a><span data-ttu-id="35981-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="35981-123">Request headers</span></span>
| <span data-ttu-id="35981-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="35981-124">Header</span></span>       | <span data-ttu-id="35981-125">Значение</span><span class="sxs-lookup"><span data-stu-id="35981-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="35981-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="35981-126">Authorization</span></span>  | <span data-ttu-id="35981-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="35981-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="35981-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="35981-129">Content-Type</span></span>  | <span data-ttu-id="35981-130">application/json</span><span class="sxs-lookup"><span data-stu-id="35981-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="35981-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="35981-131">Request body</span></span>
<span data-ttu-id="35981-132">В этой операции нет содержимого запроса.</span><span class="sxs-lookup"><span data-stu-id="35981-132">This operation has no request content.</span></span>

## <a name="response"></a><span data-ttu-id="35981-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="35981-133">Response</span></span>

<span data-ttu-id="35981-134">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="35981-134">If successful, this method returns a `204 No Content` response code.</span></span>

>[!NOTE]
><span data-ttu-id="35981-135">У этого API есть [известная проблема](/graph/known-issues#revoke-sign-in-sessions-returns-wrong-HTTP-code).</span><span class="sxs-lookup"><span data-stu-id="35981-135">This API has a [known issue](/graph/known-issues#revoke-sign-in-sessions-returns-wrong-HTTP-code).</span></span> <span data-ttu-id="35981-136">Он возвращает другой код HTTP-ответа.</span><span class="sxs-lookup"><span data-stu-id="35981-136">It returns a different HTTP response code.</span></span>

## <a name="example"></a><span data-ttu-id="35981-137">Пример</span><span class="sxs-lookup"><span data-stu-id="35981-137">Example</span></span>
<span data-ttu-id="35981-138">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="35981-138">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="35981-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="35981-139">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="35981-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="35981-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_revokesigninsessionss"
}-->
```http
POST https://graph.microsoft.com/beta/me/revokeSignInSessions
```
# <a name="c"></a>[<span data-ttu-id="35981-141">C#</span><span class="sxs-lookup"><span data-stu-id="35981-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-revokesigninsessionss-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="35981-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="35981-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-revokesigninsessionss-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="35981-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="35981-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-revokesigninsessionss-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="35981-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="35981-144">Response</span></span>
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


