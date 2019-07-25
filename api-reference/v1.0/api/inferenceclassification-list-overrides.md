---
title: Переопределение списка
description: Получение переопределений, настроенных пользователем для классификации сообщений от определенных отправителей.
localization_priority: Normal
ms.openlocfilehash: 8bbe0eb84f03e4a6c11114c9eca78640e4f0036f
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35880874"
---
# <a name="list-overrides"></a><span data-ttu-id="a3d38-103">Переопределение списка</span><span class="sxs-lookup"><span data-stu-id="a3d38-103">List overrides</span></span>

<span data-ttu-id="a3d38-104">Получение переопределений, настроенных пользователем для классификации сообщений от определенных отправителей.</span><span class="sxs-lookup"><span data-stu-id="a3d38-104">Get the overrides that a user has set up to always classify messages from certain senders in specific ways.</span></span>

<span data-ttu-id="a3d38-p101">Каждое переопределение соответствует SMTP-адресу отправителя. Изначально у пользователя нет переопределений.</span><span class="sxs-lookup"><span data-stu-id="a3d38-p101">Each override corresponds to an SMTP address of a sender. Initially, a user does not have any overrides.</span></span>
## <a name="permissions"></a><span data-ttu-id="a3d38-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a3d38-107">Permissions</span></span>
<span data-ttu-id="a3d38-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a3d38-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3d38-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a3d38-110">Permission type</span></span>      | <span data-ttu-id="a3d38-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a3d38-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a3d38-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a3d38-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a3d38-113">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="a3d38-113">Mail.Read</span></span>    |
|<span data-ttu-id="a3d38-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a3d38-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a3d38-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="a3d38-115">Mail.Read</span></span>    |
|<span data-ttu-id="a3d38-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a3d38-116">Application</span></span> | <span data-ttu-id="a3d38-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="a3d38-117">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="a3d38-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a3d38-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/inferenceClassification/overrides
GET /users/{id}/inferenceClassification/overrides
```

## <a name="request-headers"></a><span data-ttu-id="a3d38-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a3d38-119">Request headers</span></span>
| <span data-ttu-id="a3d38-120">Имя</span><span class="sxs-lookup"><span data-stu-id="a3d38-120">Name</span></span>       | <span data-ttu-id="a3d38-121">Тип</span><span class="sxs-lookup"><span data-stu-id="a3d38-121">Type</span></span> | <span data-ttu-id="a3d38-122">Описание</span><span class="sxs-lookup"><span data-stu-id="a3d38-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a3d38-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a3d38-123">Authorization</span></span>  | <span data-ttu-id="a3d38-124">string</span><span class="sxs-lookup"><span data-stu-id="a3d38-124">string</span></span>  | <span data-ttu-id="a3d38-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a3d38-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a3d38-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a3d38-127">Request body</span></span>
<span data-ttu-id="a3d38-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a3d38-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a3d38-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="a3d38-129">Response</span></span>

<span data-ttu-id="a3d38-p104">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) в тексте отклика. Если у пользователя нет настроенных переопределений, возвращается пустая коллекция.</span><span class="sxs-lookup"><span data-stu-id="a3d38-p104">If successful, this method returns a `200 OK` response code and a collection of [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) objects in the response body. An empty collection is returned if the user doesn't have any overrides set up.</span></span>
## <a name="example"></a><span data-ttu-id="a3d38-132">Пример</span><span class="sxs-lookup"><span data-stu-id="a3d38-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a3d38-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="a3d38-133">Request</span></span>
<span data-ttu-id="a3d38-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a3d38-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a3d38-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="a3d38-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_overrides"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/inferenceClassification/overrides
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a3d38-136">C#</span><span class="sxs-lookup"><span data-stu-id="a3d38-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-overrides-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a3d38-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="a3d38-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-overrides-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a3d38-138">Цель — C</span><span class="sxs-lookup"><span data-stu-id="a3d38-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-overrides-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="a3d38-139">Java</span><span class="sxs-lookup"><span data-stu-id="a3d38-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-overrides-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a3d38-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="a3d38-140">Response</span></span>
<span data-ttu-id="a3d38-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a3d38-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List overrides",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
