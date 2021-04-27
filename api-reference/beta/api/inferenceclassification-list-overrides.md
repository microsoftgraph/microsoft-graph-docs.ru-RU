---
title: Список переопределений
description: Получение переопределений сортировки почты, настроенных пользователем для классификации сообщений от определенных отправителей.
localization_priority: Normal
doc_type: apiPageType
author: abheek-das
ms.prod: ''
ms.openlocfilehash: 07de9e0bb9d8992811b64a8fe19685a2a329a8c1
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52040611"
---
# <a name="list-overrides"></a><span data-ttu-id="063c3-103">Список переопределений</span><span class="sxs-lookup"><span data-stu-id="063c3-103">List overrides</span></span>

<span data-ttu-id="063c3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="063c3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="063c3-105">Получите [переопределения](../resources/manage-focused-inbox.md) сфокусированных почтовых ящиков, которые пользователь настроил, чтобы всегда классифицировать сообщения определенных отправителей определенными способами.</span><span class="sxs-lookup"><span data-stu-id="063c3-105">Get the [Focused Inbox](../resources/manage-focused-inbox.md) overrides that a user has set up to always classify messages from certain senders in specific ways.</span></span>

<span data-ttu-id="063c3-p101">Каждое переопределение соответствует SMTP-адресу отправителя. Изначально у пользователя нет переопределений.</span><span class="sxs-lookup"><span data-stu-id="063c3-p101">Each override corresponds to an SMTP address of a sender. Initially, a user does not have any overrides.</span></span>
## <a name="permissions"></a><span data-ttu-id="063c3-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="063c3-108">Permissions</span></span>
<span data-ttu-id="063c3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="063c3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="063c3-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="063c3-111">Permission type</span></span>      | <span data-ttu-id="063c3-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="063c3-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="063c3-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="063c3-113">Delegated (work or school account)</span></span> | <span data-ttu-id="063c3-114">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="063c3-114">Mail.Read</span></span>    |
|<span data-ttu-id="063c3-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="063c3-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="063c3-116">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="063c3-116">Mail.Read</span></span>    |
|<span data-ttu-id="063c3-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="063c3-117">Application</span></span> | <span data-ttu-id="063c3-118">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="063c3-118">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="063c3-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="063c3-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/inferenceClassification/overrides
GET /users/{id}/inferenceClassification/overrides
```

## <a name="request-headers"></a><span data-ttu-id="063c3-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="063c3-120">Request headers</span></span>
| <span data-ttu-id="063c3-121">Имя</span><span class="sxs-lookup"><span data-stu-id="063c3-121">Name</span></span>       | <span data-ttu-id="063c3-122">Тип</span><span class="sxs-lookup"><span data-stu-id="063c3-122">Type</span></span> | <span data-ttu-id="063c3-123">Описание</span><span class="sxs-lookup"><span data-stu-id="063c3-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="063c3-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="063c3-124">Authorization</span></span>  | <span data-ttu-id="063c3-125">string</span><span class="sxs-lookup"><span data-stu-id="063c3-125">string</span></span>  | <span data-ttu-id="063c3-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="063c3-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="063c3-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="063c3-128">Request body</span></span>
<span data-ttu-id="063c3-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="063c3-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="063c3-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="063c3-130">Response</span></span>

<span data-ttu-id="063c3-131">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="063c3-131">If successful, this method returns a `200 OK` response code and a collection of [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="063c3-132">Пример</span><span class="sxs-lookup"><span data-stu-id="063c3-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="063c3-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="063c3-133">Request</span></span>
<span data-ttu-id="063c3-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="063c3-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="063c3-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="063c3-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_overrides"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/inferenceClassification/overrides
```
# <a name="c"></a>[<span data-ttu-id="063c3-136">C#</span><span class="sxs-lookup"><span data-stu-id="063c3-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-overrides-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="063c3-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="063c3-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-overrides-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="063c3-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="063c3-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-overrides-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="063c3-139">Java</span><span class="sxs-lookup"><span data-stu-id="063c3-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-overrides-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="063c3-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="063c3-140">Response</span></span>
<span data-ttu-id="063c3-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="063c3-141">Here is an example of the response.</span></span> <span data-ttu-id="063c3-142">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="063c3-142">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.inferenceClassificationOverride",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "classifyAs": "focused",
      "senderEmailAddress": {
        "name": "Samantha Booth",
        "address": "samanthab@adatum.onmicrosoft.com"
      },
      "id": "98f5bdef-576a-404d-a2ea-07a3cf11a9b9"
    },
    {
      "classifyAs": "other",
      "senderEmailAddress": {
        "name": "Randi Welch",
        "address": "randiw@adatum.onmicrosoft.com"
      },
      "id": "98f5bdef-576a-404d-a2ea-07a3cf34af4r"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List overrides",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


