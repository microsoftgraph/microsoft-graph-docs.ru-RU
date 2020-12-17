---
title: Список чатов
description: Получить список чатов для пользователя.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 629f64883dd28bd4c0b248c61232f5399794b36f
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/17/2020
ms.locfileid: "49705832"
---
# <a name="list-chats"></a><span data-ttu-id="11c9f-103">Список чатов</span><span class="sxs-lookup"><span data-stu-id="11c9f-103">List chats</span></span>

<span data-ttu-id="11c9f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11c9f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="11c9f-105">Получить список [чатов,](../resources/chat.md) в которые входит пользователь.</span><span class="sxs-lookup"><span data-stu-id="11c9f-105">Retrieve the list of [chats](../resources/chat.md) that the user is part of.</span></span>

## <a name="permissions"></a><span data-ttu-id="11c9f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="11c9f-106">Permissions</span></span>

<span data-ttu-id="11c9f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11c9f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="11c9f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="11c9f-109">Permission type</span></span>      | <span data-ttu-id="11c9f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="11c9f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="11c9f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="11c9f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="11c9f-112">Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="11c9f-112">Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span></span> |
|<span data-ttu-id="11c9f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="11c9f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="11c9f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="11c9f-114">Not supported.</span></span>    |
|<span data-ttu-id="11c9f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="11c9f-115">Application</span></span> | <span data-ttu-id="11c9f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="11c9f-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="11c9f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="11c9f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/chats
GET /users/{user-id}/chats
GET /chats
```

## <a name="optional-query-parameters"></a><span data-ttu-id="11c9f-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="11c9f-118">Optional query parameters</span></span>

<span data-ttu-id="11c9f-119">Этот метод поддерживает (только для свойства members) и параметры запроса `$expand`  `$filter` [OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="11c9f-119">This method supports the `$expand` (only for the **members** property) and `$filter` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="11c9f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="11c9f-120">Request headers</span></span>

| <span data-ttu-id="11c9f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="11c9f-121">Header</span></span>       | <span data-ttu-id="11c9f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="11c9f-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="11c9f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="11c9f-123">Authorization</span></span>  | <span data-ttu-id="11c9f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="11c9f-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="11c9f-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="11c9f-126">Request body</span></span>

<span data-ttu-id="11c9f-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="11c9f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="11c9f-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="11c9f-128">Response</span></span>

<span data-ttu-id="11c9f-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [chat](../resources/chat.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="11c9f-129">If successful, this method returns a `200 OK` response code and a collection of [chat](../resources/chat.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="11c9f-130">Пример</span><span class="sxs-lookup"><span data-stu-id="11c9f-130">Example</span></span>

### <a name="example-1-list-all-the-chats"></a><span data-ttu-id="11c9f-131">Пример 1. Список всех чатов</span><span class="sxs-lookup"><span data-stu-id="11c9f-131">Example 1: List all the chats</span></span>

#### <a name="request"></a><span data-ttu-id="11c9f-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="11c9f-132">Request</span></span>

<span data-ttu-id="11c9f-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="11c9f-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="11c9f-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="11c9f-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_chats"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5/chats
```

---

#### <a name="response"></a><span data-ttu-id="11c9f-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="11c9f-135">Response</span></span>

<span data-ttu-id="11c9f-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="11c9f-136">Here is an example of the response.</span></span> 

><span data-ttu-id="11c9f-137">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="11c9f-137">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chat",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#chats",
    "@odata.count": 3,
    "value": [
        {
            "id": "19:meeting_MjdhNjM4YzUtYzExZi00OTFkLTkzZTAtNTVlNmZmMDhkNGU2@thread.v2",
            "topic": "Meeting chat sample",
            "createdDateTime": "2020-12-08T23:53:05.801Z",
            "lastUpdatedDateTime": "2020-12-08T23:58:32.511Z",
            "chatType": "meeting"
        },
        {
            "id": "19:561082c0f3f847a58069deb8eb300807@thread.v2",
            "topic": "Group chat sample",
            "createdDateTime": "2020-12-03T19:41:07.054Z",
            "lastUpdatedDateTime": "2020-12-08T23:53:11.012Z",
            "chatType": "group"
        },
        {
            "id": "19:d74fc2ed-cb0e-4288-a219-b5c71abaf2aa_8c0a1a67-50ce-4114-bb6c-da9c5dbcf6ca@unq.gbl.spaces",
            "topic": null,
            "createdDateTime": "2020-12-04T23:10:28.51Z",
            "lastUpdatedDateTime": "2020-12-04T23:10:36.925Z",
            "chatType": "oneOnOne"
        }
    ]
}
```

### <a name="example-2-list-all-the-chats-along-with-the-members-of-each-chat"></a><span data-ttu-id="11c9f-138">Пример 2. Список всех чатов вместе с участниками каждого чата</span><span class="sxs-lookup"><span data-stu-id="11c9f-138">Example 2: List all the chats along with the members of each chat</span></span>
#### <a name="request"></a><span data-ttu-id="11c9f-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="11c9f-139">Request</span></span>

<span data-ttu-id="11c9f-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="11c9f-140">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="11c9f-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="11c9f-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_chats_expand_members"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5/chats?$expand=members
```

---

#### <a name="response"></a><span data-ttu-id="11c9f-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="11c9f-142">Response</span></span>

<span data-ttu-id="11c9f-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="11c9f-143">Here is an example of the response.</span></span> 

> [!NOTE]
> <span data-ttu-id="11c9f-144">Идентификаторы членства, возвращаемые сервером, должны рассматриваться как непрозрачные строки.</span><span class="sxs-lookup"><span data-stu-id="11c9f-144">The membership IDs returned by the server must be treated as opaque strings.</span></span> <span data-ttu-id="11c9f-145">Клиент не должен пытаться анализировать или делать какие-либо предположения об этих идентификаторах ресурсов.</span><span class="sxs-lookup"><span data-stu-id="11c9f-145">The client should not try to parse or make any assumptions about these resource IDs.</span></span>
>
> <span data-ttu-id="11c9f-146">Результаты членства могут быть соединимы с пользователями из разных клиентов, как указано в ответе, в будущем.</span><span class="sxs-lookup"><span data-stu-id="11c9f-146">The membership results can map to users from different tenants, as indicated in the response, in the future.</span></span> <span data-ttu-id="11c9f-147">Клиент не должен предполагать, что все участники относятся только к текущему клиенту.</span><span class="sxs-lookup"><span data-stu-id="11c9f-147">The client should not assume that all members are from the current tenant only.</span></span>

><span data-ttu-id="11c9f-148">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="11c9f-148">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chat",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#chats(members())",
    "@odata.count": 3,
    "value": [
        {
            "id": "19:meeting_MjdhNjM4YzUtYzExZi00OTFkLTkzZTAtNTVlNmZmMDhkNGU2@thread.v2",
            "topic": "Meeting chat sample",
            "createdDateTime": "2020-12-08T23:53:05.801Z",
            "lastUpdatedDateTime": "2020-12-08T23:58:32.511Z",
            "chatType": "meeting",
            "members@odata.context": "https://graph.microsoft.com/beta/$metadata#chats('19%3Ameeting_MjdhNjM4YzUtYzExZi00OTFkLTkzZTAtNTVlNmZmMDhkNGU2%40thread.v2')/members",
            "members": [
                {
                    "@odata.type": "#microsoft.graph.aadUserConversationMember",
                    "id": "MmFiOWM3OTYtMjkwMi00NWY4LWI3MTItN2M1YTYzY2Y0MWM0IyNlZWY5Y2IzNi0wNmRlLTQ2OWItODdjZC03MGY0Y2JlMzJkM123=",
                    "roles": [],
                    "displayName": "Tony Stark",
                    "userId": "4595d2f2-7b31-446c-84fd-9b795e63114b",
                    "email": "starkt@teamsgraph.onmicrosoft.com"
                },
                {
                    "@odata.type": "#microsoft.graph.aadUserConversationMember",
                    "id": "MmFiOWM3OTYtMjkwMi00NWY4LWI3MTItN2M1YTYzY2Y0MWM0IyNlZWY5Y2IzNi0wNmRlLTQ2OWItODdjZC03MGY0Y2JlMz6Jk45=",
                    "roles": [],
                    "displayName": "Peter Parker",
                    "userId": "d74fc2ed-cb0e-4288-a219-b5c71abaf2aa",
                    "email": "parkerp@teamsgraph.onmicrosoft.com"
                },
                {
                    "@odata.type": "#microsoft.graph.aadUserConversationMember",
                    "id": "MmFiOWM3OTYtMjkwMi00NWY4LWI3MTItN2M1YTYzY2Y0MWM0IyNlZWY5Y2IzNi0wNmRlLTQ2OWItODdjZC03MGY0Y2JlMzJ989kMTQ=",
                    "roles": [],
                    "displayName": "Nick Fury",
                    "userId": "8c0a1a67-50ce-4114-bb6c-da9c5dbcf6ca",
                    "email": "furyn@teamsgraph.onmicrosoft.com"
                }
            ]
        },
        {
            "id": "19:561082c0f3f847a58069deb8eb300807@thread.v2",
            "topic": "Group chat sample",
            "createdDateTime": "2020-12-03T19:41:07.054Z",
            "lastUpdatedDateTime": "2020-12-08T23:53:11.012Z",
            "chatType": "group",
            "members@odata.context": "https://graph.microsoft.com/beta/$metadata#chats('19%3A561082c0f3f847a58069deb8eb300807%40thread.v2')/members",
            "members": [
                {
                    "@odata.type": "#microsoft.graph.aadUserConversationMember",
                    "id": "MmFiOWM3OTYtMjkwMi00NWY4LWI3MTItN2M1YTYzY2Y0MWM0IyNlZWY5Y2IzNi0wNmRlLTQ2OWItODdjZC03MGY0Y2JlMzJkM123=",
                    "roles": [],
                    "displayName": "Tony Stark",
                    "userId": "4595d2f2-7b31-446c-84fd-9b795e63114b",
                    "email": "starkt@teamsgraph.onmicrosoft.com"
                },
                {
                    "@odata.type": "#microsoft.graph.aadUserConversationMember",
                    "id": "MmFiOWM312ftMjkwMi00NWY4LWI3MTItN2M1YTYzY2Y0MWM0IyNlZWY5Y2IzNi0wNmRlLTQ2OWItODdjZC03MGY0Y2JlMzJkM123=",
                    "roles": [],
                    "displayName": "Bruce Banner",
                    "userId": "48bf9d52-dca7-4a5f-8398-37b95cc7bd83",
                    "email": "bannerb@teamsgraph.onmicrosoft.com"
                },
                {
                    "@odata.type": "#microsoft.graph.aadUserConversationMember",
                    "id": "MmFiOWM3OTYtMjkwMi00NWY4LWai3MTetN2M1YTYzY2Y0MWM0IyNlZWY5Y2IzNi0wNmRlLTQ2OWItODdjZC03MGY0Y2JlMzJkM123=",
                    "roles": [],
                    "displayName": "TChalla",
                    "userId": "9efb1aea-4f83-4673-bdcd-d3f3c7be28c2",
                    "email": "tchalla@teamsgraph.onmicrosoft.com"
                },
                {
                    "@odata.type": "#microsoft.graph.aadUserConversationMember",
                    "id": "MmFiOWM3OTYtMjkwamii00NWY4LWI3MTItN2M1YTYzY2Y0MWM0IyNlZWY5Y2IzNi0wNmRlLTQ2OWItODdjZC03MGY0Y2JlMzJkM123=",
                    "roles": [],
                    "displayName": "Thor Odinson",
                    "userId": "976f4b31-fd01-4e0b-9178-29cc40c14438",
                    "email": "odinsont@teamsgraph.onmicrosoft.com"
                },
                {
                    "@odata.type": "#microsoft.graph.aadUserConversationMember",
                    "id": "MmFiOWM3OTYtMjkwMi00NWopiLWI3MTItN2M1YTYzY2Y0MWM0IyNlZWY5Y2IzNi0wNmRlLTQ2OWItODdjZC03MGY0Y2JlMzJkM123=",
                    "roles": [],
                    "displayName": "Steve Rogers",
                    "userId": "976f4b31-fd01-4e0b-9178-29cc40c14438",
                    "email": "rogerss@teamsgraph.onmicrosoft.com"
                }
            ]
        },
        {
            "id": "19:d74fc2ed-cb0e-4288-a219-b5c71abaf2aa_8c0a1a67-50ce-4114-bb6c-da9c5dbcf6ca@unq.gbl.spaces",
            "topic": null,
            "createdDateTime": "2020-12-04T23:10:28.51Z",
            "lastUpdatedDateTime": "2020-12-04T23:10:36.925Z",
            "chatType": "oneOnOne",
            "members@odata.context": "https://graph.microsoft.com/beta/$metadata#chats('19%3Ad74fc2ed-cb0e-4288-a219-b5c71abaf2aa_8c0a1a67-50ce-4114-bb6c-da9c5dbcf6ca%40unq.gbl.spaces')/members",
            "members": [
                {
                    "@odata.type": "#microsoft.graph.aadUserConversationMember",
                    "id": "MmFiOWM3OTYtMjkwMi00NWY4LWI3MTItN2M1YTYzY2Y0MWM0IyNlZWY5Y2IzNi0wNmRlLTQ2OWItODdjZC03MGY0Y2JlMzJ989kMTQ=",
                    "roles": [],
                    "displayName": "Nick Fury",
                    "userId": "8c0a1a67-50ce-4114-bb6c-da9c5dbcf6ca",
                    "email": "furyn@teamsgraph.onmicrosoft.com"
                },
                {
                    "@odata.type": "#microsoft.graph.aadUserConversationMember",
                    "id": "MmFiOWM3OTYtMjkwMi00NWY4LWI3MTItN2M1YTYzY2Y0MWM0IyNlZWY5Y2IzNi0wNmRlLTQ2OWItODdjZC03MGY0Y2JlMz6Jk45=",
                    "roles": [],
                    "displayName": "Peter Parker",
                    "userId": "d74fc2ed-cb0e-4288-a219-b5c71abaf2aa",
                    "email": "parkerp@teamsgraph.onmicrosoft.com"
                }
            ]
        }
    ]
}
```

### <a name="example-3-list-all-the-chats-that-have-a-member-with-a-specific-display-name"></a><span data-ttu-id="11c9f-149">Пример 3. Список всех чатов с участником с определенным отображаемой именем</span><span class="sxs-lookup"><span data-stu-id="11c9f-149">Example 3: List all the chats that have a member with a specific display name</span></span>

#### <a name="request"></a><span data-ttu-id="11c9f-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="11c9f-150">Request</span></span>

<span data-ttu-id="11c9f-151">Ниже показан пример запроса, который будет фильтровать все чаты на основе отображаемого имени определенного участника.</span><span class="sxs-lookup"><span data-stu-id="11c9f-151">Here is an example of a request that will filter all the chats based on a specific member's display name.</span></span>

# <a name="http"></a>[<span data-ttu-id="11c9f-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="11c9f-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_chats_expand_members_and_filter"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5/chats?$expand=members&$filter=members/any(o: o/displayname eq 'Peter Parker')
```

---

#### <a name="response"></a><span data-ttu-id="11c9f-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="11c9f-153">Response</span></span>

<span data-ttu-id="11c9f-154">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="11c9f-154">Here is an example of the response.</span></span> 

> [!NOTE]
> <span data-ttu-id="11c9f-155">Идентификатор членства, возвращенный сервером, должен рассматриваться как непрозрачные строки.</span><span class="sxs-lookup"><span data-stu-id="11c9f-155">The membership ID returned by server must be treated as opaque strings.</span></span> <span data-ttu-id="11c9f-156">Клиент не должен пытаться анализировать или делать какие-либо предположения об этих идентификаторах ресурсов.</span><span class="sxs-lookup"><span data-stu-id="11c9f-156">The client should not try to parse or make any assumptions about these resource IDs.</span></span>
>
> <span data-ttu-id="11c9f-157">В дальнейшем результаты членства могут сопоставляться с пользователями различных клиентов, как указано в отклике.</span><span class="sxs-lookup"><span data-stu-id="11c9f-157">The membership results could map to users from different tenants, as indicated in the response, in the future.</span></span> <span data-ttu-id="11c9f-158">Клиент не должен предполагать, что все участники относятся только к текущему клиенту.</span><span class="sxs-lookup"><span data-stu-id="11c9f-158">The client should not assume that all members are from the current tenant only.</span></span>

><span data-ttu-id="11c9f-159">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="11c9f-159">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chat",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#chats(members())",
    "@odata.count": 2,
    "value": [
        {
            "id": "19:meeting_MjdhNjM4YzUtYzExZi00OTFkLTkzZTAtNTVlNmZmMDhkNGU2@thread.v2",
            "topic": "Meeting chat sample",
            "createdDateTime": "2020-12-08T23:53:05.801Z",
            "lastUpdatedDateTime": "2020-12-08T23:58:32.511Z",
            "chatType": "meeting",
            "members@odata.context": "https://graph.microsoft.com/beta/$metadata#chats('19%3Ameeting_MjdhNjM4YzUtYzExZi00OTFkLTkzZTAtNTVlNmZmMDhkNGU2%40thread.v2')/members",
            "members": [
                {
                    "@odata.type": "#microsoft.graph.aadUserConversationMember",
                    "id": "MmFiOWM3OTYtMjkwMi00NWY4LWI3MTItN2M1YTYzY2Y0MWM0IyNlZWY5Y2IzNi0wNmRlLTQ2OWItODdjZC03MGY0Y2JlMzJkM123=",
                    "roles": [],
                    "displayName": "Tony Stark",
                    "userId": "4595d2f2-7b31-446c-84fd-9b795e63114b",
                    "email": "starkt@teamsgraph.onmicrosoft.com"
                },
                {
                    "@odata.type": "#microsoft.graph.aadUserConversationMember",
                    "id": "MmFiOWM3OTYtMjkwMi00NWY4LWI3MTItN2M1YTYzY2Y0MWM0IyNlZWY5Y2IzNi0wNmRlLTQ2OWItODdjZC03MGY0Y2JlMz6Jk45=",
                    "roles": [],
                    "displayName": "Peter Parker",
                    "userId": "d74fc2ed-cb0e-4288-a219-b5c71abaf2aa",
                    "email": "parkerp@teamsgraph.onmicrosoft.com"
                },
                {
                    "@odata.type": "#microsoft.graph.aadUserConversationMember",
                    "id": "MmFiOWM3OTYtMjkwMi00NWY4LWI3MTItN2M1YTYzY2Y0MWM0IyNlZWY5Y2IzNi0wNmRlLTQ2OWItODdjZC03MGY0Y2JlMzJ989kMTQ=",
                    "roles": [],
                    "displayName": "Nick Fury",
                    "userId": "8c0a1a67-50ce-4114-bb6c-da9c5dbcf6ca",
                    "email": "furyn@teamsgraph.onmicrosoft.com"
                }
            ]
        },
        {
            "id": "19:d74fc2ed-cb0e-4288-a219-b5c71abaf2aa_8c0a1a67-50ce-4114-bb6c-da9c5dbcf6ca@unq.gbl.spaces",
            "topic": null,
            "createdDateTime": "2020-12-04T23:10:28.51Z",
            "lastUpdatedDateTime": "2020-12-04T23:10:36.925Z",
            "chatType": "oneOnOne",
            "members@odata.context": "https://graph.microsoft.com/beta/$metadata#chats('19%3Ad74fc2ed-cb0e-4288-a219-b5c71abaf2aa_8c0a1a67-50ce-4114-bb6c-da9c5dbcf6ca%40unq.gbl.spaces')/members",
            "members": [
                {
                    "@odata.type": "#microsoft.graph.aadUserConversationMember",
                    "id": "MmFiOWM3OTYtMjkwMi00NWY4LWI3MTItN2M1YTYzY2Y0MWM0IyNlZWY5Y2IzNi0wNmRlLTQ2OWItODdjZC03MGY0Y2JlMzJ989kMTQ=",
                    "roles": [],
                    "displayName": "Nick Fury",
                    "userId": "8c0a1a67-50ce-4114-bb6c-da9c5dbcf6ca",
                    "email": "furyn@teamsgraph.onmicrosoft.com"
                },
                {
                    "@odata.type": "#microsoft.graph.aadUserConversationMember",
                    "id": "MmFiOWM3OTYtMjkwMi00NWY4LWI3MTItN2M1YTYzY2Y0MWM0IyNlZWY5Y2IzNi0wNmRlLTQ2OWItODdjZC03MGY0Y2JlMz6Jk45=",
                    "roles": [],
                    "displayName": "Peter Parker",
                    "userId": "d74fc2ed-cb0e-4288-a219-b5c71abaf2aa",
                    "email": "parkerp@teamsgraph.onmicrosoft.com"
                }
            ]
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List chats",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
