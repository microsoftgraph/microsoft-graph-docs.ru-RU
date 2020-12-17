---
title: Получение чата
description: Получение одного объекта chat.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 9ad608215fe237c94dd2092a1796ac652e7b95c0
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/17/2020
ms.locfileid: "49705900"
---
# <a name="get-chat"></a><span data-ttu-id="51fda-103">Получение чата</span><span class="sxs-lookup"><span data-stu-id="51fda-103">Get chat</span></span>

<span data-ttu-id="51fda-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="51fda-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="51fda-105">Получение одного объекта [chat](../resources/chat.md) (без его сообщений).</span><span class="sxs-lookup"><span data-stu-id="51fda-105">Retrieve a single [chat](../resources/chat.md) (without its messages).</span></span>

## <a name="permissions"></a><span data-ttu-id="51fda-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="51fda-106">Permissions</span></span>

<span data-ttu-id="51fda-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51fda-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="51fda-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="51fda-109">Permission type</span></span>      | <span data-ttu-id="51fda-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="51fda-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="51fda-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="51fda-111">Delegated (work or school account)</span></span> | <span data-ttu-id="51fda-112">Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="51fda-112">Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span></span> |
|<span data-ttu-id="51fda-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="51fda-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="51fda-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51fda-114">Not supported.</span></span>    |
|<span data-ttu-id="51fda-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="51fda-115">Application</span></span> | <span data-ttu-id="51fda-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51fda-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="51fda-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="51fda-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/chats/{chat-id}
GET /users/{user-id}/chats/{chat-id}
GET /chats/{chat-id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="51fda-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="51fda-118">Optional query parameters</span></span>

<span data-ttu-id="51fda-119">Это действие в настоящее время не поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="51fda-119">This operation does not currently support [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="51fda-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="51fda-120">Request headers</span></span>

| <span data-ttu-id="51fda-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="51fda-121">Header</span></span>       | <span data-ttu-id="51fda-122">Значение</span><span class="sxs-lookup"><span data-stu-id="51fda-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="51fda-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="51fda-123">Authorization</span></span>  | <span data-ttu-id="51fda-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="51fda-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="51fda-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="51fda-126">Request body</span></span>

<span data-ttu-id="51fda-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="51fda-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="51fda-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="51fda-128">Response</span></span>

<span data-ttu-id="51fda-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [chat](../resources/chat.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="51fda-129">If successful, this method returns a `200 OK` response code and a collection of [chat](../resources/chat.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51fda-130">Пример</span><span class="sxs-lookup"><span data-stu-id="51fda-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="51fda-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="51fda-131">Request</span></span>
<span data-ttu-id="51fda-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="51fda-132">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="51fda-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="51fda-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chat"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5/chats/19:8b081ef6-4792-4def-b2c9-c363a1bf41d5_877192bd-9183-47d3-a74c-8aa0426716cf@unq.gbl.spaces
```

---

##### <a name="response"></a><span data-ttu-id="51fda-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="51fda-134">Response</span></span>
<span data-ttu-id="51fda-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="51fda-135">Here is an example of the response.</span></span> 

><span data-ttu-id="51fda-136">**Примечание.** Объект отклика, показанный здесь, сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="51fda-136">**Note:** The response object shown here is shortened for readability.</span></span> <span data-ttu-id="51fda-137">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="51fda-137">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chat"
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
    "lastUpdatedDateTime": "2019-04-18T23:51:43.255Z",
    "chatType": "oneOnOne"
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


