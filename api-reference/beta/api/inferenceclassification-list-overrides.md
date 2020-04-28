---
title: Список переопределений
description: Получение переопределений сортировки почты, настроенных пользователем для классификации сообщений от определенных отправителей.
localization_priority: Normal
doc_type: apiPageType
author: ''
ms.prod: ''
ms.openlocfilehash: da22fcbc47a57d07b25b4d937fac3a6d266d9e79
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446431"
---
# <a name="list-overrides"></a><span data-ttu-id="e2ad6-103">Список переопределений</span><span class="sxs-lookup"><span data-stu-id="e2ad6-103">List overrides</span></span>

<span data-ttu-id="e2ad6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e2ad6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e2ad6-105">Получение параметров [сортировки папки "Входящие"](../resources/manage-focused-inbox.md) , которые пользователь настроил для того, чтобы всегда классифицировать сообщения от определенных отправителей определенными способами.</span><span class="sxs-lookup"><span data-stu-id="e2ad6-105">Get the [Focused Inbox](../resources/manage-focused-inbox.md) overrides that a user has set up to always classify messages from certain senders in specific ways.</span></span>

<span data-ttu-id="e2ad6-106">Каждое переопределение соответствует SMTP-адресу отправителя.</span><span class="sxs-lookup"><span data-stu-id="e2ad6-106">Each override corresponds to an SMTP address of a sender.</span></span> <span data-ttu-id="e2ad6-107">Изначально у пользователя нет переопределений.</span><span class="sxs-lookup"><span data-stu-id="e2ad6-107">Initially, a user does not have any overrides.</span></span>
## <a name="permissions"></a><span data-ttu-id="e2ad6-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e2ad6-108">Permissions</span></span>
<span data-ttu-id="e2ad6-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e2ad6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2ad6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e2ad6-111">Permission type</span></span>      | <span data-ttu-id="e2ad6-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e2ad6-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e2ad6-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e2ad6-113">Delegated (work or school account)</span></span> | <span data-ttu-id="e2ad6-114">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="e2ad6-114">Mail.Read</span></span>    |
|<span data-ttu-id="e2ad6-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e2ad6-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e2ad6-116">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="e2ad6-116">Mail.Read</span></span>    |
|<span data-ttu-id="e2ad6-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e2ad6-117">Application</span></span> | <span data-ttu-id="e2ad6-118">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="e2ad6-118">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="e2ad6-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e2ad6-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/inferenceClassification/overrides
GET /users/{id}/inferenceClassification/overrides
```

## <a name="request-headers"></a><span data-ttu-id="e2ad6-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e2ad6-120">Request headers</span></span>
| <span data-ttu-id="e2ad6-121">Имя</span><span class="sxs-lookup"><span data-stu-id="e2ad6-121">Name</span></span>       | <span data-ttu-id="e2ad6-122">Тип</span><span class="sxs-lookup"><span data-stu-id="e2ad6-122">Type</span></span> | <span data-ttu-id="e2ad6-123">Описание</span><span class="sxs-lookup"><span data-stu-id="e2ad6-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e2ad6-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="e2ad6-124">Authorization</span></span>  | <span data-ttu-id="e2ad6-125">string</span><span class="sxs-lookup"><span data-stu-id="e2ad6-125">string</span></span>  | <span data-ttu-id="e2ad6-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e2ad6-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e2ad6-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e2ad6-128">Request body</span></span>
<span data-ttu-id="e2ad6-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e2ad6-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e2ad6-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="e2ad6-130">Response</span></span>

<span data-ttu-id="e2ad6-131">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e2ad6-131">If successful, this method returns a `200 OK` response code and a collection of [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e2ad6-132">Пример</span><span class="sxs-lookup"><span data-stu-id="e2ad6-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e2ad6-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="e2ad6-133">Request</span></span>
<span data-ttu-id="e2ad6-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e2ad6-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e2ad6-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="e2ad6-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_overrides"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/inferenceClassification/overrides
```
# <a name="c"></a>[<span data-ttu-id="e2ad6-136">C#</span><span class="sxs-lookup"><span data-stu-id="e2ad6-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-overrides-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e2ad6-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e2ad6-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-overrides-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e2ad6-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e2ad6-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-overrides-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e2ad6-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="e2ad6-139">Response</span></span>
<span data-ttu-id="e2ad6-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e2ad6-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
