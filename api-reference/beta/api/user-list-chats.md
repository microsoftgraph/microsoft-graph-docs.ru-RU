---
title: Список чатов
description: Получение списка объектов Chat.
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 55754e66306a021526b5dda0b071accb9992a472
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35867476"
---
# <a name="list-chats"></a><span data-ttu-id="428d0-103">Список чатов</span><span class="sxs-lookup"><span data-stu-id="428d0-103">List chats</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="428d0-104">Получение списка объектов Chat.</span><span class="sxs-lookup"><span data-stu-id="428d0-104">Retrieve a list of chat objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="428d0-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="428d0-105">Permissions</span></span>

<span data-ttu-id="428d0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="428d0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="428d0-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="428d0-108">Permission type</span></span>                        | <span data-ttu-id="428d0-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="428d0-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="428d0-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="428d0-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="428d0-111">Чат. Read, Chat. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="428d0-111">Chat.Read, Chat.ReadWrite</span></span> |
| <span data-ttu-id="428d0-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="428d0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="428d0-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="428d0-113">Not supported.</span></span> |
| <span data-ttu-id="428d0-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="428d0-114">Application</span></span>                            | <span data-ttu-id="428d0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="428d0-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="428d0-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="428d0-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /users/{id}/chats
```

## <a name="optional-query-parameters"></a><span data-ttu-id="428d0-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="428d0-117">Optional query parameters</span></span>

<span data-ttu-id="428d0-118">Эта операция не поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="428d0-118">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="428d0-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="428d0-119">Request headers</span></span>

| <span data-ttu-id="428d0-120">Имя</span><span class="sxs-lookup"><span data-stu-id="428d0-120">Name</span></span>      |<span data-ttu-id="428d0-121">Описание</span><span class="sxs-lookup"><span data-stu-id="428d0-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="428d0-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="428d0-122">Authorization</span></span> | <span data-ttu-id="428d0-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="428d0-123">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="428d0-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="428d0-124">Request body</span></span>

<span data-ttu-id="428d0-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="428d0-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="428d0-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="428d0-126">Response</span></span>

<span data-ttu-id="428d0-127">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [chat](../resources/chat.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="428d0-127">If successful, this method returns a `200 OK` response code and a collection of [chat](../resources/chat.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="428d0-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="428d0-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="428d0-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="428d0-129">Request</span></span>

<span data-ttu-id="428d0-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="428d0-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="428d0-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="428d0-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chats"
}-->

```http
GET https://graph.microsoft.com/beta/users/{id}/chats
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="428d0-132">C#</span><span class="sxs-lookup"><span data-stu-id="428d0-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chats-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="428d0-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="428d0-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chats-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="428d0-134">Цель — C</span><span class="sxs-lookup"><span data-stu-id="428d0-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chats-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="428d0-135">Java</span><span class="sxs-lookup"><span data-stu-id="428d0-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-chats-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="428d0-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="428d0-136">Response</span></span>

<span data-ttu-id="428d0-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="428d0-137">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="428d0-138">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="428d0-138">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="428d0-139">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="428d0-139">All the properties will be returned from an actual call.</span></span>

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
