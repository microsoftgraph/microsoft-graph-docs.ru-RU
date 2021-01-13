---
title: Get teamworkBot
description: Чтение свойств и связей объекта teamworkBot.
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: b0c0eaecb59140450d365c0eee931156b8b99e16
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/13/2021
ms.locfileid: "49844725"
---
# <a name="get-teamworkbot"></a><span data-ttu-id="a794e-103">Get teamworkBot</span><span class="sxs-lookup"><span data-stu-id="a794e-103">Get teamworkBot</span></span>

<span data-ttu-id="a794e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a794e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a794e-105">Получите бота, связанного с определенным [определением](../resources/teamsappdefinition.md) [TeamsApp.](../resources/teamsapp.md)</span><span class="sxs-lookup"><span data-stu-id="a794e-105">Get the bot associated with a specific [definition](../resources/teamsappdefinition.md) of the  [TeamsApp](../resources/teamsapp.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a794e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a794e-106">Permissions</span></span>
<span data-ttu-id="a794e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a794e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a794e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a794e-109">Permission type</span></span>|<span data-ttu-id="a794e-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a794e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a794e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a794e-111">Delegated (work or school account)</span></span>| <span data-ttu-id="a794e-112">AppCatalog.Submit, AppCatalog.Read.All, AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a794e-112">AppCatalog.Submit, AppCatalog.Read.All, AppCatalog.ReadWrite.All</span></span> |
|<span data-ttu-id="a794e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a794e-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="a794e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a794e-114">Not supported.</span></span> |
|<span data-ttu-id="a794e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a794e-115">Application</span></span>| <span data-ttu-id="a794e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a794e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a794e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a794e-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /appCatalogs/teamsApps/{app-id}/appDefinitions/{app-definition-id}/bot
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a794e-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a794e-118">Optional query parameters</span></span>
<span data-ttu-id="a794e-119">Этот метод поддерживает `$select` [параметры запросов OData](/graph/query-parameter) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="a794e-119">This method supports the `$select` [OData query parameters](/graph/query-parameter) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a794e-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a794e-120">Request headers</span></span>
|<span data-ttu-id="a794e-121">Имя</span><span class="sxs-lookup"><span data-stu-id="a794e-121">Name</span></span>|<span data-ttu-id="a794e-122">Описание</span><span class="sxs-lookup"><span data-stu-id="a794e-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a794e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a794e-123">Authorization</span></span>|<span data-ttu-id="a794e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a794e-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a794e-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a794e-126">Request body</span></span>
<span data-ttu-id="a794e-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a794e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a794e-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="a794e-128">Response</span></span>

<span data-ttu-id="a794e-129">В случае успеха этот метод возвращает код отклика и объект `200 OK` [teamworkBot](../resources/teamworkbot.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a794e-129">If successful, this method returns a `200 OK` response code and a [teamworkBot](../resources/teamworkbot.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a794e-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="a794e-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a794e-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="a794e-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="a794e-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="a794e-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_teamworkbot"
}
-->
``` http
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps/e4c5c249-bb4b-419e-b7c5-b1d98559368b/appDefinitions/ZTRjNWMyNDktYmI0Yi00MTllLWI3YzUtYjFkOTg1NTkzNjhiIyMyLjAuMSMjUHVibGlzaGVk/bot
```
# <a name="c"></a>[<span data-ttu-id="a794e-133">C#</span><span class="sxs-lookup"><span data-stu-id="a794e-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-teamworkbot-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a794e-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a794e-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-teamworkbot-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a794e-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a794e-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-teamworkbot-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a794e-136">Java</span><span class="sxs-lookup"><span data-stu-id="a794e-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-teamworkbot-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="a794e-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="a794e-137">Response</span></span>
<span data-ttu-id="a794e-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a794e-138">**Note:** The response object shown here might be shortened for readability.</span></span>
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
## <a name="see-also"></a><span data-ttu-id="a794e-139">См. также</span><span class="sxs-lookup"><span data-stu-id="a794e-139">See also</span></span>

- <span data-ttu-id="a794e-140">Чтобы получить боты, установленные в команде, см. пример 2 в [списке приложений в команде.](team-list-installedapps.md)</span><span class="sxs-lookup"><span data-stu-id="a794e-140">To get bots installed in a team, see example 2 in [List apps in team](team-list-installedapps.md).</span></span>
- <span data-ttu-id="a794e-141">Чтобы получить боты, установленные в чате, см. пример 2 в [списке приложений в чате.](chat-list-installedapps.md)</span><span class="sxs-lookup"><span data-stu-id="a794e-141">To get bots installed in a chat, see example 2 in [List apps in chat](chat-list-installedapps.md).</span></span>
- <span data-ttu-id="a794e-142">Чтобы получить боты, установленные в личной области пользователя, см. пример 2 в списке [приложений, установленных для пользователя.](userteamwork-list-installedapps.md)</span><span class="sxs-lookup"><span data-stu-id="a794e-142">To get bots installed in the personal scope of a user, see example 2 in [List apps installed for user](userteamwork-list-installedapps.md).</span></span>


