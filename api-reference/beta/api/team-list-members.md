---
title: Список участников группы
description: Получение conversationMembers группы.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 4685e277f386d6ecaa51565778529ac812ba1c65
ms.sourcegitcommit: 2d665f916371aa9515e4c542aa67094abff2fa1a
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/24/2020
ms.locfileid: "49387593"
---
# <a name="list-members-of-team"></a><span data-ttu-id="30b04-103">Список участников группы</span><span class="sxs-lookup"><span data-stu-id="30b04-103">List members of team</span></span>
<span data-ttu-id="30b04-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="30b04-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="30b04-105">Получение набора данных [conversationMember](../resources/conversationmember.md) [группы](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="30b04-105">Get the [conversationMember](../resources/conversationmember.md) collection of a [team](../resources/team.md).</span></span>

> [!NOTE]
> <span data-ttu-id="30b04-106">Идентификаторы членства, возвращаемые сервером, должны рассматриваться как непрозрачные строки.</span><span class="sxs-lookup"><span data-stu-id="30b04-106">The membership IDs returned by the server must be treated as opaque strings.</span></span> <span data-ttu-id="30b04-107">Клиент не должен пытаться анализировать или делать какие-либо предположения об этих идентификаторах ресурсов.</span><span class="sxs-lookup"><span data-stu-id="30b04-107">The client should not try to parse or make any assumptions about these resource IDs.</span></span>
>
> <span data-ttu-id="30b04-108">В дальнейшем результаты членства могут сопоставляться с пользователями различных клиентов, как указано в отклике.</span><span class="sxs-lookup"><span data-stu-id="30b04-108">The membership results could map to users from different tenants, as indicated in the response, in the future.</span></span> <span data-ttu-id="30b04-109">Клиент не должен предполагать, что все участники относятся только к текущему клиенту.</span><span class="sxs-lookup"><span data-stu-id="30b04-109">The client should not assume that all members are from the current tenant only.</span></span>

## <a name="permissions"></a><span data-ttu-id="30b04-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="30b04-110">Permissions</span></span>
<span data-ttu-id="30b04-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="30b04-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30b04-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="30b04-113">Permission type</span></span>|<span data-ttu-id="30b04-114">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="30b04-114">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="30b04-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="30b04-115">Delegated (work or school account)</span></span>| <span data-ttu-id="30b04-116">TeamMember.Read.All, TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30b04-116">TeamMember.Read.All, TeamMember.ReadWrite.All</span></span> |
|<span data-ttu-id="30b04-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="30b04-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="30b04-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30b04-118">Not supported.</span></span>    |
|<span data-ttu-id="30b04-119">Приложение</span><span class="sxs-lookup"><span data-stu-id="30b04-119">Application</span></span>| <span data-ttu-id="30b04-120">TeamMember.Read.Group\*, TeamMember.Read.All, TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30b04-120">TeamMember.Read.Group\*, TeamMember.Read.All, TeamMember.ReadWrite.All</span></span> |

> <span data-ttu-id="30b04-121">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="30b04-121">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

## <a name="http-request"></a><span data-ttu-id="30b04-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="30b04-122">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /teams/{team-id}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="30b04-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="30b04-123">Optional query parameters</span></span>
<span data-ttu-id="30b04-124">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="30b04-124">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="30b04-125">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="30b04-125">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="30b04-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="30b04-126">Request headers</span></span>
|<span data-ttu-id="30b04-127">Имя</span><span class="sxs-lookup"><span data-stu-id="30b04-127">Name</span></span>|<span data-ttu-id="30b04-128">Описание</span><span class="sxs-lookup"><span data-stu-id="30b04-128">Description</span></span>|
|:---|:---|
|<span data-ttu-id="30b04-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="30b04-129">Authorization</span></span>|<span data-ttu-id="30b04-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="30b04-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="30b04-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="30b04-132">Request body</span></span>
<span data-ttu-id="30b04-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="30b04-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="30b04-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="30b04-134">Response</span></span>

<span data-ttu-id="30b04-135">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [conversationMember](../resources/conversationmember.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="30b04-135">If successful, this method returns a `200 OK` response code and a collection of [conversationMember](../resources/conversationmember.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="30b04-136">Примеры</span><span class="sxs-lookup"><span data-stu-id="30b04-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="30b04-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="30b04-137">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="30b04-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="30b04-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_conversationmember"
}
-->
``` http
GET https://graph.microsoft.com/beta/teams/ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062/members
```
# <a name="c"></a>[<span data-ttu-id="30b04-139">C#</span><span class="sxs-lookup"><span data-stu-id="30b04-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-conversationmember-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="30b04-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="30b04-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-conversationmember-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="30b04-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="30b04-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-conversationmember-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="30b04-142">Java</span><span class="sxs-lookup"><span data-stu-id="30b04-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-conversationmember-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="30b04-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="30b04-143">Response</span></span>
<span data-ttu-id="30b04-144">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="30b04-144">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "name": "get_conversationmember",
  "@odata.type": "collection(microsoft.graph.aadUserConversationMember)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062')/members",
    "@odata.count": 2,
    "value": [
        {
            "@odata.type": "#microsoft.graph.aadUserConversationMember",
            "id": "ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=",
            "roles": [],
            "displayName": "Adele Vance",
            "userId": "73761f06-2ac9-469c-9f10-279a8cc267f9",
            "email": "AdeleV@M365x987948.OnMicrosoft.com"
        },
        {
            "@odata.type": "#microsoft.graph.aadUserConversationMember",
            "id": "ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM1OThlZmNkNC1lNTQ5LTQwMmEtOTYwMi0wYjUwMjAxZmFlYmU=",
            "roles": [
                "owner"
            ],
            "displayName": "MOD Administrator",
            "userId": "598efcd4-e549-402a-9602-0b50201faebe",
            "email": "admin@M365x987948.OnMicrosoft.com"
        }
    ]
}
```

## <a name="see-also"></a><span data-ttu-id="30b04-145">См. также</span><span class="sxs-lookup"><span data-stu-id="30b04-145">See also</span></span>

- [<span data-ttu-id="30b04-146">Список участников в канале</span><span class="sxs-lookup"><span data-stu-id="30b04-146">List members in channel</span></span>](channel-list-members.md)
