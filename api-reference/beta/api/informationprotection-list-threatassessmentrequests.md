---
title: List threatAssessmentRequests
description: Извлечение списка объектов threatassessmentrequest.
localization_priority: Normal
author: hafen-ms
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: d830c80c71e0873806d67ff0e6196a1bdc4d6483
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52040513"
---
# <a name="list-threatassessmentrequests"></a><span data-ttu-id="2a2eb-103">List threatAssessmentRequests</span><span class="sxs-lookup"><span data-stu-id="2a2eb-103">List threatAssessmentRequests</span></span>

<span data-ttu-id="2a2eb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2a2eb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2a2eb-105">Извлечение списка [объектов threatAssessmentRequest.](../resources/threatassessmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="2a2eb-105">Retrieve a list of [threatAssessmentRequest](../resources/threatassessmentrequest.md) objects.</span></span>

<span data-ttu-id="2a2eb-106">Запрос на оценку угроз может быть одним из следующих типов:</span><span class="sxs-lookup"><span data-stu-id="2a2eb-106">A threat assessment request can be one of the following types:</span></span>

* [<span data-ttu-id="2a2eb-107">Почта</span><span class="sxs-lookup"><span data-stu-id="2a2eb-107">Mail</span></span>](../resources/mailAssessmentRequest.md)
* [<span data-ttu-id="2a2eb-108">Файл электронной почты</span><span class="sxs-lookup"><span data-stu-id="2a2eb-108">Email file</span></span>](../resources/emailFileAssessmentRequest.md)
* [<span data-ttu-id="2a2eb-109">Файл</span><span class="sxs-lookup"><span data-stu-id="2a2eb-109">File</span></span>](../resources/fileAssessmentRequest.md)
* [<span data-ttu-id="2a2eb-110">URL-адрес</span><span class="sxs-lookup"><span data-stu-id="2a2eb-110">URL</span></span>](../resources/urlAssessmentRequest.md)

## <a name="permissions"></a><span data-ttu-id="2a2eb-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2a2eb-111">Permissions</span></span>

<span data-ttu-id="2a2eb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2a2eb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2a2eb-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2a2eb-114">Permission type</span></span>                        | <span data-ttu-id="2a2eb-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2a2eb-115">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2a2eb-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2a2eb-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="2a2eb-117">ThreatAssessment.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a2eb-117">ThreatAssessment.ReadWrite.All</span></span>             |
| <span data-ttu-id="2a2eb-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2a2eb-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2a2eb-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a2eb-119">Not supported.</span></span>                              |
| <span data-ttu-id="2a2eb-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2a2eb-120">Application</span></span>                            | <span data-ttu-id="2a2eb-121">ThreatAssessment.Read.All</span><span class="sxs-lookup"><span data-stu-id="2a2eb-121">ThreatAssessment.Read.All</span></span>                  |

## <a name="http-request"></a><span data-ttu-id="2a2eb-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2a2eb-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /informationProtection/threatAssessmentRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2a2eb-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2a2eb-123">Optional query parameters</span></span>

<span data-ttu-id="2a2eb-124">Этот метод поддерживает следующие параметры запроса OData, чтобы помочь настроить ответ.</span><span class="sxs-lookup"><span data-stu-id="2a2eb-124">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="2a2eb-125">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="2a2eb-125">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

|<span data-ttu-id="2a2eb-126">Имя</span><span class="sxs-lookup"><span data-stu-id="2a2eb-126">Name</span></span>            |<span data-ttu-id="2a2eb-127">Значение</span><span class="sxs-lookup"><span data-stu-id="2a2eb-127">Value</span></span>    |<span data-ttu-id="2a2eb-128">Описание</span><span class="sxs-lookup"><span data-stu-id="2a2eb-128">Description</span></span>                                                                                                                                                                 |
|:---------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="2a2eb-129">$filter</span><span class="sxs-lookup"><span data-stu-id="2a2eb-129">$filter</span></span>         |<span data-ttu-id="2a2eb-130">string</span><span class="sxs-lookup"><span data-stu-id="2a2eb-130">string</span></span>   |<span data-ttu-id="2a2eb-131">Ограничивает ответ только теми объектами, которые содержат указанные критерии.</span><span class="sxs-lookup"><span data-stu-id="2a2eb-131">Limits the response to only those objects which contain the specified criteria.</span></span>                                                                                             |
|<span data-ttu-id="2a2eb-132">$orderby</span><span class="sxs-lookup"><span data-stu-id="2a2eb-132">$orderby</span></span>        |<span data-ttu-id="2a2eb-133">строка</span><span class="sxs-lookup"><span data-stu-id="2a2eb-133">string</span></span>   |<span data-ttu-id="2a2eb-134">По умолчанию объекты в ответе будут нисходящими по своему **значению createdDateTime.**</span><span class="sxs-lookup"><span data-stu-id="2a2eb-134">By default, the objects in the response are descending ordered by their **createdDateTime** value.</span></span>                                                                          |
|<span data-ttu-id="2a2eb-135">$select</span><span class="sxs-lookup"><span data-stu-id="2a2eb-135">$select</span></span>         |<span data-ttu-id="2a2eb-136">string</span><span class="sxs-lookup"><span data-stu-id="2a2eb-136">string</span></span>   |<span data-ttu-id="2a2eb-p103">Список разделенных запятыми свойств, которые необходимо включить в отклик. Для оптимизации производительности выбирайте только необходимые свойства.</span><span class="sxs-lookup"><span data-stu-id="2a2eb-p103">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>                                        |
|<span data-ttu-id="2a2eb-139">$skipToken</span><span class="sxs-lookup"><span data-stu-id="2a2eb-139">$skipToken</span></span>      |<span data-ttu-id="2a2eb-140">string</span><span class="sxs-lookup"><span data-stu-id="2a2eb-140">string</span></span>   |<span data-ttu-id="2a2eb-141">Возвращает следующую страницу результатов из результирующих наборов, занимающих несколько страниц.</span><span class="sxs-lookup"><span data-stu-id="2a2eb-141">Retrieves the next page of results from result sets that span multiple pages.</span></span>                                                                                               |

## <a name="request-headers"></a><span data-ttu-id="2a2eb-142">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2a2eb-142">Request headers</span></span>

| <span data-ttu-id="2a2eb-143">Имя</span><span class="sxs-lookup"><span data-stu-id="2a2eb-143">Name</span></span>      |<span data-ttu-id="2a2eb-144">Описание</span><span class="sxs-lookup"><span data-stu-id="2a2eb-144">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2a2eb-145">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2a2eb-145">Authorization</span></span> | <span data-ttu-id="2a2eb-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2a2eb-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2a2eb-148">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2a2eb-148">Request body</span></span>

<span data-ttu-id="2a2eb-149">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2a2eb-149">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2a2eb-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="2a2eb-150">Response</span></span>

<span data-ttu-id="2a2eb-151">В случае успешного выполнения этот метод возвращает код ответа и коллекцию объектов `200 OK` [threatAssessmentRequest](../resources/threatassessmentrequest.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="2a2eb-151">If successful, this method returns a `200 OK` response code and a collection of [threatAssessmentRequest](../resources/threatassessmentrequest.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2a2eb-152">Примеры</span><span class="sxs-lookup"><span data-stu-id="2a2eb-152">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2a2eb-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="2a2eb-153">Request</span></span>

<span data-ttu-id="2a2eb-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2a2eb-154">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2a2eb-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="2a2eb-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_threatassessmentrequests"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/informationProtection/threatAssessmentRequests
```
# <a name="c"></a>[<span data-ttu-id="2a2eb-156">C#</span><span class="sxs-lookup"><span data-stu-id="2a2eb-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-threatassessmentrequests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2a2eb-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2a2eb-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-threatassessmentrequests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2a2eb-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2a2eb-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-threatassessmentrequests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2a2eb-159">Java</span><span class="sxs-lookup"><span data-stu-id="2a2eb-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-threatassessmentrequests-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2a2eb-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="2a2eb-160">Response</span></span>

<span data-ttu-id="2a2eb-161">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="2a2eb-161">The following is an example of the response.</span></span>

> <span data-ttu-id="2a2eb-162">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="2a2eb-162">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.threatAssessmentRequest",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#informationProtection/threatAssessmentRequests",
  "@odata.nextLink": "https://graph.microsoft.com/beta/informationProtection/threatAssessmentRequests?$skiptoken=eyJQYWdlQ29va2llIjoiPHJvdyBpZF9JZGVudGl0",
  "value": [
    {
      "@odata.type": "#microsoft.graph.mailAssessmentRequest",
      "id": "49c5ef5b-1f65-444a-e6b9-08d772ea2059",
      "createdDateTime": "2019-11-27T03:30:18.6890937Z",
      "contentType": "mail",
      "expectedAssessment": "block",
      "category": "spam",
      "status": "pending",
      "requestSource": "administrator",
      "recipientEmail": "tifc@a830edad9050849eqtpwbjzxodq.onmicrosoft.com",
      "destinationRoutingReason": "notJunk",
      "messageUri": "https://graph.microsoft.com/beta/users/c52ce8db-3e4b-4181-93c4-7d6b6bffaf60/messages/AAMkADU3MWUxOTU0LWNlOTEt=",
      "createdBy": {
        "user": {
          "id": "c52ce8db-3e4b-4181-93c4-7d6b6bffaf60",
          "displayName": "Ronald Admin"
        }
      }
    },
    {
      "@odata.type": "#microsoft.graph.emailFileAssessmentRequest",
      "id": "ab2ad9b3-2213-4091-ae0c-08d76ddbcacf",
      "createdDateTime": "2019-11-20T17:05:06.4088076Z",
      "contentType": "mail",
      "expectedAssessment": "block",
      "category": "malware",
      "status": "completed",
      "requestSource": "administrator",
      "recipientEmail": "tifc@a830edad9050849EQTPWBJZXODQ.onmicrosoft.com",
      "destinationRoutingReason": "notJunk",
      "contentData": "",
      "createdBy": {
        "user": {
          "id": "c52ce8db-3e4b-4181-93c4-7d6b6bffaf60",
          "displayName": "Ronald Admin"
        }
      }
    },
    {
      "@odata.type": "#microsoft.graph.fileAssessmentRequest",
      "id": "18406a56-7209-4720-a250-08d772fccdaa",
      "createdDateTime": "2019-11-27T05:44:00.4051536Z",
      "contentType": "file",
      "expectedAssessment": "block",
      "category": "malware",
      "status": "completed",
      "requestSource": "administrator",
      "fileName": "b3d5b715-4b88-4bbb-b0ae-9a9281a3f18a.csv",
      "contentData": "",
      "createdBy": {
        "user": {
          "id": "c52ce8db-3e4b-4181-93c4-7d6b6bffaf60",
          "displayName": "Ronald Admin"
        }
      }
    },
    {
      "@odata.type": "#microsoft.graph.urlAssessmentRequest",
      "id": "723c35be-8b5a-47ae-29c0-08d76ddb7f5b",
      "createdDateTime": "2019-11-20T17:02:59.8160832Z",
      "contentType": "url",
      "expectedAssessment": "unblock",
      "category": "phishing",
      "status": "completed",
      "requestSource": "administrator",
      "url": "http://test.com",
      "createdBy": {
        "user": {
          "id": "c52ce8db-3e4b-4181-93c4-7d6b6bffaf60",
          "displayName": "Ronald Admin"
        }
      }
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List threatAssessmentRequests",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


