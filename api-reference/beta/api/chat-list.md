---
title: Список чатов
description: Получение списка бесед для пользователя.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 9f8437aba52cef0d01eda94f4050a37a9cf4c45d
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36418182"
---
# <a name="list-chats"></a><span data-ttu-id="8e7a9-103">Список чатов</span><span class="sxs-lookup"><span data-stu-id="8e7a9-103">List chats</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8e7a9-104">Получение списка [сеансов](../resources/chat.md) , в которые входит пользователь.</span><span class="sxs-lookup"><span data-stu-id="8e7a9-104">Retrieve the list of [chats](../resources/chat.md) that the user is part of.</span></span>

## <a name="permissions"></a><span data-ttu-id="8e7a9-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8e7a9-105">Permissions</span></span>

<span data-ttu-id="8e7a9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e7a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e7a9-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8e7a9-108">Permission type</span></span>      | <span data-ttu-id="8e7a9-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8e7a9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8e7a9-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8e7a9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8e7a9-111">Chat.Read</span><span class="sxs-lookup"><span data-stu-id="8e7a9-111">Chat.Read</span></span>   |
|<span data-ttu-id="8e7a9-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8e7a9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8e7a9-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e7a9-113">Not supported.</span></span>    |
|<span data-ttu-id="8e7a9-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8e7a9-114">Application</span></span> | <span data-ttu-id="8e7a9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e7a9-115">Not supported.</span></span>   |

## <a name="http-request"></a><span data-ttu-id="8e7a9-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8e7a9-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/chats
GET /users/{id}/chats
GET /chats
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8e7a9-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8e7a9-117">Optional query parameters</span></span>

<span data-ttu-id="8e7a9-118">Это действие в настоящее время не поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="8e7a9-118">This operation does not currently support [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8e7a9-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8e7a9-119">Request headers</span></span>

| <span data-ttu-id="8e7a9-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8e7a9-120">Header</span></span>       | <span data-ttu-id="8e7a9-121">Значение</span><span class="sxs-lookup"><span data-stu-id="8e7a9-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8e7a9-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8e7a9-122">Authorization</span></span>  | <span data-ttu-id="8e7a9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8e7a9-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8e7a9-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8e7a9-125">Request body</span></span>

<span data-ttu-id="8e7a9-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8e7a9-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8e7a9-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e7a9-127">Response</span></span>

<span data-ttu-id="8e7a9-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [chat](../resources/chat.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8e7a9-128">If successful, this method returns a `200 OK` response code and a collection of [chat](../resources/chat.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e7a9-129">Пример</span><span class="sxs-lookup"><span data-stu-id="8e7a9-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="8e7a9-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="8e7a9-130">Request</span></span>

<span data-ttu-id="8e7a9-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8e7a9-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8e7a9-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="8e7a9-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chats"
}-->
```http
GET https://graph.microsoft.com/beta/users/{id}/chats
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8e7a9-133">C#</span><span class="sxs-lookup"><span data-stu-id="8e7a9-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chats-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8e7a9-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8e7a9-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chats-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8e7a9-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="8e7a9-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chats-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="8e7a9-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="8e7a9-136">Response</span></span>

<span data-ttu-id="8e7a9-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8e7a9-137">Here is an example of the response.</span></span> 

><span data-ttu-id="8e7a9-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8e7a9-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "suppressions": [
  ]
}
-->
