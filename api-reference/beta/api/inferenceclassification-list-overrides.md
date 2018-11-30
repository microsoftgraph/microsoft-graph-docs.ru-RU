---
title: Список переопределений
description: Получите переопределения фокус папки "Входящие", пользователь настроил для всегда классификации сообщения от определенных отправителей различными способами.
ms.openlocfilehash: 343faaacf47d16b723cd8aebc25a6df79ef7e3db
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082084"
---
# <a name="list-overrides"></a><span data-ttu-id="a9d29-103">Список переопределений</span><span class="sxs-lookup"><span data-stu-id="a9d29-103">List overrides</span></span>

> <span data-ttu-id="a9d29-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a9d29-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a9d29-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a9d29-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a9d29-106">Получите переопределения [Фокус папки "Входящие"](../resources/manage-focused-inbox.md) , пользователь настроил для всегда классификации сообщения от определенных отправителей различными способами.</span><span class="sxs-lookup"><span data-stu-id="a9d29-106">Get the [Focused Inbox](../resources/manage-focused-inbox.md) overrides that a user has set up to always classify messages from certain senders in specific ways.</span></span>

<span data-ttu-id="a9d29-p102">Каждое переопределение соответствует SMTP-адресу отправителя. Изначально у пользователя нет переопределений.</span><span class="sxs-lookup"><span data-stu-id="a9d29-p102">Each override corresponds to an SMTP address of a sender. Initially, a user does not have any overrides.</span></span>
## <a name="permissions"></a><span data-ttu-id="a9d29-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a9d29-109">Permissions</span></span>
<span data-ttu-id="a9d29-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a9d29-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9d29-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a9d29-112">Permission type</span></span>      | <span data-ttu-id="a9d29-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a9d29-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a9d29-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a9d29-114">Delegated (work or school account)</span></span> | <span data-ttu-id="a9d29-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="a9d29-115">Mail.Read</span></span>    |
|<span data-ttu-id="a9d29-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a9d29-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a9d29-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="a9d29-117">Mail.Read</span></span>    |
|<span data-ttu-id="a9d29-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a9d29-118">Application</span></span> | <span data-ttu-id="a9d29-119">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="a9d29-119">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="a9d29-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a9d29-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/inferenceClassification/overrides
GET /users/{id}/inferenceClassification/overrides
```

## <a name="request-headers"></a><span data-ttu-id="a9d29-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a9d29-121">Request headers</span></span>
| <span data-ttu-id="a9d29-122">Имя</span><span class="sxs-lookup"><span data-stu-id="a9d29-122">Name</span></span>       | <span data-ttu-id="a9d29-123">Тип</span><span class="sxs-lookup"><span data-stu-id="a9d29-123">Type</span></span> | <span data-ttu-id="a9d29-124">Описание</span><span class="sxs-lookup"><span data-stu-id="a9d29-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a9d29-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="a9d29-125">Authorization</span></span>  | <span data-ttu-id="a9d29-126">string</span><span class="sxs-lookup"><span data-stu-id="a9d29-126">string</span></span>  | <span data-ttu-id="a9d29-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a9d29-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a9d29-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a9d29-129">Request body</span></span>
<span data-ttu-id="a9d29-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a9d29-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a9d29-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="a9d29-131">Response</span></span>

<span data-ttu-id="a9d29-132">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="a9d29-132">If successful, this method returns a `200 OK` response code and a collection of [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a9d29-133">Пример</span><span class="sxs-lookup"><span data-stu-id="a9d29-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a9d29-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="a9d29-134">Request</span></span>
<span data-ttu-id="a9d29-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a9d29-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_overrides"
}-->
```http
GET https://graph.microsoft.com/beta/me/inferenceClassification/overrides
```
##### <a name="response"></a><span data-ttu-id="a9d29-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="a9d29-136">Response</span></span>
<span data-ttu-id="a9d29-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="a9d29-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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