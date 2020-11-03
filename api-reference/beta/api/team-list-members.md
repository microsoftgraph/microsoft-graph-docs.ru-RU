---
title: Список участников
description: Получение conversationMembers группы.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 151274972a58707a8af7410eed5027261c4e6326
ms.sourcegitcommit: d1e72c8d36aad78732133f9ecefaf66c433b8530
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2020
ms.locfileid: "48848849"
---
# <a name="list-members"></a><span data-ttu-id="49e55-103">Список участников</span><span class="sxs-lookup"><span data-stu-id="49e55-103">List members</span></span>
<span data-ttu-id="49e55-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49e55-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="49e55-105">Получение [conversationMember](../resources/conversationmember.md) [группы](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="49e55-105">Get the [conversationMember](../resources/conversationmember.md) of a [team](../resources/team.md).</span></span>

><span data-ttu-id="49e55-106">Примечание. в настоящее время данный API не поддерживает разбивку на страницы, поэтому если в одном запросе помещено слишком много участников, вы не сможете получить доступ ко всем участникам.</span><span class="sxs-lookup"><span data-stu-id="49e55-106">Note: This API currently does not support pagination, so if there's too many members to fit into one request, you won't get all the members.</span></span>

## <a name="permissions"></a><span data-ttu-id="49e55-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="49e55-107">Permissions</span></span>
<span data-ttu-id="49e55-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49e55-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49e55-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="49e55-110">Permission type</span></span>|<span data-ttu-id="49e55-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="49e55-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="49e55-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="49e55-112">Delegated (work or school account)</span></span>| <span data-ttu-id="49e55-113">TeamMember.Read.All, TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49e55-113">TeamMember.Read.All, TeamMember.ReadWrite.All</span></span> |
|<span data-ttu-id="49e55-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="49e55-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="49e55-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49e55-115">Not supported.</span></span>    |
|<span data-ttu-id="49e55-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="49e55-116">Application</span></span>| <span data-ttu-id="49e55-117">TeamMember.Read.Group\*, TeamMember.Read.All, TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49e55-117">TeamMember.Read.Group\*, TeamMember.Read.All, TeamMember.ReadWrite.All</span></span> |

> <span data-ttu-id="49e55-118">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="49e55-118">**Note** : Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

## <a name="http-request"></a><span data-ttu-id="49e55-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="49e55-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /teams/{teamsId}/members
GET /teams/{teamsId}/channels/{channelId}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="49e55-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="49e55-120">Optional query parameters</span></span>
<span data-ttu-id="49e55-121">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="49e55-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="49e55-122">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="49e55-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="49e55-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="49e55-123">Request headers</span></span>
|<span data-ttu-id="49e55-124">Имя</span><span class="sxs-lookup"><span data-stu-id="49e55-124">Name</span></span>|<span data-ttu-id="49e55-125">Описание</span><span class="sxs-lookup"><span data-stu-id="49e55-125">Description</span></span>|
|:---|:---|
|<span data-ttu-id="49e55-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="49e55-126">Authorization</span></span>|<span data-ttu-id="49e55-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="49e55-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="49e55-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="49e55-129">Request body</span></span>
<span data-ttu-id="49e55-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="49e55-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="49e55-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="49e55-131">Response</span></span>

<span data-ttu-id="49e55-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [conversationMember](../resources/conversationmember.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="49e55-132">If successful, this method returns a `200 OK` response code and a collection of [conversationMember](../resources/conversationmember.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="49e55-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="49e55-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="49e55-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="49e55-134">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="49e55-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="49e55-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_conversationmember"
}
-->
``` http
GET https://graph.microsoft.com/beta/teams/{teamsId}/members
```
# <a name="c"></a>[<span data-ttu-id="49e55-136">C#</span><span class="sxs-lookup"><span data-stu-id="49e55-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-conversationmember-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="49e55-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="49e55-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-conversationmember-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="49e55-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="49e55-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-conversationmember-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="49e55-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="49e55-139">Response</span></span>
<span data-ttu-id="49e55-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="49e55-140">**Note:** The response object shown here might be shortened for readability.</span></span>
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


