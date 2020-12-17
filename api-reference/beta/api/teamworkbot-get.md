---
title: Get teamworkBot
description: Чтение свойств и связей объекта teamworkBot.
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 33a6312474994ff65397f6d09b416d15560bb08c
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/17/2020
ms.locfileid: "49706491"
---
# <a name="get-teamworkbot"></a><span data-ttu-id="c9a2a-103">Get teamworkBot</span><span class="sxs-lookup"><span data-stu-id="c9a2a-103">Get teamworkBot</span></span>
<span data-ttu-id="c9a2a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c9a2a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c9a2a-105">Получите бота, связанного с определенным [определением](../resources/teamsappdefinition.md) [TeamsApp.](../resources/teamsapp.md)</span><span class="sxs-lookup"><span data-stu-id="c9a2a-105">Get the bot associated with a specific [definition](../resources/teamsappdefinition.md) of the  [TeamsApp](../resources/teamsapp.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c9a2a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c9a2a-106">Permissions</span></span>
<span data-ttu-id="c9a2a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9a2a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9a2a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c9a2a-109">Permission type</span></span>|<span data-ttu-id="c9a2a-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c9a2a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c9a2a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c9a2a-111">Delegated (work or school account)</span></span>| <span data-ttu-id="c9a2a-112">AppCatalog.Submit, AppCatalog.Read.All, AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9a2a-112">AppCatalog.Submit, AppCatalog.Read.All, AppCatalog.ReadWrite.All</span></span> |
|<span data-ttu-id="c9a2a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c9a2a-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="c9a2a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9a2a-114">Not supported.</span></span> |
|<span data-ttu-id="c9a2a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c9a2a-115">Application</span></span>| <span data-ttu-id="c9a2a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9a2a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c9a2a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c9a2a-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /appCatalogs/teamsApps/{app-id}/appDefinitions/{app-definition-id}/bot
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c9a2a-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c9a2a-118">Optional query parameters</span></span>
<span data-ttu-id="c9a2a-119">Этот метод поддерживает `$select` [параметры запросов OData](/graph/query-parameter) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="c9a2a-119">This method supports the `$select` [OData query parameters](/graph/query-parameter) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c9a2a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c9a2a-120">Request headers</span></span>
|<span data-ttu-id="c9a2a-121">Имя</span><span class="sxs-lookup"><span data-stu-id="c9a2a-121">Name</span></span>|<span data-ttu-id="c9a2a-122">Описание</span><span class="sxs-lookup"><span data-stu-id="c9a2a-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c9a2a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c9a2a-123">Authorization</span></span>|<span data-ttu-id="c9a2a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c9a2a-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c9a2a-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c9a2a-126">Request body</span></span>
<span data-ttu-id="c9a2a-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c9a2a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c9a2a-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9a2a-128">Response</span></span>

<span data-ttu-id="c9a2a-129">В случае успеха этот метод возвращает код отклика и объект `200 OK` [teamworkBot](../resources/teamworkbot.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c9a2a-129">If successful, this method returns a `200 OK` response code and a [teamworkBot](../resources/teamworkbot.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c9a2a-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="c9a2a-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c9a2a-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="c9a2a-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_teamworkbot"
}
-->
``` http
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps/e4c5c249-bb4b-419e-b7c5-b1d98559368b/appDefinitions/ZTRjNWMyNDktYmI0Yi00MTllLWI3YzUtYjFkOTg1NTkzNjhiIyMyLjAuMSMjUHVibGlzaGVk/bot
```


### <a name="response"></a><span data-ttu-id="c9a2a-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9a2a-132">Response</span></span>
<span data-ttu-id="c9a2a-133">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c9a2a-133">**Note:** The response object shown here might be shortened for readability.</span></span>
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
## <a name="see-also"></a><span data-ttu-id="c9a2a-134">См. также</span><span class="sxs-lookup"><span data-stu-id="c9a2a-134">See also</span></span>

- <span data-ttu-id="c9a2a-135">Чтобы получить ботов, установленных в команде, см. пример 2 в [списке приложений в команде.](team-list-installedapps.md)</span><span class="sxs-lookup"><span data-stu-id="c9a2a-135">To get bots installed in a team, see example 2 in [List apps in team](team-list-installedapps.md).</span></span>
- <span data-ttu-id="c9a2a-136">Чтобы получить боты, установленные в чате, см. пример 2 в [списке приложений в чате.](chat-list-installedapps.md)</span><span class="sxs-lookup"><span data-stu-id="c9a2a-136">To get bots installed in a chat, see example 2 in [List apps in chat](chat-list-installedapps.md).</span></span>
- <span data-ttu-id="c9a2a-137">Чтобы получить боты, установленные в личной области пользователя, см. пример 2 в списке [приложений, установленных для пользователя.](userteamwork-list-installedapps.md)</span><span class="sxs-lookup"><span data-stu-id="c9a2a-137">To get bots installed in the personal scope of a user, see example 2 in [List apps installed for user](userteamwork-list-installedapps.md).</span></span>


