---
title: Список переопределений
description: Получение переопределений сортировки почты, настроенных пользователем для классификации сообщений от определенных отправителей.
localization_priority: Normal
doc_type: apiPageType
author: svpsiva
ms.prod: ''
ms.openlocfilehash: b0880959138f9d7b914c490f45fd43b8a7ad866c
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48953117"
---
# <a name="list-overrides"></a><span data-ttu-id="07dc1-103">Список переопределений</span><span class="sxs-lookup"><span data-stu-id="07dc1-103">List overrides</span></span>

<span data-ttu-id="07dc1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="07dc1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="07dc1-105">Получение параметров [сортировки папки "Входящие"](../resources/manage-focused-inbox.md) , которые пользователь настроил для того, чтобы всегда классифицировать сообщения от определенных отправителей определенными способами.</span><span class="sxs-lookup"><span data-stu-id="07dc1-105">Get the [Focused Inbox](../resources/manage-focused-inbox.md) overrides that a user has set up to always classify messages from certain senders in specific ways.</span></span>

<span data-ttu-id="07dc1-106">Каждое переопределение соответствует SMTP-адресу отправителя.</span><span class="sxs-lookup"><span data-stu-id="07dc1-106">Each override corresponds to an SMTP address of a sender.</span></span> <span data-ttu-id="07dc1-107">Изначально у пользователя нет переопределений.</span><span class="sxs-lookup"><span data-stu-id="07dc1-107">Initially, a user does not have any overrides.</span></span>
## <a name="permissions"></a><span data-ttu-id="07dc1-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="07dc1-108">Permissions</span></span>
<span data-ttu-id="07dc1-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="07dc1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07dc1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="07dc1-111">Permission type</span></span>      | <span data-ttu-id="07dc1-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="07dc1-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="07dc1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="07dc1-113">Delegated (work or school account)</span></span> | <span data-ttu-id="07dc1-114">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="07dc1-114">Mail.Read</span></span>    |
|<span data-ttu-id="07dc1-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="07dc1-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="07dc1-116">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="07dc1-116">Mail.Read</span></span>    |
|<span data-ttu-id="07dc1-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="07dc1-117">Application</span></span> | <span data-ttu-id="07dc1-118">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="07dc1-118">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="07dc1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="07dc1-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/inferenceClassification/overrides
GET /users/{id}/inferenceClassification/overrides
```

## <a name="request-headers"></a><span data-ttu-id="07dc1-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="07dc1-120">Request headers</span></span>
| <span data-ttu-id="07dc1-121">Имя</span><span class="sxs-lookup"><span data-stu-id="07dc1-121">Name</span></span>       | <span data-ttu-id="07dc1-122">Тип</span><span class="sxs-lookup"><span data-stu-id="07dc1-122">Type</span></span> | <span data-ttu-id="07dc1-123">Описание</span><span class="sxs-lookup"><span data-stu-id="07dc1-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="07dc1-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="07dc1-124">Authorization</span></span>  | <span data-ttu-id="07dc1-125">string</span><span class="sxs-lookup"><span data-stu-id="07dc1-125">string</span></span>  | <span data-ttu-id="07dc1-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="07dc1-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="07dc1-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="07dc1-128">Request body</span></span>
<span data-ttu-id="07dc1-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="07dc1-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="07dc1-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="07dc1-130">Response</span></span>

<span data-ttu-id="07dc1-131">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="07dc1-131">If successful, this method returns a `200 OK` response code and a collection of [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="07dc1-132">Пример</span><span class="sxs-lookup"><span data-stu-id="07dc1-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="07dc1-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="07dc1-133">Request</span></span>
<span data-ttu-id="07dc1-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="07dc1-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="07dc1-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="07dc1-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_overrides"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/inferenceClassification/overrides
```
# <a name="c"></a>[<span data-ttu-id="07dc1-136">C#</span><span class="sxs-lookup"><span data-stu-id="07dc1-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-overrides-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="07dc1-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="07dc1-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-overrides-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="07dc1-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="07dc1-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-overrides-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="07dc1-139">Java</span><span class="sxs-lookup"><span data-stu-id="07dc1-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-overrides-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="07dc1-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="07dc1-140">Response</span></span>
<span data-ttu-id="07dc1-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="07dc1-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


