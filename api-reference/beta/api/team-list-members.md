---
title: Список участников
description: Получение Конверсатионмемберс команды.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 9adfa391634164af0818bd81b2cc33d9969a79df
ms.sourcegitcommit: 67433748b69541727185fc1f32ed356718bf6ff1
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2020
ms.locfileid: "45051056"
---
# <a name="list-members"></a><span data-ttu-id="7911e-103">Список участников</span><span class="sxs-lookup"><span data-stu-id="7911e-103">List members</span></span>
<span data-ttu-id="7911e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7911e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7911e-105">Получение [конверсатионмембер](../resources/conversationmember.md) [команды](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="7911e-105">Get the [conversationMember](../resources/conversationmember.md) of a [team](../resources/team.md).</span></span>

><span data-ttu-id="7911e-106">Note: в настоящее время этот API не поддерживает разбивку на страницы, поэтому при наличии слишком большого количества участников, которые могут помещаться в один запрос, не будут получены все элементы.</span><span class="sxs-lookup"><span data-stu-id="7911e-106">Note: This API currently does not support pagination, so if there's too many members to fit into one request, you won't get all the members.</span></span>

## <a name="permissions"></a><span data-ttu-id="7911e-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7911e-107">Permissions</span></span>
<span data-ttu-id="7911e-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="7911e-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="7911e-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7911e-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7911e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7911e-110">Permission type</span></span>|<span data-ttu-id="7911e-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7911e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7911e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7911e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7911e-113">Теаммембер. Read. ALL, Теаммембер. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="7911e-113">TeamMember.Read.All, TeamMember.ReadWrite.All</span></span>|
|<span data-ttu-id="7911e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7911e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7911e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7911e-115">Not supported.</span></span>    |
|<span data-ttu-id="7911e-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="7911e-116">Application</span></span>|<span data-ttu-id="7911e-117">Теаммембер. Read. ALL, Теаммембер. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="7911e-117">TeamMember.Read.All, TeamMember.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7911e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7911e-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /teams/{teamsId}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7911e-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7911e-119">Optional query parameters</span></span>
<span data-ttu-id="7911e-120">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="7911e-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="7911e-121">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="7911e-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="7911e-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7911e-122">Request headers</span></span>
|<span data-ttu-id="7911e-123">Имя</span><span class="sxs-lookup"><span data-stu-id="7911e-123">Name</span></span>|<span data-ttu-id="7911e-124">Описание</span><span class="sxs-lookup"><span data-stu-id="7911e-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="7911e-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7911e-125">Authorization</span></span>|<span data-ttu-id="7911e-126">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="7911e-126">Bearer {token}.</span></span> <span data-ttu-id="7911e-127">Required.</span><span class="sxs-lookup"><span data-stu-id="7911e-127">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7911e-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7911e-128">Request body</span></span>
<span data-ttu-id="7911e-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7911e-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7911e-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="7911e-130">Response</span></span>

<span data-ttu-id="7911e-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [конверсатионмембер](../resources/conversationmember.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7911e-131">If successful, this method returns a `200 OK` response code and a collection of [conversationMember](../resources/conversationmember.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7911e-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="7911e-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7911e-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="7911e-133">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_conversationmember"
}
-->
``` http
GET https://graph.microsoft.com/beta/teams/{teamsId}/members
```


### <a name="response"></a><span data-ttu-id="7911e-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="7911e-134">Response</span></span>
<span data-ttu-id="7911e-135">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="7911e-135">**Note:** The response object shown here might be shortened for readability.</span></span>
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
