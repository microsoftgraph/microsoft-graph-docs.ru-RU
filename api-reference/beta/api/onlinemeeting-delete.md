---
title: Удаление Онлинемитинг
description: Удаление собрания по сети.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: d6b5f0afa09bf88c9f070ef88adda2f5be20c50f
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871913"
---
# <a name="delete-onlinemeeting"></a><span data-ttu-id="d1495-103">Удаление Онлинемитинг</span><span class="sxs-lookup"><span data-stu-id="d1495-103">Delete onlineMeeting</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d1495-104">Удаление объекта [онлинемитинг](../resources/onlinemeeting.md) .</span><span class="sxs-lookup"><span data-stu-id="d1495-104">Delete an [onlineMeeting](../resources/onlinemeeting.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d1495-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="d1495-105">Permissions</span></span>

| <span data-ttu-id="d1495-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d1495-106">Permission type</span></span> | <span data-ttu-id="d1495-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d1495-107">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="d1495-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d1495-108">Delegated (work or school account)</span></span>     | <span data-ttu-id="d1495-109">OnlineMeetings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d1495-109">OnlineMeetings.ReadWrite</span></span>              |
| <span data-ttu-id="d1495-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d1495-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d1495-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d1495-111">Not Supported.</span></span>                         |
| <span data-ttu-id="d1495-112">Приложение</span><span class="sxs-lookup"><span data-stu-id="d1495-112">Application</span></span>                            | <span data-ttu-id="d1495-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d1495-113">Not Supported.</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="d1495-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d1495-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE https://graph.microsoft.com/beta/me/onlineMeetings/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d1495-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d1495-115">Request headers</span></span>
| <span data-ttu-id="d1495-116">Имя</span><span class="sxs-lookup"><span data-stu-id="d1495-116">Name</span></span>          | <span data-ttu-id="d1495-117">Описание</span><span class="sxs-lookup"><span data-stu-id="d1495-117">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="d1495-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d1495-118">Authorization</span></span> | <span data-ttu-id="d1495-p101">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d1495-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d1495-121">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d1495-121">Request body</span></span>
<span data-ttu-id="d1495-122">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d1495-122">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d1495-123">Ответ</span><span class="sxs-lookup"><span data-stu-id="d1495-123">Response</span></span>
<span data-ttu-id="d1495-p102">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d1495-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d1495-126">Примеры</span><span class="sxs-lookup"><span data-stu-id="d1495-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d1495-127">Запрос</span><span class="sxs-lookup"><span data-stu-id="d1495-127">Request</span></span>
<span data-ttu-id="d1495-128">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d1495-128">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="d1495-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="d1495-129">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete-call"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/onlineMeetings/550fae72-d251-43ec-868c-373732c2704f_19:meeting_M2IzYzczNTItYmY3OC00MDlmLWJjMzUtYmFiMjNlOTY4MGEz@thread.skype
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d1495-130">C#</span><span class="sxs-lookup"><span data-stu-id="d1495-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-call-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d1495-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d1495-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-call-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d1495-132">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d1495-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-call-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d1495-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="d1495-133">Response</span></span>

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
