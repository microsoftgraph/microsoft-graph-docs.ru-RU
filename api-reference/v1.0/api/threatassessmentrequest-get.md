---
title: Получение объекта threatAssessmentRequest
description: Получение свойств и связей указанного объекта среатассессментрекуест.
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9b68ccdcb31dcc4f90e8b90f7590e69e912deb94
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47978316"
---
# <a name="get-threatassessmentrequest"></a><span data-ttu-id="d52b7-103">Получение объекта threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="d52b7-103">Get threatAssessmentRequest</span></span>

<span data-ttu-id="d52b7-104">Получение свойств и связей указанного объекта [среатассессментрекуест](../resources/threatassessmentrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="d52b7-104">Retrieve the properties and relationships of a specified [threatAssessmentRequest](../resources/threatassessmentrequest.md) object.</span></span>

<span data-ttu-id="d52b7-105">Запрос на оценку угроз может иметь один из следующих типов:</span><span class="sxs-lookup"><span data-stu-id="d52b7-105">A threat assessment request can be one of the following types:</span></span>

* [<span data-ttu-id="d52b7-106">Почта</span><span class="sxs-lookup"><span data-stu-id="d52b7-106">Mail</span></span>](../resources/mailAssessmentRequest.md)
* [<span data-ttu-id="d52b7-107">Файл электронной почты</span><span class="sxs-lookup"><span data-stu-id="d52b7-107">Email file</span></span>](../resources/emailFileAssessmentRequest.md)
* [<span data-ttu-id="d52b7-108">File</span><span class="sxs-lookup"><span data-stu-id="d52b7-108">File</span></span>](../resources/fileAssessmentRequest.md)
* [<span data-ttu-id="d52b7-109">URL-адрес</span><span class="sxs-lookup"><span data-stu-id="d52b7-109">URL</span></span>](../resources/urlAssessmentRequest.md)

## <a name="permissions"></a><span data-ttu-id="d52b7-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d52b7-110">Permissions</span></span>

<span data-ttu-id="d52b7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d52b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d52b7-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d52b7-113">Permission type</span></span>                        | <span data-ttu-id="d52b7-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d52b7-114">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d52b7-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d52b7-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="d52b7-116">Среатассессмент. ReadWrite. ALL.</span><span class="sxs-lookup"><span data-stu-id="d52b7-116">ThreatAssessment.ReadWrite.All.</span></span>             |
| <span data-ttu-id="d52b7-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d52b7-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d52b7-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d52b7-118">Not supported.</span></span>                              |
| <span data-ttu-id="d52b7-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d52b7-119">Application</span></span>                            | <span data-ttu-id="d52b7-120">Среатассессмент. Read. ALL.</span><span class="sxs-lookup"><span data-stu-id="d52b7-120">ThreatAssessment.Read.All.</span></span>                  |

## <a name="http-request"></a><span data-ttu-id="d52b7-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d52b7-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /informationProtection/threatAssessmentRequests/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d52b7-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d52b7-122">Optional query parameters</span></span>

<span data-ttu-id="d52b7-123">Этот метод поддерживает следующие параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d52b7-123">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="d52b7-124">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="d52b7-124">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

|<span data-ttu-id="d52b7-125">Имя</span><span class="sxs-lookup"><span data-stu-id="d52b7-125">Name</span></span>            |<span data-ttu-id="d52b7-126">Значение</span><span class="sxs-lookup"><span data-stu-id="d52b7-126">Value</span></span>    |<span data-ttu-id="d52b7-127">Описание</span><span class="sxs-lookup"><span data-stu-id="d52b7-127">Description</span></span>                                                                                                                                                                 |
|:---------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="d52b7-128">$expand</span><span class="sxs-lookup"><span data-stu-id="d52b7-128">$expand</span></span>         |<span data-ttu-id="d52b7-129">string</span><span class="sxs-lookup"><span data-stu-id="d52b7-129">string</span></span>   |<span data-ttu-id="d52b7-130">Использование `$expand=results` в запросе для получения результатов оценки угроз.</span><span class="sxs-lookup"><span data-stu-id="d52b7-130">Using `$expand=results` in the query to retrieve the threat assessment result.</span></span>                                                                                              |
|<span data-ttu-id="d52b7-131">$select</span><span class="sxs-lookup"><span data-stu-id="d52b7-131">$select</span></span>         |<span data-ttu-id="d52b7-132">string</span><span class="sxs-lookup"><span data-stu-id="d52b7-132">string</span></span>   |<span data-ttu-id="d52b7-p103">Список разделенных запятыми свойств, которые необходимо включить в отклик. Для оптимизации производительности выбирайте только необходимые свойства.</span><span class="sxs-lookup"><span data-stu-id="d52b7-p103">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>                                        |

## <a name="request-headers"></a><span data-ttu-id="d52b7-135">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d52b7-135">Request headers</span></span>

| <span data-ttu-id="d52b7-136">Имя</span><span class="sxs-lookup"><span data-stu-id="d52b7-136">Name</span></span>      |<span data-ttu-id="d52b7-137">Описание</span><span class="sxs-lookup"><span data-stu-id="d52b7-137">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d52b7-138">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d52b7-138">Authorization</span></span> | <span data-ttu-id="d52b7-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d52b7-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d52b7-141">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d52b7-141">Request body</span></span>

<span data-ttu-id="d52b7-142">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d52b7-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d52b7-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="d52b7-143">Response</span></span>

<span data-ttu-id="d52b7-144">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [среатассессментрекуест](../resources/threatassessmentrequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d52b7-144">If successful, this method returns a `200 OK` response code and the requested [threatAssessmentRequest](../resources/threatassessmentrequest.md) object in the response body.</span></span> <span data-ttu-id="d52b7-145">Возвращаются свойства этого типа: [маилассессментрекуест](../resources/mailAssessmentRequest.md), [емаилфилеассессментрекуест](../resources/emailFileAssessmentRequest.md), [филеассессментрекуест](../resources/fileAssessmentRequest.md), [урлассессментрекуест](../resources/urlAssessmentRequest.md).</span><span class="sxs-lookup"><span data-stu-id="d52b7-145">The properties of that type are returned: [mailAssessmentRequest](../resources/mailAssessmentRequest.md), [emailFileAssessmentRequest](../resources/emailFileAssessmentRequest.md), [fileAssessmentRequest](../resources/fileAssessmentRequest.md), [urlAssessmentRequest](../resources/urlAssessmentRequest.md).</span></span>

## <a name="examples"></a><span data-ttu-id="d52b7-146">Примеры</span><span class="sxs-lookup"><span data-stu-id="d52b7-146">Examples</span></span>

### <a name="example-1-get-the-properties-of-a-mail-assessment-request"></a><span data-ttu-id="d52b7-147">Пример 1: получение свойств запроса на оценку почты</span><span class="sxs-lookup"><span data-stu-id="d52b7-147">Example 1: Get the properties of a mail assessment request</span></span>

#### <a name="request"></a><span data-ttu-id="d52b7-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="d52b7-148">Request</span></span>

<span data-ttu-id="d52b7-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d52b7-149">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d52b7-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="d52b7-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mailassessmentrequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/informationProtection/threatAssessmentRequests/49c5ef5b-1f65-444a-e6b9-08d772ea2059
```
# <a name="c"></a>[<span data-ttu-id="d52b7-151">C#</span><span class="sxs-lookup"><span data-stu-id="d52b7-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailassessmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d52b7-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d52b7-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailassessmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d52b7-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d52b7-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailassessmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d52b7-154">Java</span><span class="sxs-lookup"><span data-stu-id="d52b7-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-mailassessmentrequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d52b7-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="d52b7-155">Response</span></span>

<span data-ttu-id="d52b7-156">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d52b7-156">The following is an example of the response.</span></span>

> <span data-ttu-id="d52b7-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d52b7-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailAssessmentRequest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#informationProtection/threatAssessmentRequests/$entity",
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
  "messageUri": "https://graph.microsoft.com/v1.0/users/c52ce8db-3e4b-4181-93c4-7d6b6bffaf60/messages/AAMkADU3MWUxOTU0LWNlOTEt=",
  "createdBy": {
    "user": {
      "id": "c52ce8db-3e4b-4181-93c4-7d6b6bffaf60",
      "displayName": "Ronald Admin"
    }
  }
}
```

### <a name="example-2-get-the-properties-of-an-email-file-assessment-request"></a><span data-ttu-id="d52b7-159">Пример 2: получение свойств запроса на оценку файла электронной почты</span><span class="sxs-lookup"><span data-stu-id="d52b7-159">Example 2: Get the properties of an email file assessment request</span></span>

#### <a name="request"></a><span data-ttu-id="d52b7-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="d52b7-160">Request</span></span>

<span data-ttu-id="d52b7-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d52b7-161">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d52b7-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="d52b7-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_emailfileassessmentrequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/informationProtection/threatAssessmentRequests/ab2ad9b3-2213-4091-ae0c-08d76ddbcacf
```
# <a name="c"></a>[<span data-ttu-id="d52b7-163">C#</span><span class="sxs-lookup"><span data-stu-id="d52b7-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-emailfileassessmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d52b7-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d52b7-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-emailfileassessmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d52b7-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d52b7-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-emailfileassessmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d52b7-166">Java</span><span class="sxs-lookup"><span data-stu-id="d52b7-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-emailfileassessmentrequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d52b7-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="d52b7-167">Response</span></span>

<span data-ttu-id="d52b7-168">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d52b7-168">The following is an example of the response.</span></span>

> <span data-ttu-id="d52b7-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d52b7-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailFileAssessmentRequest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#informationProtection/threatAssessmentRequests/$entity",
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
}
```

### <a name="example-3-get-the-properties-of-a-file-assessment-request"></a><span data-ttu-id="d52b7-171">Пример 3: получение свойств запроса на оценку файла</span><span class="sxs-lookup"><span data-stu-id="d52b7-171">Example 3: Get the properties of a file assessment request</span></span>

#### <a name="request"></a><span data-ttu-id="d52b7-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="d52b7-172">Request</span></span>

<span data-ttu-id="d52b7-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d52b7-173">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d52b7-174">HTTP</span><span class="sxs-lookup"><span data-stu-id="d52b7-174">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_fileassessmentrequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/informationProtection/threatAssessmentRequests/18406a56-7209-4720-a250-08d772fccdaa
```
# <a name="c"></a>[<span data-ttu-id="d52b7-175">C#</span><span class="sxs-lookup"><span data-stu-id="d52b7-175">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-fileassessmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d52b7-176">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d52b7-176">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-fileassessmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d52b7-177">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d52b7-177">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-fileassessmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d52b7-178">Java</span><span class="sxs-lookup"><span data-stu-id="d52b7-178">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-fileassessmentrequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d52b7-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="d52b7-179">Response</span></span>

<span data-ttu-id="d52b7-180">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d52b7-180">The following is an example of the response.</span></span>

> <span data-ttu-id="d52b7-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d52b7-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.fileAssessmentRequest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#informationProtection/threatAssessmentRequests/$entity",
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
}
```

### <a name="example-4-get-the-properties-of-an-url-assessment-request"></a><span data-ttu-id="d52b7-183">Пример 4: получение свойств запроса на оценку URL-адреса</span><span class="sxs-lookup"><span data-stu-id="d52b7-183">Example 4: Get the properties of an url assessment request</span></span>

#### <a name="request"></a><span data-ttu-id="d52b7-184">Запрос</span><span class="sxs-lookup"><span data-stu-id="d52b7-184">Request</span></span>

<span data-ttu-id="d52b7-185">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d52b7-185">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d52b7-186">HTTP</span><span class="sxs-lookup"><span data-stu-id="d52b7-186">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_urlassessmentrequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/informationProtection/threatAssessmentRequests/723c35be-8b5a-47ae-29c0-08d76ddb7f5b
```
# <a name="c"></a>[<span data-ttu-id="d52b7-187">C#</span><span class="sxs-lookup"><span data-stu-id="d52b7-187">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-urlassessmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d52b7-188">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d52b7-188">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-urlassessmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d52b7-189">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d52b7-189">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-urlassessmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d52b7-190">Java</span><span class="sxs-lookup"><span data-stu-id="d52b7-190">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-urlassessmentrequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d52b7-191">Отклик</span><span class="sxs-lookup"><span data-stu-id="d52b7-191">Response</span></span>

<span data-ttu-id="d52b7-192">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d52b7-192">The following is an example of the response.</span></span>

> <span data-ttu-id="d52b7-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d52b7-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.urlAssessmentRequest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#informationProtection/threatAssessmentRequests/$entity",
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
```

### <a name="example-5-expand-threat-assessment-results-for-a-request"></a><span data-ttu-id="d52b7-195">Пример 5: развертывание результатов оценки угроз для запроса</span><span class="sxs-lookup"><span data-stu-id="d52b7-195">Example 5: Expand threat assessment results for a request</span></span>

#### <a name="request"></a><span data-ttu-id="d52b7-196">Запрос</span><span class="sxs-lookup"><span data-stu-id="d52b7-196">Request</span></span>

<span data-ttu-id="d52b7-197">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d52b7-197">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d52b7-198">HTTP</span><span class="sxs-lookup"><span data-stu-id="d52b7-198">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_threatassessmentrequest_expand_results"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/informationProtection/threatAssessmentRequests/11922306-b25b-4605-ff0d-08d772fcf996?$expand=results
```
# <a name="c"></a>[<span data-ttu-id="d52b7-199">C#</span><span class="sxs-lookup"><span data-stu-id="d52b7-199">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-threatassessmentrequest-expand-results-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d52b7-200">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d52b7-200">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-threatassessmentrequest-expand-results-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d52b7-201">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d52b7-201">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-threatassessmentrequest-expand-results-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d52b7-202">Java</span><span class="sxs-lookup"><span data-stu-id="d52b7-202">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-threatassessmentrequest-expand-results-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d52b7-203">Отклик</span><span class="sxs-lookup"><span data-stu-id="d52b7-203">Response</span></span>

<span data-ttu-id="d52b7-204">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d52b7-204">The following is an example of the response.</span></span>

> <span data-ttu-id="d52b7-p110">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d52b7-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailAssessmentRequest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#informationProtection/threatAssessmentRequests(results())/$entity",
    "@odata.type": "#microsoft.graph.mailAssessmentRequest",
    "id": "11922306-b25b-4605-ff0d-08d772fcf996",
    "createdDateTime": "2019-11-27T05:45:14.0962061Z",
    "contentType": "mail",
    "expectedAssessment": "block",
    "category": "phishing",
    "status": "completed",
    "requestSource": "administrator",
    "recipientEmail": "tifc@a830edad9050849eqtpwbjzxodq.onmicrosoft.com",
    "destinationRoutingReason": "notJunk",
    "messageUri": "",
    "createdBy": {
      "user": {
        "id": "c52ce8db-3e4b-4181-93c4-7d6b6bffaf60",
        "displayName": "Ronald Admin"
      }
    },
    "results@odata.context": "https://graph.microsoft.com/v1.0/$metadata#informationProtection/threatAssessmentRequests('11922306-b25b-4605-ff0d-08d772fcf996')/microsoft.graph.mailAssessmentRequest/results",
    "results": [
        {
            "id": "63798129-a62c-4f9e-2c6d-08d772fcfb0e",
            "createdDateTime": "2019-11-27T05:45:16.55Z",
            "resultType": "checkPolicy",
            "message": "No policy was hit."
        },
        {
            "id": "d38c2448-79eb-467e-2495-08d772fdb7d1",
            "createdDateTime": "2019-11-27T05:50:33.243Z",
            "resultType": "rescan",
            "message": "Not Spam"
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get threatAssessmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

