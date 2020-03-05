---
title: Получение чата
description: Получение одного объекта chat.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 4e0e9126564074d34fd88d48751440dede270d8b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42438654"
---
# <a name="get-chat"></a><span data-ttu-id="8fba6-103">Получение чата</span><span class="sxs-lookup"><span data-stu-id="8fba6-103">Get chat</span></span>

<span data-ttu-id="8fba6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8fba6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8fba6-105">Получение одного объекта [chat](../resources/chat.md) (без его сообщений).</span><span class="sxs-lookup"><span data-stu-id="8fba6-105">Retrieve a single [chat](../resources/chat.md) (without its messages).</span></span>

## <a name="permissions"></a><span data-ttu-id="8fba6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8fba6-106">Permissions</span></span>

<span data-ttu-id="8fba6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8fba6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="8fba6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8fba6-109">Permission type</span></span>      | <span data-ttu-id="8fba6-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8fba6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8fba6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8fba6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8fba6-112">Chat.Read</span><span class="sxs-lookup"><span data-stu-id="8fba6-112">Chat.Read</span></span>   |
|<span data-ttu-id="8fba6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8fba6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8fba6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8fba6-114">Not supported.</span></span>    |
|<span data-ttu-id="8fba6-115">Для приложения</span><span class="sxs-lookup"><span data-stu-id="8fba6-115">Application</span></span> | <span data-ttu-id="8fba6-116">Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8fba6-116">Chat.Read.All, Chat.ReadWrite.All</span></span>   |

> [!NOTE]
> <span data-ttu-id="8fba6-117">С разрешениями приложений поддерживается получение отдельного чата, но не поддерживается [получение списка чатов](chat-list.md).</span><span class="sxs-lookup"><span data-stu-id="8fba6-117">With application permissions, getting a single chat is supported, but [getting a list of chats](chat-list.md) is not.</span></span>

> [!NOTE]
> <span data-ttu-id="8fba6-118">Перед вызовом этого API с разрешениями приложения необходимо запросить доступ.</span><span class="sxs-lookup"><span data-stu-id="8fba6-118">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="8fba6-119">Дополнительные сведения см. в статье [Защищенные APIs в Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="8fba6-119">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="8fba6-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8fba6-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/chats/{id}
GET /users/{id}/chats/{id}
GET /chats/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8fba6-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8fba6-121">Optional query parameters</span></span>

<span data-ttu-id="8fba6-122">Это действие в настоящее время не поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="8fba6-122">This operation does not currently support [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8fba6-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8fba6-123">Request headers</span></span>

| <span data-ttu-id="8fba6-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8fba6-124">Header</span></span>       | <span data-ttu-id="8fba6-125">Значение</span><span class="sxs-lookup"><span data-stu-id="8fba6-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8fba6-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8fba6-126">Authorization</span></span>  | <span data-ttu-id="8fba6-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8fba6-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8fba6-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8fba6-129">Request body</span></span>

<span data-ttu-id="8fba6-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8fba6-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8fba6-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="8fba6-131">Response</span></span>

<span data-ttu-id="8fba6-132">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [chat](../resources/chat.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8fba6-132">If successful, this method returns a `200 OK` response code and a collection of [chat](../resources/chat.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8fba6-133">Пример</span><span class="sxs-lookup"><span data-stu-id="8fba6-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8fba6-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="8fba6-134">Request</span></span>
<span data-ttu-id="8fba6-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8fba6-135">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8fba6-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="8fba6-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chat_message"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/chats/{id}
```
# <a name="c"></a>[<span data-ttu-id="8fba6-137">C#</span><span class="sxs-lookup"><span data-stu-id="8fba6-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chat-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8fba6-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8fba6-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chat-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8fba6-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8fba6-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chat-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="8fba6-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="8fba6-140">Response</span></span>
<span data-ttu-id="8fba6-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8fba6-141">Here is an example of the response.</span></span> 

><span data-ttu-id="8fba6-142">**Примечание.** Объект отклика, показанный здесь, сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="8fba6-142">**Note:** The response object shown here is shortened for readability.</span></span> <span data-ttu-id="8fba6-143">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8fba6-143">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#chats/$entity",
    "id": "19:8b081ef6-4792-4def-b2c9-c363a1bf41d5_877192bd-9183-47d3-a74c-8aa0426716cf@unq.gbl.spaces",
    "topic": null,
    "createdDateTime": "2019-04-18T23:51:42.099Z",
    "lastUpdatedDateTime": "2019-04-18T23:51:43.255Z"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get chat",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
