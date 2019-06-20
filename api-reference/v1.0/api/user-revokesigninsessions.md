---
title: 'Пользователь: Ревокесигнинсессионс'
description: Делает недействительным все маркеры обновления пользователя, выданные приложениям (а также файлам cookie сеанса в браузере пользователя), путем сброса свойства пользователя **сигнинсессионсвалидфромдатетиме** к текущей дате и времени.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 7ab60a38e404dc13dbbc58b1103931cfe0b16c44
ms.sourcegitcommit: b523648530fcc8c2a3ded35b419be8047b9fcd10
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/20/2019
ms.locfileid: "35083951"
---
# <a name="user-revokesigninsessions"></a><span data-ttu-id="5fe28-103">Пользователь: Ревокесигнинсессионс</span><span class="sxs-lookup"><span data-stu-id="5fe28-103">user: revokeSignInSessions</span></span>

<span data-ttu-id="5fe28-104">Делает недействительными все маркеры обновления, выданные приложениям для пользователя (а также файлы cookie сеансов в браузере пользователя), путем сброса свойства пользователя **сигнинсессионсвалидфромдатетиме** к текущей дате и времени.</span><span class="sxs-lookup"><span data-stu-id="5fe28-104">Invalidates all the refresh tokens issued to applications for a user (as well as session cookies in a user's browser), by resetting the **signInSessionsValidFromDateTime** user property to the current date-time.</span></span> <span data-ttu-id="5fe28-105">Как правило, эта операция выполняется (пользователем или администратором), если пользователь имеет утерянное или украденное устройство.</span><span class="sxs-lookup"><span data-stu-id="5fe28-105">Typically, this operation is performed (by the user or an administrator) if the user has a lost or stolen device.</span></span> <span data-ttu-id="5fe28-106">Эта операция запрещает доступ к данным Организации через приложения на устройстве, требуя от пользователя повторного входа во все приложения, которые ранее были отосланы, независимо от устройства.</span><span class="sxs-lookup"><span data-stu-id="5fe28-106">This operation prevents access to the organization's data through applications on the device by requiring the user to sign in again to all applications that they have previously consented to, independent of device.</span></span>

><span data-ttu-id="5fe28-107">Если приложение пытается активировать маркер делегированного доступа для этого пользователя с помощью недействительного маркера обновления, приложение получит ошибку.</span><span class="sxs-lookup"><span data-stu-id="5fe28-107">If the application attempts to redeem a delegated access token for this user by using an invalidated refresh token, the application will get an error.</span></span> <span data-ttu-id="5fe28-108">В этом случае приложению потребуется получить новый маркер обновления, выполнив запрос к конечной точке авторизации, которая вынуждает пользователя выполнить вход.</span><span class="sxs-lookup"><span data-stu-id="5fe28-108">If this happens, the application will need to acquire a new refresh token by making a request to the authorize endpoint, which will force the user to sign in.</span></span>

>[!NOTE]
><span data-ttu-id="5fe28-109">После вызова **ревокесигнинсессионс**может возникнуть небольшая задержка в несколько минут до отзыва маркеров.</span><span class="sxs-lookup"><span data-stu-id="5fe28-109">After calling **revokeSignInSessions**, there might be a small delay of a few minutes before tokens are revoked.</span></span>

## <a name="permissions"></a><span data-ttu-id="5fe28-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5fe28-110">Permissions</span></span>

<span data-ttu-id="5fe28-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5fe28-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5fe28-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5fe28-113">Permission type</span></span>                        | <span data-ttu-id="5fe28-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5fe28-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="5fe28-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5fe28-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="5fe28-116">User. ReadWrite, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="5fe28-116">User.ReadWrite, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="5fe28-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5fe28-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5fe28-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5fe28-118">Not supported.</span></span> |
|<span data-ttu-id="5fe28-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5fe28-119">Application</span></span>                            | <span data-ttu-id="5fe28-120">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5fe28-120">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5fe28-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5fe28-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/revokeSignInSessions
POST /users/{id | userPrincipalName}/revokeSignInSessions
```

## <a name="request-headers"></a><span data-ttu-id="5fe28-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5fe28-122">Request headers</span></span>
| <span data-ttu-id="5fe28-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5fe28-123">Header</span></span>       | <span data-ttu-id="5fe28-124">Значение</span><span class="sxs-lookup"><span data-stu-id="5fe28-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5fe28-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5fe28-125">Authorization</span></span>  | <span data-ttu-id="5fe28-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5fe28-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5fe28-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5fe28-128">Request body</span></span>
<span data-ttu-id="5fe28-129">В этой операции нет содержимого запроса.</span><span class="sxs-lookup"><span data-stu-id="5fe28-129">This operation has no request content.</span></span>

## <a name="response"></a><span data-ttu-id="5fe28-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="5fe28-130">Response</span></span>

<span data-ttu-id="5fe28-131">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="5fe28-131">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="5fe28-132">Пример</span><span class="sxs-lookup"><span data-stu-id="5fe28-132">Example</span></span>
<span data-ttu-id="5fe28-133">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="5fe28-133">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="5fe28-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="5fe28-134">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "user_revokesigninsessionss"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/revokeSignInSessions
```

##### <a name="response"></a><span data-ttu-id="5fe28-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="5fe28-135">Response</span></span>
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
    "Error: /api-reference/beta/api/user-revokesigninsessions.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-revokesigninsessions.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
