---
title: 'Пользователь: Ревокесигнинсессионс'
description: Делает недействительным все маркеры обновления пользователя, выданные приложениям (а также файлам cookie сеанса в браузере пользователя), путем сброса свойства пользователя **сигнинсессионсвалидфромдатетиме** к текущей дате и времени.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 128ebec580fa97707c56d099f5a6e7c66fa3dfc2
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334531"
---
# <a name="user-revokesigninsessions"></a><span data-ttu-id="59b27-103">Пользователь: Ревокесигнинсессионс</span><span class="sxs-lookup"><span data-stu-id="59b27-103">user: revokeSignInSessions</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59b27-104">Делает недействительными все маркеры обновления, выданные приложениям для пользователя (а также файлы cookie сеансов в браузере пользователя), путем сброса свойства пользователя **сигнинсессионсвалидфромдатетиме** к текущей дате и времени.</span><span class="sxs-lookup"><span data-stu-id="59b27-104">Invalidates all the refresh tokens issued to applications for a user (as well as session cookies in a user's browser), by resetting the **signInSessionsValidFromDateTime** user property to the current date-time.</span></span> <span data-ttu-id="59b27-105">Как правило, эта операция выполняется (пользователем или администратором), если пользователь имеет утерянное или украденное устройство.</span><span class="sxs-lookup"><span data-stu-id="59b27-105">Typically, this operation is performed (by the user or an administrator) if the user has a lost or stolen device.</span></span> <span data-ttu-id="59b27-106">Эта операция запрещает доступ к данным Организации через приложения на устройстве, требуя от пользователя повторного входа во все приложения, которые ранее были отосланы, независимо от устройства.</span><span class="sxs-lookup"><span data-stu-id="59b27-106">This operation prevents access to the organization's data through applications on the device by requiring the user to sign in again to all applications that they have previously consented to, independent of device.</span></span>

<span data-ttu-id="59b27-107">Если приложение пытается активировать маркер делегированного доступа для этого пользователя с помощью недействительного маркера обновления, приложение получит ошибку.</span><span class="sxs-lookup"><span data-stu-id="59b27-107">If the application attempts to redeem a delegated access token for this user by using an invalidated refresh token, the application will get an error.</span></span> <span data-ttu-id="59b27-108">В этом случае приложению потребуется получить новый маркер обновления, выполнив запрос к конечной точке авторизации, которая вынуждает пользователя выполнить вход.</span><span class="sxs-lookup"><span data-stu-id="59b27-108">If this happens, the application will need to acquire a new refresh token by making a request to the authorize endpoint, which will force the user to sign in.</span></span>

## <a name="permissions"></a><span data-ttu-id="59b27-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="59b27-109">Permissions</span></span>
<span data-ttu-id="59b27-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="59b27-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59b27-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="59b27-112">Permission type</span></span>                        | <span data-ttu-id="59b27-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="59b27-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="59b27-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="59b27-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="59b27-115">User. ReadWrite, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="59b27-115">User.ReadWrite, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="59b27-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="59b27-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="59b27-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="59b27-117">Not supported.</span></span> |
|<span data-ttu-id="59b27-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="59b27-118">Application</span></span>                            | <span data-ttu-id="59b27-119">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="59b27-119">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="59b27-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="59b27-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/revokeSignInSessions
POST /users/{id | userPrincipalName}/revokeSignInSessions
```
## <a name="request-headers"></a><span data-ttu-id="59b27-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="59b27-121">Request headers</span></span>
| <span data-ttu-id="59b27-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="59b27-122">Header</span></span>       | <span data-ttu-id="59b27-123">Значение</span><span class="sxs-lookup"><span data-stu-id="59b27-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="59b27-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="59b27-124">Authorization</span></span>  | <span data-ttu-id="59b27-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="59b27-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="59b27-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="59b27-127">Request body</span></span>
<span data-ttu-id="59b27-128">В этой операции нет содержимого запроса.</span><span class="sxs-lookup"><span data-stu-id="59b27-128">This operation has no request content.</span></span>

## <a name="response"></a><span data-ttu-id="59b27-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="59b27-129">Response</span></span>

<span data-ttu-id="59b27-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="59b27-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="59b27-131">Пример</span><span class="sxs-lookup"><span data-stu-id="59b27-131">Example</span></span>
<span data-ttu-id="59b27-132">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="59b27-132">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="59b27-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="59b27-133">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "user_revokesigninsessionss"
}-->
```http
POST https://graph.microsoft.com/beta/me/revokeSignInSessions
```

##### <a name="response"></a><span data-ttu-id="59b27-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="59b27-134">Response</span></span>
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
  "suppressions": []
}
-->
