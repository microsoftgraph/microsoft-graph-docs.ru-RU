---
title: Удаление Онлинемитинг
description: Удаление собрания по сети.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: a85e1d77022e1f890eb0bba70fac8557918f8b8f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42511280"
---
# <a name="delete-onlinemeeting"></a><span data-ttu-id="48ee8-103">Удаление Онлинемитинг</span><span class="sxs-lookup"><span data-stu-id="48ee8-103">Delete onlineMeeting</span></span>

<span data-ttu-id="48ee8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="48ee8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="48ee8-105">Удаление объекта [онлинемитинг](../resources/onlinemeeting.md) .</span><span class="sxs-lookup"><span data-stu-id="48ee8-105">Delete an [onlineMeeting](../resources/onlinemeeting.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="48ee8-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="48ee8-106">Permissions</span></span>

| <span data-ttu-id="48ee8-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="48ee8-107">Permission type</span></span> | <span data-ttu-id="48ee8-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="48ee8-108">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="48ee8-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="48ee8-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="48ee8-110">OnlineMeetings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="48ee8-110">OnlineMeetings.ReadWrite</span></span>              |
| <span data-ttu-id="48ee8-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="48ee8-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="48ee8-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48ee8-112">Not Supported.</span></span>                         |
| <span data-ttu-id="48ee8-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="48ee8-113">Application</span></span>                            | <span data-ttu-id="48ee8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48ee8-114">Not Supported.</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="48ee8-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="48ee8-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE https://graph.microsoft.com/v1.0/me/onlineMeetings/{id}
```

## <a name="request-headers"></a><span data-ttu-id="48ee8-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="48ee8-116">Request headers</span></span>
| <span data-ttu-id="48ee8-117">Имя</span><span class="sxs-lookup"><span data-stu-id="48ee8-117">Name</span></span>          | <span data-ttu-id="48ee8-118">Описание</span><span class="sxs-lookup"><span data-stu-id="48ee8-118">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="48ee8-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="48ee8-119">Authorization</span></span> | <span data-ttu-id="48ee8-p101">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="48ee8-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="48ee8-122">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="48ee8-122">Request body</span></span>
<span data-ttu-id="48ee8-123">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="48ee8-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="48ee8-124">Ответ</span><span class="sxs-lookup"><span data-stu-id="48ee8-124">Response</span></span>
<span data-ttu-id="48ee8-p102">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="48ee8-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="48ee8-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="48ee8-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="48ee8-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="48ee8-128">Request</span></span>
<span data-ttu-id="48ee8-129">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="48ee8-129">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="48ee8-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="48ee8-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete-call"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/onlineMeetings/550fae72-d251-43ec-868c-373732c2704f_19:meeting_M2IzYzczNTItYmY3OC00MDlmLWJjMzUtYmFiMjNlOTY4MGEz@thread.skype
```
# <a name="c"></a>[<span data-ttu-id="48ee8-131">C#</span><span class="sxs-lookup"><span data-stu-id="48ee8-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-call-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="48ee8-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="48ee8-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-call-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="48ee8-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="48ee8-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-call-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="48ee8-134">Java</span><span class="sxs-lookup"><span data-stu-id="48ee8-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-call-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="48ee8-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="48ee8-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete call",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
