---
title: 'пользователь: invalidateAllRefreshTokens'
description: Признает недействительным всех маркеров обновления пользователя, выданный приложений (а также файлы cookie сеанса в браузере пользователя), сброс свойство пользователя **refreshTokensValidFromDateTime** текущая дата и время. Как правило эта операция выполняется (по пользователь или администратор), если у пользователя есть потерянных или украденных устройств.  Эта операция может запретить доступ к любой из организации данных, доступных через приложения на устройстве без уведомления пользователя, сначала необходимо выполнить повторный вход. На самом деле эта операция будет принудительно пользователя выполнить повторный вход для всех приложений, которые они ранее согласие, вне зависимости от устройства.
ms.openlocfilehash: 23743c4bc372193a5478d79432b7bb4e0a9ec4ce
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081557"
---
# <a name="user-invalidateallrefreshtokens"></a><span data-ttu-id="2aa43-106">пользователь: invalidateAllRefreshTokens</span><span class="sxs-lookup"><span data-stu-id="2aa43-106">user: invalidateAllRefreshTokens</span></span>

> <span data-ttu-id="2aa43-107">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2aa43-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2aa43-108">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2aa43-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2aa43-109">Признает недействительным всех маркеров обновления пользователя, выданный приложений (а также файлы cookie сеанса в браузере пользователя), сброс свойство пользователя **refreshTokensValidFromDateTime** текущая дата и время.</span><span class="sxs-lookup"><span data-stu-id="2aa43-109">Invalidates all of the user's refresh tokens issued to applications (as well as session cookies in a user's browser), by resetting the **refreshTokensValidFromDateTime** user property to the current date-time.</span></span> <span data-ttu-id="2aa43-110">Как правило эта операция выполняется (по пользователь или администратор), если у пользователя есть потерянных или украденных устройств.</span><span class="sxs-lookup"><span data-stu-id="2aa43-110">Typically, this operation is performed (by the user or an administrator) if the user has a lost or stolen device.</span></span>  <span data-ttu-id="2aa43-111">Эта операция может запретить доступ к любой из организации данных, доступных через приложения на устройстве без уведомления пользователя, сначала необходимо выполнить повторный вход.</span><span class="sxs-lookup"><span data-stu-id="2aa43-111">This operation would prevent access to any of the organization's data accessed through applications on the device without the user first being required to sign in again.</span></span> <span data-ttu-id="2aa43-112">На самом деле эта операция будет принудительно пользователя выполнить повторный вход для всех приложений, которые они ранее согласие, вне зависимости от устройства.</span><span class="sxs-lookup"><span data-stu-id="2aa43-112">In fact, this operation would force the user to sign in again for all applications that they have previously consented to, independent of device.</span></span>

<span data-ttu-id="2aa43-113">Для разработчиков Если приложение пытается использовать маркер делегированные доступа для этого пользователя с помощью маркера недействительным обновления приложения появится сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="2aa43-113">For developers, if the application attempts to redeem a delegated access token for this user by using an invalidated refresh token, the application will get an error.</span></span> <span data-ttu-id="2aa43-114">В этом случае приложения необходимо получить новый маркер обновления при выполнении запроса к конечной точке авторизовать, которая отвечает за выполнение принудительной пользователи могут входить в.</span><span class="sxs-lookup"><span data-stu-id="2aa43-114">If this happens, the application will need to acquire a new refresh token by making a request to the authorize endpoint, which will force the user to sign in.</span></span>

## <a name="permissions"></a><span data-ttu-id="2aa43-115">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2aa43-115">Permissions</span></span>
<span data-ttu-id="2aa43-p105">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2aa43-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

+ <span data-ttu-id="2aa43-118">Приложение может разрешить подписанных в пользователю недействительными приложений они согласие на: User.ReadWrite, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2aa43-118">For an application to allow the signed in user to invalidate applications they've consented to: User.ReadWrite, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>
+ <span data-ttu-id="2aa43-119">Для приложения Разрешить администраторам недействительными приложений пользователя изъявил: Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2aa43-119">For an application to allow an administrator to invalidate applications a user has consented to: Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>

## <a name="http-request"></a><span data-ttu-id="2aa43-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2aa43-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/invalidateAllRefreshTokens
POST /users/{id | userPrincipalName}/invalidateAllRefreshTokens
```
## <a name="request-headers"></a><span data-ttu-id="2aa43-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2aa43-121">Request headers</span></span>
| <span data-ttu-id="2aa43-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2aa43-122">Header</span></span>       | <span data-ttu-id="2aa43-123">Значение</span><span class="sxs-lookup"><span data-stu-id="2aa43-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2aa43-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2aa43-124">Authorization</span></span>  | <span data-ttu-id="2aa43-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2aa43-p106">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2aa43-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2aa43-127">Request body</span></span>
<span data-ttu-id="2aa43-128">Эта операция не имеет запроса содержимого.</span><span class="sxs-lookup"><span data-stu-id="2aa43-128">This operation has no request content.</span></span>

## <a name="response"></a><span data-ttu-id="2aa43-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="2aa43-129">Response</span></span>

<span data-ttu-id="2aa43-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="2aa43-130">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2aa43-131">Пример</span><span class="sxs-lookup"><span data-stu-id="2aa43-131">Example</span></span>
<span data-ttu-id="2aa43-132">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="2aa43-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="2aa43-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="2aa43-133">Request</span></span>
<span data-ttu-id="2aa43-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2aa43-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_invalidateallrefreshtokens"
}-->
```http
POST https://graph.microsoft.com/beta/me/invalidateAllRefreshTokens
```

##### <a name="response"></a><span data-ttu-id="2aa43-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="2aa43-135">Response</span></span>
<span data-ttu-id="2aa43-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2aa43-136">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: invalidateAllRefreshTokens",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
