---
title: Переопределение списка
description: Получение параметров сортировки папки "Входящие", которые пользователь настроил для того, чтобы всегда классифицировать сообщения от определенных отправителей определенными способами.
localization_priority: Normal
doc_type: apiPageType
author: ''
ms.prod: ''
ms.openlocfilehash: 8c824ed0ee2809281974006209773731919630f2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35953106"
---
# <a name="list-overrides"></a><span data-ttu-id="29d6a-103">Переопределение списка</span><span class="sxs-lookup"><span data-stu-id="29d6a-103">List overrides</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="29d6a-104">Получение параметров [сортировки папки "Входящие"](../resources/manage-focused-inbox.md) , которые пользователь настроил для того, чтобы всегда классифицировать сообщения от определенных отправителей определенными способами.</span><span class="sxs-lookup"><span data-stu-id="29d6a-104">Get the [Focused Inbox](../resources/manage-focused-inbox.md) overrides that a user has set up to always classify messages from certain senders in specific ways.</span></span>

<span data-ttu-id="29d6a-105">Каждое переопределение соответствует SMTP-адресу отправителя.</span><span class="sxs-lookup"><span data-stu-id="29d6a-105">Each override corresponds to an SMTP address of a sender.</span></span> <span data-ttu-id="29d6a-106">Изначально у пользователя нет переопределений.</span><span class="sxs-lookup"><span data-stu-id="29d6a-106">Initially, a user does not have any overrides.</span></span>
## <a name="permissions"></a><span data-ttu-id="29d6a-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="29d6a-107">Permissions</span></span>
<span data-ttu-id="29d6a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="29d6a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="29d6a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="29d6a-110">Permission type</span></span>      | <span data-ttu-id="29d6a-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="29d6a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="29d6a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="29d6a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="29d6a-113">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="29d6a-113">Mail.Read</span></span>    |
|<span data-ttu-id="29d6a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="29d6a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="29d6a-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="29d6a-115">Mail.Read</span></span>    |
|<span data-ttu-id="29d6a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="29d6a-116">Application</span></span> | <span data-ttu-id="29d6a-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="29d6a-117">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="29d6a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="29d6a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/inferenceClassification/overrides
GET /users/{id}/inferenceClassification/overrides
```

## <a name="request-headers"></a><span data-ttu-id="29d6a-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="29d6a-119">Request headers</span></span>
| <span data-ttu-id="29d6a-120">Имя</span><span class="sxs-lookup"><span data-stu-id="29d6a-120">Name</span></span>       | <span data-ttu-id="29d6a-121">Тип</span><span class="sxs-lookup"><span data-stu-id="29d6a-121">Type</span></span> | <span data-ttu-id="29d6a-122">Описание</span><span class="sxs-lookup"><span data-stu-id="29d6a-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="29d6a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="29d6a-123">Authorization</span></span>  | <span data-ttu-id="29d6a-124">string</span><span class="sxs-lookup"><span data-stu-id="29d6a-124">string</span></span>  | <span data-ttu-id="29d6a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="29d6a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="29d6a-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="29d6a-127">Request body</span></span>
<span data-ttu-id="29d6a-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="29d6a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="29d6a-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="29d6a-129">Response</span></span>

<span data-ttu-id="29d6a-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="29d6a-130">If successful, this method returns a `200 OK` response code and a collection of [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="29d6a-131">Пример</span><span class="sxs-lookup"><span data-stu-id="29d6a-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="29d6a-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="29d6a-132">Request</span></span>
<span data-ttu-id="29d6a-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="29d6a-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="29d6a-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="29d6a-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_overrides"
}-->
```http
GET https://graph.microsoft.com/beta/me/inferenceClassification/overrides
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="29d6a-135">C#</span><span class="sxs-lookup"><span data-stu-id="29d6a-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-overrides-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="29d6a-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="29d6a-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-overrides-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="29d6a-137">Цель — C</span><span class="sxs-lookup"><span data-stu-id="29d6a-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-overrides-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="29d6a-138">Java</span><span class="sxs-lookup"><span data-stu-id="29d6a-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-overrides-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="29d6a-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="29d6a-139">Response</span></span>
<span data-ttu-id="29d6a-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="29d6a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
