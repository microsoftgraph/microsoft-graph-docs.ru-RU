---
title: Получение объекта threatAssessmentRequest
description: Получение свойств и связей указанного объекта среатассессментрекуест.
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ff1ab5527f58551bde3a3e3bcaada7e4a66e8692
ms.sourcegitcommit: 9edfcf99706c8490cd5832a1c706a88a89e24db1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/07/2020
ms.locfileid: "42452430"
---
# <a name="get-threatassessmentrequest"></a><span data-ttu-id="fbcdf-103">Получение объекта threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="fbcdf-103">Get threatAssessmentRequest</span></span>

<span data-ttu-id="fbcdf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fbcdf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fbcdf-105">Получение свойств и связей указанного объекта [среатассессментрекуест](../resources/threatassessmentrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="fbcdf-105">Retrieve the properties and relationships of a specified [threatAssessmentRequest](../resources/threatassessmentrequest.md) object.</span></span>

<span data-ttu-id="fbcdf-106">Запрос на оценку угроз может иметь один из следующих типов:</span><span class="sxs-lookup"><span data-stu-id="fbcdf-106">A threat assessment request can be one of the following types:</span></span>

* [<span data-ttu-id="fbcdf-107">Почта</span><span class="sxs-lookup"><span data-stu-id="fbcdf-107">Mail</span></span>](../resources/mailAssessmentRequest.md)
* [<span data-ttu-id="fbcdf-108">Файл электронной почты</span><span class="sxs-lookup"><span data-stu-id="fbcdf-108">Email file</span></span>](../resources/emailFileAssessmentRequest.md)
* [<span data-ttu-id="fbcdf-109">Файл</span><span class="sxs-lookup"><span data-stu-id="fbcdf-109">File</span></span>](../resources/fileAssessmentRequest.md)
* [<span data-ttu-id="fbcdf-110">URL</span><span class="sxs-lookup"><span data-stu-id="fbcdf-110">URL</span></span>](../resources/urlAssessmentRequest.md)

## <a name="permissions"></a><span data-ttu-id="fbcdf-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fbcdf-111">Permissions</span></span>

<span data-ttu-id="fbcdf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fbcdf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fbcdf-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fbcdf-114">Permission type</span></span>                        | <span data-ttu-id="fbcdf-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fbcdf-115">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="fbcdf-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fbcdf-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="fbcdf-117">Среатассессмент. ReadWrite. ALL.</span><span class="sxs-lookup"><span data-stu-id="fbcdf-117">ThreatAssessment.ReadWrite.All.</span></span>             |
| <span data-ttu-id="fbcdf-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fbcdf-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fbcdf-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fbcdf-119">Not supported.</span></span>                              |
| <span data-ttu-id="fbcdf-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fbcdf-120">Application</span></span>                            | <span data-ttu-id="fbcdf-121">Среатассессмент. Read. ALL.</span><span class="sxs-lookup"><span data-stu-id="fbcdf-121">ThreatAssessment.Read.All.</span></span>                  |

## <a name="http-request"></a><span data-ttu-id="fbcdf-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fbcdf-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /informationProtection/threatAssessmentRequests/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fbcdf-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="fbcdf-123">Optional query parameters</span></span>

<span data-ttu-id="fbcdf-124">Этот метод поддерживает следующие параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="fbcdf-124">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="fbcdf-125">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="fbcdf-125">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

|<span data-ttu-id="fbcdf-126">Имя</span><span class="sxs-lookup"><span data-stu-id="fbcdf-126">Name</span></span>            |<span data-ttu-id="fbcdf-127">Значение</span><span class="sxs-lookup"><span data-stu-id="fbcdf-127">Value</span></span>    |<span data-ttu-id="fbcdf-128">Описание</span><span class="sxs-lookup"><span data-stu-id="fbcdf-128">Description</span></span>                                                                                                                                                                 |
|:---------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="fbcdf-129">$expand</span><span class="sxs-lookup"><span data-stu-id="fbcdf-129">$expand</span></span>         |<span data-ttu-id="fbcdf-130">string</span><span class="sxs-lookup"><span data-stu-id="fbcdf-130">string</span></span>   |<span data-ttu-id="fbcdf-131">Использование `$expand=results` в запросе для получения результатов оценки угроз.</span><span class="sxs-lookup"><span data-stu-id="fbcdf-131">Using `$expand=results` in the query to retrieve the threat assessment result.</span></span>                                                                                              |
|<span data-ttu-id="fbcdf-132">$select</span><span class="sxs-lookup"><span data-stu-id="fbcdf-132">$select</span></span>         |<span data-ttu-id="fbcdf-133">string</span><span class="sxs-lookup"><span data-stu-id="fbcdf-133">string</span></span>   |<span data-ttu-id="fbcdf-p103">Список разделенных запятыми свойств, которые необходимо включить в отклик. Для оптимизации производительности выбирайте только необходимые свойства.</span><span class="sxs-lookup"><span data-stu-id="fbcdf-p103">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>                                        |

## <a name="request-headers"></a><span data-ttu-id="fbcdf-136">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fbcdf-136">Request headers</span></span>

| <span data-ttu-id="fbcdf-137">Имя</span><span class="sxs-lookup"><span data-stu-id="fbcdf-137">Name</span></span>      |<span data-ttu-id="fbcdf-138">Описание</span><span class="sxs-lookup"><span data-stu-id="fbcdf-138">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="fbcdf-139">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fbcdf-139">Authorization</span></span> | <span data-ttu-id="fbcdf-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fbcdf-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fbcdf-142">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fbcdf-142">Request body</span></span>

<span data-ttu-id="fbcdf-143">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fbcdf-143">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fbcdf-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="fbcdf-144">Response</span></span>

<span data-ttu-id="fbcdf-145">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [среатассессментрекуест](../resources/threatassessmentrequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fbcdf-145">If successful, this method returns a `200 OK` response code and the requested [threatAssessmentRequest](../resources/threatassessmentrequest.md) object in the response body.</span></span> <span data-ttu-id="fbcdf-146">Возвращаются свойства этого типа: [маилассессментрекуест](../resources/mailAssessmentRequest.md), [емаилфилеассессментрекуест](../resources/emailFileAssessmentRequest.md), [филеассессментрекуест](../resources/fileAssessmentRequest.md), [урлассессментрекуест](../resources/urlAssessmentRequest.md).</span><span class="sxs-lookup"><span data-stu-id="fbcdf-146">The properties of that type are returned: [mailAssessmentRequest](../resources/mailAssessmentRequest.md), [emailFileAssessmentRequest](../resources/emailFileAssessmentRequest.md), [fileAssessmentRequest](../resources/fileAssessmentRequest.md), [urlAssessmentRequest](../resources/urlAssessmentRequest.md).</span></span>

## <a name="examples"></a><span data-ttu-id="fbcdf-147">Примеры</span><span class="sxs-lookup"><span data-stu-id="fbcdf-147">Examples</span></span>

### <a name="example-1-get-the-properties-of-a-mail-assessment-request"></a><span data-ttu-id="fbcdf-148">Пример 1: получение свойств запроса на оценку почты</span><span class="sxs-lookup"><span data-stu-id="fbcdf-148">Example 1: Get the properties of a mail assessment request</span></span>

#### <a name="request"></a><span data-ttu-id="fbcdf-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="fbcdf-149">Request</span></span>

<span data-ttu-id="fbcdf-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fbcdf-150">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="fbcdf-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="fbcdf-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mailassessmentrequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/informationProtection/threatAssessmentRequests/49c5ef5b-1f65-444a-e6b9-08d772ea2059
```
# <a name="c"></a>[<span data-ttu-id="fbcdf-152">C#</span><span class="sxs-lookup"><span data-stu-id="fbcdf-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailassessmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fbcdf-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fbcdf-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailassessmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fbcdf-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fbcdf-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailassessmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="fbcdf-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="fbcdf-155">Response</span></span>

<span data-ttu-id="fbcdf-156">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fbcdf-156">The following is an example of the response.</span></span>

> <span data-ttu-id="fbcdf-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fbcdf-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailAssessmentRequest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#informationProtection/threatAssessmentRequests/$entity",
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
}
```

### <a name="example-2-get-the-properties-of-an-email-file-assessment-request"></a><span data-ttu-id="fbcdf-159">Пример 2: получение свойств запроса на оценку файла электронной почты</span><span class="sxs-lookup"><span data-stu-id="fbcdf-159">Example 2: Get the properties of an email file assessment request</span></span>

#### <a name="request"></a><span data-ttu-id="fbcdf-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="fbcdf-160">Request</span></span>

<span data-ttu-id="fbcdf-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fbcdf-161">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="fbcdf-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="fbcdf-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_emailfileassessmentrequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/informationProtection/threatAssessmentRequests/ab2ad9b3-2213-4091-ae0c-08d76ddbcacf
```
# <a name="c"></a>[<span data-ttu-id="fbcdf-163">C#</span><span class="sxs-lookup"><span data-stu-id="fbcdf-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-emailfileassessmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fbcdf-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fbcdf-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-emailfileassessmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fbcdf-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fbcdf-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-emailfileassessmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="fbcdf-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="fbcdf-166">Response</span></span>

<span data-ttu-id="fbcdf-167">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fbcdf-167">The following is an example of the response.</span></span>

> <span data-ttu-id="fbcdf-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fbcdf-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailFileAssessmentRequest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#informationProtection/threatAssessmentRequests/$entity",
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

### <a name="example-3-get-the-properties-of-a-file-assessment-request"></a><span data-ttu-id="fbcdf-170">Пример 3: получение свойств запроса на оценку файла</span><span class="sxs-lookup"><span data-stu-id="fbcdf-170">Example 3: Get the properties of a file assessment request</span></span>

#### <a name="request"></a><span data-ttu-id="fbcdf-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="fbcdf-171">Request</span></span>

<span data-ttu-id="fbcdf-172">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fbcdf-172">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="fbcdf-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="fbcdf-173">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_fileassessmentrequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/informationProtection/threatAssessmentRequests/18406a56-7209-4720-a250-08d772fccdaa
```
# <a name="c"></a>[<span data-ttu-id="fbcdf-174">C#</span><span class="sxs-lookup"><span data-stu-id="fbcdf-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-fileassessmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fbcdf-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fbcdf-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-fileassessmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fbcdf-176">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fbcdf-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-fileassessmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="fbcdf-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="fbcdf-177">Response</span></span>

<span data-ttu-id="fbcdf-178">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fbcdf-178">The following is an example of the response.</span></span>

> <span data-ttu-id="fbcdf-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fbcdf-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.fileAssessmentRequest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#informationProtection/threatAssessmentRequests/$entity",
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

### <a name="example-4-get-the-properties-of-an-url-assessment-request"></a><span data-ttu-id="fbcdf-181">Пример 4: получение свойств запроса на оценку URL-адреса</span><span class="sxs-lookup"><span data-stu-id="fbcdf-181">Example 4: Get the properties of an url assessment request</span></span>

#### <a name="request"></a><span data-ttu-id="fbcdf-182">Запрос</span><span class="sxs-lookup"><span data-stu-id="fbcdf-182">Request</span></span>

<span data-ttu-id="fbcdf-183">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fbcdf-183">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="fbcdf-184">HTTP</span><span class="sxs-lookup"><span data-stu-id="fbcdf-184">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_urlassessmentrequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/informationProtection/threatAssessmentRequests/723c35be-8b5a-47ae-29c0-08d76ddb7f5b
```
# <a name="c"></a>[<span data-ttu-id="fbcdf-185">C#</span><span class="sxs-lookup"><span data-stu-id="fbcdf-185">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-urlassessmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fbcdf-186">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fbcdf-186">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-urlassessmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fbcdf-187">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fbcdf-187">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-urlassessmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="fbcdf-188">Отклик</span><span class="sxs-lookup"><span data-stu-id="fbcdf-188">Response</span></span>

<span data-ttu-id="fbcdf-189">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fbcdf-189">The following is an example of the response.</span></span>

> <span data-ttu-id="fbcdf-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fbcdf-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.urlAssessmentRequest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#informationProtection/threatAssessmentRequests/$entity",
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

### <a name="example-5-expand-threat-assessment-results-for-a-request"></a><span data-ttu-id="fbcdf-192">Пример 5: развертывание результатов оценки угроз для запроса</span><span class="sxs-lookup"><span data-stu-id="fbcdf-192">Example 5: Expand threat assessment results for a request</span></span>

#### <a name="request"></a><span data-ttu-id="fbcdf-193">Запрос</span><span class="sxs-lookup"><span data-stu-id="fbcdf-193">Request</span></span>

<span data-ttu-id="fbcdf-194">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fbcdf-194">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="fbcdf-195">HTTP</span><span class="sxs-lookup"><span data-stu-id="fbcdf-195">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_threatassessmentrequest_expand_results"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/informationProtection/threatAssessmentRequests/11922306-b25b-4605-ff0d-08d772fcf996?$expand=results
```
# <a name="c"></a>[<span data-ttu-id="fbcdf-196">C#</span><span class="sxs-lookup"><span data-stu-id="fbcdf-196">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-threatassessmentrequest-expand-results-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fbcdf-197">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fbcdf-197">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-threatassessmentrequest-expand-results-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fbcdf-198">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fbcdf-198">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-threatassessmentrequest-expand-results-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="fbcdf-199">Отклик</span><span class="sxs-lookup"><span data-stu-id="fbcdf-199">Response</span></span>

<span data-ttu-id="fbcdf-200">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fbcdf-200">The following is an example of the response.</span></span>

> <span data-ttu-id="fbcdf-p110">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fbcdf-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailAssessmentRequest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#informationProtection/threatAssessmentRequests(results())/$entity",
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
    "results@odata.context": "https://graph.microsoft.com/beta/$metadata#informationProtection/threatAssessmentRequests('11922306-b25b-4605-ff0d-08d772fcf996')/microsoft.graph.mailAssessmentRequest/results",
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
