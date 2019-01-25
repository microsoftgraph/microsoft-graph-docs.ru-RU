---
title: 'пользователь: invalidateAllRefreshTokens'
description: Признает недействительным всех маркеров обновления пользователя, выданный приложений (а также файлы cookie сеанса в браузере пользователя), сброс свойство пользователя **refreshTokensValidFromDateTime** текущая дата и время. Как правило эта операция выполняется (по пользователь или администратор), если у пользователя есть потерянных или украденных устройств.  Эта операция может запретить доступ к любой из организации данных, доступных через приложения на устройстве без уведомления пользователя, сначала необходимо выполнить повторный вход. На самом деле эта операция будет принудительно пользователя выполнить повторный вход для всех приложений, которые они ранее согласие, вне зависимости от устройства.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c006787c0d68ae0c6ecbb331a9ff410f957a6f93
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524529"
---
# <a name="user-invalidateallrefreshtokens"></a><span data-ttu-id="19e67-106">пользователь: invalidateAllRefreshTokens</span><span class="sxs-lookup"><span data-stu-id="19e67-106">user: invalidateAllRefreshTokens</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="19e67-107">Признает недействительным всех маркеров обновления пользователя, выданный приложений (а также файлы cookie сеанса в браузере пользователя), сброс свойство пользователя **refreshTokensValidFromDateTime** текущая дата и время.</span><span class="sxs-lookup"><span data-stu-id="19e67-107">Invalidates all of the user's refresh tokens issued to applications (as well as session cookies in a user's browser), by resetting the **refreshTokensValidFromDateTime** user property to the current date-time.</span></span> <span data-ttu-id="19e67-108">Как правило эта операция выполняется (по пользователь или администратор), если у пользователя есть потерянных или украденных устройств.</span><span class="sxs-lookup"><span data-stu-id="19e67-108">Typically, this operation is performed (by the user or an administrator) if the user has a lost or stolen device.</span></span>  <span data-ttu-id="19e67-109">Эта операция может запретить доступ к любой из организации данных, доступных через приложения на устройстве без уведомления пользователя, сначала необходимо выполнить повторный вход.</span><span class="sxs-lookup"><span data-stu-id="19e67-109">This operation would prevent access to any of the organization's data accessed through applications on the device without the user first being required to sign in again.</span></span> <span data-ttu-id="19e67-110">На самом деле эта операция будет принудительно пользователя выполнить повторный вход для всех приложений, которые они ранее согласие, вне зависимости от устройства.</span><span class="sxs-lookup"><span data-stu-id="19e67-110">In fact, this operation would force the user to sign in again for all applications that they have previously consented to, independent of device.</span></span>

<span data-ttu-id="19e67-111">Для разработчиков Если приложение пытается использовать маркер делегированные доступа для этого пользователя с помощью маркера недействительным обновления приложения появится сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="19e67-111">For developers, if the application attempts to redeem a delegated access token for this user by using an invalidated refresh token, the application will get an error.</span></span> <span data-ttu-id="19e67-112">В этом случае приложения необходимо получить новый маркер обновления при выполнении запроса к конечной точке авторизовать, которая отвечает за выполнение принудительной пользователи могут входить в.</span><span class="sxs-lookup"><span data-stu-id="19e67-112">If this happens, the application will need to acquire a new refresh token by making a request to the authorize endpoint, which will force the user to sign in.</span></span>

## <a name="permissions"></a><span data-ttu-id="19e67-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="19e67-113">Permissions</span></span>
<span data-ttu-id="19e67-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="19e67-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

+ <span data-ttu-id="19e67-116">Приложение может разрешить подписанных в пользователю недействительными приложений они согласие на: User.ReadWrite, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="19e67-116">For an application to allow the signed in user to invalidate applications they've consented to: User.ReadWrite, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>
+ <span data-ttu-id="19e67-117">Для приложения Разрешить администраторам недействительными приложений пользователя изъявил: Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="19e67-117">For an application to allow an administrator to invalidate applications a user has consented to: Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>

## <a name="http-request"></a><span data-ttu-id="19e67-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="19e67-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/invalidateAllRefreshTokens
POST /users/{id | userPrincipalName}/invalidateAllRefreshTokens
```
## <a name="request-headers"></a><span data-ttu-id="19e67-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="19e67-119">Request headers</span></span>
| <span data-ttu-id="19e67-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="19e67-120">Header</span></span>       | <span data-ttu-id="19e67-121">Значение</span><span class="sxs-lookup"><span data-stu-id="19e67-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="19e67-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="19e67-122">Authorization</span></span>  | <span data-ttu-id="19e67-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="19e67-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="19e67-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="19e67-125">Request body</span></span>
<span data-ttu-id="19e67-126">Эта операция не имеет запроса содержимого.</span><span class="sxs-lookup"><span data-stu-id="19e67-126">This operation has no request content.</span></span>

## <a name="response"></a><span data-ttu-id="19e67-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="19e67-127">Response</span></span>

<span data-ttu-id="19e67-128">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="19e67-128">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="19e67-129">Пример</span><span class="sxs-lookup"><span data-stu-id="19e67-129">Example</span></span>
<span data-ttu-id="19e67-130">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="19e67-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="19e67-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="19e67-131">Request</span></span>
<span data-ttu-id="19e67-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="19e67-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_invalidateallrefreshtokens"
}-->
```http
POST https://graph.microsoft.com/beta/me/invalidateAllRefreshTokens
```

##### <a name="response"></a><span data-ttu-id="19e67-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="19e67-133">Response</span></span>
<span data-ttu-id="19e67-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="19e67-134">Here is an example of the response.</span></span> 
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
    "Error: /api-reference/beta/api/user-invalidateallrefreshtokens.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
