---
title: Получить командную работуBot
description: Ознакомьтесь с свойствами и отношениями объекта teamworkBot.
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: c77153aa36628edeb9b1a4ab2100b6acf38c0ea5
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50476432"
---
# <a name="get-teamworkbot"></a><span data-ttu-id="86285-103">Получить командную работуBot</span><span class="sxs-lookup"><span data-stu-id="86285-103">Get teamworkBot</span></span>

<span data-ttu-id="86285-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="86285-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="86285-105">Получите бот, связанный с определенным [определением](../resources/teamsappdefinition.md) [TeamsApp.](../resources/teamsapp.md)</span><span class="sxs-lookup"><span data-stu-id="86285-105">Get the bot associated with a specific [definition](../resources/teamsappdefinition.md) of the  [TeamsApp](../resources/teamsapp.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="86285-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="86285-106">Permissions</span></span>
<span data-ttu-id="86285-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="86285-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86285-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="86285-109">Permission type</span></span>|<span data-ttu-id="86285-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="86285-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="86285-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="86285-111">Delegated (work or school account)</span></span>| <span data-ttu-id="86285-112">AppCatalog.Read.All, AppCatalog.ReadWrite.All, AppCatalog.Submit</span><span class="sxs-lookup"><span data-stu-id="86285-112">AppCatalog.Read.All, AppCatalog.ReadWrite.All, AppCatalog.Submit</span></span> |
|<span data-ttu-id="86285-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="86285-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="86285-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="86285-114">Not supported.</span></span> |
|<span data-ttu-id="86285-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="86285-115">Application</span></span>| <span data-ttu-id="86285-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="86285-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="86285-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="86285-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /appCatalogs/teamsApps/{app-id}/appDefinitions/{app-definition-id}/bot
```

## <a name="optional-query-parameters"></a><span data-ttu-id="86285-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="86285-118">Optional query parameters</span></span>
<span data-ttu-id="86285-119">Этот метод поддерживает `$select` [параметры запросов OData](/graph/query-parameter) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="86285-119">This method supports the `$select` [OData query parameters](/graph/query-parameter) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="86285-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="86285-120">Request headers</span></span>
|<span data-ttu-id="86285-121">Имя</span><span class="sxs-lookup"><span data-stu-id="86285-121">Name</span></span>|<span data-ttu-id="86285-122">Описание</span><span class="sxs-lookup"><span data-stu-id="86285-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="86285-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="86285-123">Authorization</span></span>|<span data-ttu-id="86285-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="86285-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="86285-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="86285-126">Request body</span></span>
<span data-ttu-id="86285-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="86285-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="86285-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="86285-128">Response</span></span>

<span data-ttu-id="86285-129">В случае успешной работы этот метод возвращает код отклика и объект `200 OK` [teamworkBot](../resources/teamworkbot.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="86285-129">If successful, this method returns a `200 OK` response code and a [teamworkBot](../resources/teamworkbot.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="86285-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="86285-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="86285-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="86285-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_teamworkbot"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/e4c5c249-bb4b-419e-b7c5-b1d98559368b/appDefinitions/ZTRjNWMyNDktYmI0Yi00MTllLWI3YzUtYjFkOTg1NTkzNjhiIyMyLjAuMSMjUHVibGlzaGVk/bot
```

### <a name="response"></a><span data-ttu-id="86285-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="86285-132">Response</span></span>
<span data-ttu-id="86285-133">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="86285-133">**Note:** The response object shown here might be shortened for readability.</span></span>
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
## <a name="see-also"></a><span data-ttu-id="86285-134">См. также</span><span class="sxs-lookup"><span data-stu-id="86285-134">See also</span></span>

- <span data-ttu-id="86285-135">Чтобы получить боты, установленные в команде, см. пример 2 в [списке приложений в команде.](team-list-installedapps.md)</span><span class="sxs-lookup"><span data-stu-id="86285-135">To get bots installed in a team, see example 2 in [List apps in team](team-list-installedapps.md).</span></span> <!-- - To get bots installed in a chat, see example 2 in [List apps in chat](chat-list-installedapps.md). -->
- <span data-ttu-id="86285-136">Чтобы получить боты, установленные в личной области пользователя, см. пример 2 в [приложениях List, установленных для пользователя.](userteamwork-list-installedapps.md)</span><span class="sxs-lookup"><span data-stu-id="86285-136">To get bots installed in the personal scope of a user, see example 2 in [List apps installed for user](userteamwork-list-installedapps.md).</span></span>


