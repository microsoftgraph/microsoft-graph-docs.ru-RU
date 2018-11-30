---
title: Список переопределений
description: Получение переопределений, настроенных пользователем для классификации сообщений от определенных отправителей.
ms.openlocfilehash: 7953c776b60f4e63aec03245817bfcf6630bbdf8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024700"
---
# <a name="list-overrides"></a><span data-ttu-id="464e9-103">Список переопределений</span><span class="sxs-lookup"><span data-stu-id="464e9-103">List overrides</span></span>

<span data-ttu-id="464e9-104">Получение переопределений, настроенных пользователем для классификации сообщений от определенных отправителей.</span><span class="sxs-lookup"><span data-stu-id="464e9-104">Get the overrides that a user has set up to always classify messages from certain senders in specific ways.</span></span>

<span data-ttu-id="464e9-p101">Каждое переопределение соответствует SMTP-адресу отправителя. Изначально у пользователя нет переопределений.</span><span class="sxs-lookup"><span data-stu-id="464e9-p101">Each override corresponds to an SMTP address of a sender. Initially, a user does not have any overrides.</span></span>
## <a name="permissions"></a><span data-ttu-id="464e9-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="464e9-107">Permissions</span></span>
<span data-ttu-id="464e9-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="464e9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="464e9-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="464e9-110">Permission type</span></span>      | <span data-ttu-id="464e9-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="464e9-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="464e9-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="464e9-112">Delegated (work or school account)</span></span> | <span data-ttu-id="464e9-113">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="464e9-113">Mail.Read</span></span>    |
|<span data-ttu-id="464e9-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="464e9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="464e9-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="464e9-115">Mail.Read</span></span>    |
|<span data-ttu-id="464e9-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="464e9-116">Application</span></span> | <span data-ttu-id="464e9-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="464e9-117">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="464e9-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="464e9-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/inferenceClassification/overrides
GET /users/{id}/inferenceClassification/overrides
```

## <a name="request-headers"></a><span data-ttu-id="464e9-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="464e9-119">Request headers</span></span>
| <span data-ttu-id="464e9-120">Имя</span><span class="sxs-lookup"><span data-stu-id="464e9-120">Name</span></span>       | <span data-ttu-id="464e9-121">Тип</span><span class="sxs-lookup"><span data-stu-id="464e9-121">Type</span></span> | <span data-ttu-id="464e9-122">Описание</span><span class="sxs-lookup"><span data-stu-id="464e9-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="464e9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="464e9-123">Authorization</span></span>  | <span data-ttu-id="464e9-124">string</span><span class="sxs-lookup"><span data-stu-id="464e9-124">string</span></span>  | <span data-ttu-id="464e9-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="464e9-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="464e9-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="464e9-127">Request body</span></span>
<span data-ttu-id="464e9-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="464e9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="464e9-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="464e9-129">Response</span></span>

<span data-ttu-id="464e9-p104">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) в тексте отклика. Если у пользователя нет настроенных переопределений, возвращается пустая коллекция.</span><span class="sxs-lookup"><span data-stu-id="464e9-p104">If successful, this method returns a `200 OK` response code and a collection of [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) objects in the response body. An empty collection is returned if the user doesn't have any overrides set up.</span></span>
## <a name="example"></a><span data-ttu-id="464e9-132">Пример</span><span class="sxs-lookup"><span data-stu-id="464e9-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="464e9-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="464e9-133">Request</span></span>
<span data-ttu-id="464e9-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="464e9-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_overrides"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/inferenceClassification/overrides
```
##### <a name="response"></a><span data-ttu-id="464e9-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="464e9-135">Response</span></span>
<span data-ttu-id="464e9-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="464e9-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->