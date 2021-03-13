---
title: Получить командную работуBot
description: Ознакомьтесь с свойствами и отношениями объекта teamworkBot.
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 3efbbf65c12e81f3c1ce243e97ad9e2bc98c4d0d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50774780"
---
# <a name="get-teamworkbot"></a><span data-ttu-id="a4bea-103">Получить командную работуBot</span><span class="sxs-lookup"><span data-stu-id="a4bea-103">Get teamworkBot</span></span>

<span data-ttu-id="a4bea-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4bea-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a4bea-105">Получите бот, связанный с определенным [определением](../resources/teamsappdefinition.md) [TeamsApp.](../resources/teamsapp.md)</span><span class="sxs-lookup"><span data-stu-id="a4bea-105">Get the bot associated with a specific [definition](../resources/teamsappdefinition.md) of the  [TeamsApp](../resources/teamsapp.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a4bea-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a4bea-106">Permissions</span></span>
<span data-ttu-id="a4bea-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a4bea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4bea-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a4bea-109">Permission type</span></span>|<span data-ttu-id="a4bea-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a4bea-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a4bea-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a4bea-111">Delegated (work or school account)</span></span>| <span data-ttu-id="a4bea-112">AppCatalog.Read.All, AppCatalog.ReadWrite.All, AppCatalog.Submit</span><span class="sxs-lookup"><span data-stu-id="a4bea-112">AppCatalog.Read.All, AppCatalog.ReadWrite.All, AppCatalog.Submit</span></span> |
|<span data-ttu-id="a4bea-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a4bea-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="a4bea-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a4bea-114">Not supported.</span></span> |
|<span data-ttu-id="a4bea-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a4bea-115">Application</span></span>| <span data-ttu-id="a4bea-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a4bea-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a4bea-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a4bea-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /appCatalogs/teamsApps/{app-id}/appDefinitions/{app-definition-id}/bot
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a4bea-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a4bea-118">Optional query parameters</span></span>
<span data-ttu-id="a4bea-119">Этот метод поддерживает `$select` [параметры запросов OData](/graph/query-parameter) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="a4bea-119">This method supports the `$select` [OData query parameters](/graph/query-parameter) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a4bea-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a4bea-120">Request headers</span></span>
|<span data-ttu-id="a4bea-121">Имя</span><span class="sxs-lookup"><span data-stu-id="a4bea-121">Name</span></span>|<span data-ttu-id="a4bea-122">Описание</span><span class="sxs-lookup"><span data-stu-id="a4bea-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a4bea-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a4bea-123">Authorization</span></span>|<span data-ttu-id="a4bea-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a4bea-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4bea-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a4bea-126">Request body</span></span>
<span data-ttu-id="a4bea-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a4bea-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a4bea-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="a4bea-128">Response</span></span>

<span data-ttu-id="a4bea-129">В случае успешной работы этот метод возвращает код отклика и объект `200 OK` [teamworkBot](../resources/teamworkbot.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a4bea-129">If successful, this method returns a `200 OK` response code and a [teamworkBot](../resources/teamworkbot.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a4bea-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="a4bea-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a4bea-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="a4bea-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="a4bea-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="a4bea-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_teamworkbot"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/e4c5c249-bb4b-419e-b7c5-b1d98559368b/appDefinitions/ZTRjNWMyNDktYmI0Yi00MTllLWI3YzUtYjFkOTg1NTkzNjhiIyMyLjAuMSMjUHVibGlzaGVk/bot
```
# <a name="c"></a>[<span data-ttu-id="a4bea-133">C#</span><span class="sxs-lookup"><span data-stu-id="a4bea-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-teamworkbot-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a4bea-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a4bea-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-teamworkbot-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a4bea-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a4bea-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-teamworkbot-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a4bea-136">Java</span><span class="sxs-lookup"><span data-stu-id="a4bea-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-teamworkbot-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a4bea-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="a4bea-137">Response</span></span>
<span data-ttu-id="a4bea-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a4bea-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamworkBot"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.teamworkBot",
  "id": "1f81bb29-bb29-1f81-29bb-811f29bb811f"
}
```
## <a name="see-also"></a><span data-ttu-id="a4bea-139">См. также</span><span class="sxs-lookup"><span data-stu-id="a4bea-139">See also</span></span>

- <span data-ttu-id="a4bea-140">Чтобы получить боты, установленные в команде, см. пример 2 в [списке приложений в команде.](team-list-installedapps.md)</span><span class="sxs-lookup"><span data-stu-id="a4bea-140">To get bots installed in a team, see example 2 in [List apps in team](team-list-installedapps.md).</span></span> <!-- - To get bots installed in a chat, see example 2 in [List apps in chat](chat-list-installedapps.md). -->
- <span data-ttu-id="a4bea-141">Чтобы получить боты, установленные в личной области пользователя, см. пример 2 в [приложениях List, установленных для пользователя.](userteamwork-list-installedapps.md)</span><span class="sxs-lookup"><span data-stu-id="a4bea-141">To get bots installed in the personal scope of a user, see example 2 in [List apps installed for user](userteamwork-list-installedapps.md).</span></span>


