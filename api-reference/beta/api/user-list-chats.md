---
title: Список чатов
description: Получение списка объектов Chat.
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: a70eaaabfce231dc05d2b226414ab1767d4c48e2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016977"
---
# <a name="list-chats"></a><span data-ttu-id="188a0-103">Список чатов</span><span class="sxs-lookup"><span data-stu-id="188a0-103">List chats</span></span>

<span data-ttu-id="188a0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="188a0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="188a0-105">Получение списка объектов Chat.</span><span class="sxs-lookup"><span data-stu-id="188a0-105">Retrieve a list of chat objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="188a0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="188a0-106">Permissions</span></span>

<span data-ttu-id="188a0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="188a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="188a0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="188a0-109">Permission type</span></span>                        | <span data-ttu-id="188a0-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="188a0-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="188a0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="188a0-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="188a0-112">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="188a0-112">Chat.Read, Chat.ReadWrite</span></span> |
| <span data-ttu-id="188a0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="188a0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="188a0-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="188a0-114">Not supported.</span></span> |
| <span data-ttu-id="188a0-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="188a0-115">Application</span></span>                            | <span data-ttu-id="188a0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="188a0-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="188a0-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="188a0-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /users/{id}/chats
```

## <a name="optional-query-parameters"></a><span data-ttu-id="188a0-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="188a0-118">Optional query parameters</span></span>

<span data-ttu-id="188a0-119">Эта операция не поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="188a0-119">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="188a0-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="188a0-120">Request headers</span></span>

| <span data-ttu-id="188a0-121">Имя</span><span class="sxs-lookup"><span data-stu-id="188a0-121">Name</span></span>      |<span data-ttu-id="188a0-122">Описание</span><span class="sxs-lookup"><span data-stu-id="188a0-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="188a0-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="188a0-123">Authorization</span></span> | <span data-ttu-id="188a0-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="188a0-124">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="188a0-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="188a0-125">Request body</span></span>

<span data-ttu-id="188a0-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="188a0-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="188a0-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="188a0-127">Response</span></span>

<span data-ttu-id="188a0-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [chat](../resources/chat.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="188a0-128">If successful, this method returns a `200 OK` response code and a collection of [chat](../resources/chat.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="188a0-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="188a0-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="188a0-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="188a0-130">Request</span></span>

<span data-ttu-id="188a0-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="188a0-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="188a0-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="188a0-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chats"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/chats
```
# <a name="c"></a>[<span data-ttu-id="188a0-133">C#</span><span class="sxs-lookup"><span data-stu-id="188a0-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chats-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="188a0-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="188a0-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chats-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="188a0-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="188a0-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chats-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="188a0-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="188a0-136">Response</span></span>

<span data-ttu-id="188a0-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="188a0-137">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="188a0-138">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="188a0-138">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="188a0-139">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="188a0-139">All the properties will be returned from an actual call.</span></span>

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
  "value": [
    {
      "id": "id-value",
      "topic": "topic-value",
      "createdDateTime": "datetime-value",
      "lastUpdatedDateTime": "datetime-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List chats",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


