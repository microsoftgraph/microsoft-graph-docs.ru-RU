---
title: Список чатов
description: Получение списка бесед для пользователя.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 818cd5037c9d37d58e96b40c85e546487676a13e
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33327712"
---
# <a name="list-chats"></a><span data-ttu-id="51b64-103">Список чатов</span><span class="sxs-lookup"><span data-stu-id="51b64-103">List chats</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="51b64-104">Получение списка [сеансов](../resources/chat.md) , в которые входит пользователь.</span><span class="sxs-lookup"><span data-stu-id="51b64-104">Retrieve the list of [chats](../resources/chat.md) that the user is part of.</span></span>

## <a name="permissions"></a><span data-ttu-id="51b64-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="51b64-105">Permissions</span></span>

<span data-ttu-id="51b64-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51b64-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51b64-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="51b64-108">Permission type</span></span>      | <span data-ttu-id="51b64-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="51b64-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="51b64-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="51b64-110">Delegated (work or school account)</span></span> | <span data-ttu-id="51b64-111">Чат. Read</span><span class="sxs-lookup"><span data-stu-id="51b64-111">Chat.Read</span></span>   |
|<span data-ttu-id="51b64-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="51b64-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="51b64-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51b64-113">Not supported.</span></span>    |
|<span data-ttu-id="51b64-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="51b64-114">Application</span></span> | <span data-ttu-id="51b64-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51b64-115">Not supported.</span></span>   |

## <a name="http-request"></a><span data-ttu-id="51b64-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="51b64-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/chats
GET /users/{id}/chats
GET /chats
```

## <a name="optional-query-parameters"></a><span data-ttu-id="51b64-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="51b64-117">Optional query parameters</span></span>

<span data-ttu-id="51b64-118">Эта операция в настоящее время не поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="51b64-118">This operation does not currently support [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="51b64-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="51b64-119">Request headers</span></span>

| <span data-ttu-id="51b64-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="51b64-120">Header</span></span>       | <span data-ttu-id="51b64-121">Значение</span><span class="sxs-lookup"><span data-stu-id="51b64-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="51b64-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="51b64-122">Authorization</span></span>  | <span data-ttu-id="51b64-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="51b64-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="51b64-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="51b64-125">Request body</span></span>

<span data-ttu-id="51b64-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="51b64-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="51b64-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="51b64-127">Response</span></span>

<span data-ttu-id="51b64-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [Chat](../resources/chat.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="51b64-128">If successful, this method returns a `200 OK` response code and a collection of [chat](../resources/chat.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51b64-129">Пример</span><span class="sxs-lookup"><span data-stu-id="51b64-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="51b64-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="51b64-130">Request</span></span>

<span data-ttu-id="51b64-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="51b64-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_chats"
}-->
```http
GET https://graph.microsoft.com/beta/users/{id}/chats
```

##### <a name="response"></a><span data-ttu-id="51b64-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="51b64-132">Response</span></span>

<span data-ttu-id="51b64-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="51b64-133">Here is an example of the response.</span></span> 

><span data-ttu-id="51b64-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="51b64-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chat",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 262

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#chats",
    "value": [
        {
            "id": "19:8b081ef6-4792-4def-b2c9-c363a1bf41d5_877192bd-9183-47d3-a74c-8aa0426716cf@unq.gbl.spaces",
            "topic": null,
            "createdDateTime": "2019-04-18T23:51:42.099Z",
            "lastUpdatedDateTime": "2019-04-18T23:51:43.255Z"
        },
        {
            "id": "19:8b081ef6-4792-4def-b2c9-c363a1bf41d5_0c5cfdbb-596f-4d39-b557-5d9516c94107@unq.gbl.spaces",
            "topic": null,
            "createdDateTime": "2019-04-18T23:19:23.76Z",
            "lastUpdatedDateTime": "2019-04-18T23:19:21.994Z"
        },
        {
            "id": "19:8b081ef6-4792-4def-b2c9-c363a1bf41d5_3ee373aa-62fa-4fc6-b11f-9627d5b4a73d@unq.gbl.spaces",
            "topic": null,
            "createdDateTime": "2019-03-21T22:30:14.867Z",
            "lastUpdatedDateTime": "2019-03-21T22:30:15.507Z"
        },
        {
            "id": "19:8b081ef6-4792-4def-b2c9-c363a1bf41d5_90a27c51-5c74-453b-944a-134ba86da790@unq.gbl.spaces",
            "topic": null,
            "createdDateTime": "2019-02-06T03:38:58.062Z",
            "lastUpdatedDateTime": "2019-02-06T03:38:58.063Z"
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
  "suppressions": []
}
-->
