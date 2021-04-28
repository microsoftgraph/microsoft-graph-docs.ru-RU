---
title: Получение объекта threatAssessmentRequest
description: Извлечение свойств и связей указанного объекта threatassessmentrequest.
localization_priority: Normal
author: hafen-ms
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: b21b7d69d241c5d986713b9e905822faf879147a
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053806"
---
# <a name="get-threatassessmentrequest"></a><span data-ttu-id="94f21-103">Получение объекта threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="94f21-103">Get threatAssessmentRequest</span></span>

<span data-ttu-id="94f21-104">Извлечение свойств и связей указанного объекта [threatAssessmentRequest.](../resources/threatassessmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="94f21-104">Retrieve the properties and relationships of a specified [threatAssessmentRequest](../resources/threatassessmentrequest.md) object.</span></span>

<span data-ttu-id="94f21-105">Запрос на оценку угроз может быть одним из следующих типов:</span><span class="sxs-lookup"><span data-stu-id="94f21-105">A threat assessment request can be one of the following types:</span></span>

* [<span data-ttu-id="94f21-106">Почта</span><span class="sxs-lookup"><span data-stu-id="94f21-106">Mail</span></span>](../resources/mailAssessmentRequest.md)
* [<span data-ttu-id="94f21-107">Файл электронной почты</span><span class="sxs-lookup"><span data-stu-id="94f21-107">Email file</span></span>](../resources/emailFileAssessmentRequest.md)
* [<span data-ttu-id="94f21-108">Файл</span><span class="sxs-lookup"><span data-stu-id="94f21-108">File</span></span>](../resources/fileAssessmentRequest.md)
* [<span data-ttu-id="94f21-109">URL-адрес</span><span class="sxs-lookup"><span data-stu-id="94f21-109">URL</span></span>](../resources/urlAssessmentRequest.md)

## <a name="permissions"></a><span data-ttu-id="94f21-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="94f21-110">Permissions</span></span>

<span data-ttu-id="94f21-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94f21-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="94f21-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="94f21-113">Permission type</span></span>                        | <span data-ttu-id="94f21-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="94f21-114">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="94f21-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="94f21-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="94f21-116">ThreatAssessment.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94f21-116">ThreatAssessment.ReadWrite.All</span></span>             |
| <span data-ttu-id="94f21-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="94f21-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94f21-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="94f21-118">Not supported.</span></span>                              |
| <span data-ttu-id="94f21-119">Приложение</span><span class="sxs-lookup"><span data-stu-id="94f21-119">Application</span></span>                            | <span data-ttu-id="94f21-120">ThreatAssessment.Read.All</span><span class="sxs-lookup"><span data-stu-id="94f21-120">ThreatAssessment.Read.All</span></span>                  |

## <a name="http-request"></a><span data-ttu-id="94f21-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="94f21-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /informationProtection/threatAssessmentRequests/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="94f21-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="94f21-122">Optional query parameters</span></span>

<span data-ttu-id="94f21-123">Этот метод поддерживает следующие параметры запроса OData, чтобы помочь настроить ответ.</span><span class="sxs-lookup"><span data-stu-id="94f21-123">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="94f21-124">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="94f21-124">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

|<span data-ttu-id="94f21-125">Имя</span><span class="sxs-lookup"><span data-stu-id="94f21-125">Name</span></span>            |<span data-ttu-id="94f21-126">Значение</span><span class="sxs-lookup"><span data-stu-id="94f21-126">Value</span></span>    |<span data-ttu-id="94f21-127">Описание</span><span class="sxs-lookup"><span data-stu-id="94f21-127">Description</span></span>                                                                                                                                                                 |
|:---------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="94f21-128">$expand</span><span class="sxs-lookup"><span data-stu-id="94f21-128">$expand</span></span>         |<span data-ttu-id="94f21-129">string</span><span class="sxs-lookup"><span data-stu-id="94f21-129">string</span></span>   |<span data-ttu-id="94f21-130">Использование `$expand=results` в запросе для получения результата оценки угрозы.</span><span class="sxs-lookup"><span data-stu-id="94f21-130">Using `$expand=results` in the query to retrieve the threat assessment result.</span></span>                                                                                              |
|<span data-ttu-id="94f21-131">$select</span><span class="sxs-lookup"><span data-stu-id="94f21-131">$select</span></span>         |<span data-ttu-id="94f21-132">string</span><span class="sxs-lookup"><span data-stu-id="94f21-132">string</span></span>   |<span data-ttu-id="94f21-p103">Список разделенных запятыми свойств, которые необходимо включить в отклик. Для оптимизации производительности выбирайте только необходимые свойства.</span><span class="sxs-lookup"><span data-stu-id="94f21-p103">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>                                        |

## <a name="request-headers"></a><span data-ttu-id="94f21-135">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="94f21-135">Request headers</span></span>

| <span data-ttu-id="94f21-136">Имя</span><span class="sxs-lookup"><span data-stu-id="94f21-136">Name</span></span>      |<span data-ttu-id="94f21-137">Описание</span><span class="sxs-lookup"><span data-stu-id="94f21-137">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="94f21-138">Авторизация</span><span class="sxs-lookup"><span data-stu-id="94f21-138">Authorization</span></span> | <span data-ttu-id="94f21-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="94f21-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="94f21-141">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="94f21-141">Request body</span></span>

<span data-ttu-id="94f21-142">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="94f21-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="94f21-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="94f21-143">Response</span></span>

<span data-ttu-id="94f21-144">В случае успешного выполнения этот метод возвращает код ответа и запрашиваемого объекта `200 OK` [threatAssessmentRequest](../resources/threatassessmentrequest.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="94f21-144">If successful, this method returns a `200 OK` response code and the requested [threatAssessmentRequest](../resources/threatassessmentrequest.md) object in the response body.</span></span> <span data-ttu-id="94f21-145">Возвращаются свойства этого типа: [mailAssessmentRequest,](../resources/mailAssessmentRequest.md) [emailFileAssessmentRequest,](../resources/emailFileAssessmentRequest.md) [fileAssessmentRequest](../resources/fileAssessmentRequest.md), [urlAssessmentRequest](../resources/urlAssessmentRequest.md).</span><span class="sxs-lookup"><span data-stu-id="94f21-145">The properties of that type are returned: [mailAssessmentRequest](../resources/mailAssessmentRequest.md), [emailFileAssessmentRequest](../resources/emailFileAssessmentRequest.md), [fileAssessmentRequest](../resources/fileAssessmentRequest.md), [urlAssessmentRequest](../resources/urlAssessmentRequest.md).</span></span>

## <a name="examples"></a><span data-ttu-id="94f21-146">Примеры</span><span class="sxs-lookup"><span data-stu-id="94f21-146">Examples</span></span>

### <a name="example-1-get-the-properties-of-a-mail-assessment-request"></a><span data-ttu-id="94f21-147">Пример 1. Получить свойства запроса на оценку почты</span><span class="sxs-lookup"><span data-stu-id="94f21-147">Example 1: Get the properties of a mail assessment request</span></span>

#### <a name="request"></a><span data-ttu-id="94f21-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="94f21-148">Request</span></span>

<span data-ttu-id="94f21-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="94f21-149">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="94f21-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="94f21-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mailassessmentrequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/informationProtection/threatAssessmentRequests/49c5ef5b-1f65-444a-e6b9-08d772ea2059
```
# <a name="c"></a>[<span data-ttu-id="94f21-151">C#</span><span class="sxs-lookup"><span data-stu-id="94f21-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailassessmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="94f21-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="94f21-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailassessmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="94f21-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="94f21-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailassessmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="94f21-154">Java</span><span class="sxs-lookup"><span data-stu-id="94f21-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-mailassessmentrequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="94f21-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="94f21-155">Response</span></span>

<span data-ttu-id="94f21-156">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="94f21-156">The following is an example of the response.</span></span>

> <span data-ttu-id="94f21-157">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="94f21-157">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-get-the-properties-of-an-email-file-assessment-request"></a><span data-ttu-id="94f21-158">Пример 2. Получить свойства запроса на оценку файлов электронной почты</span><span class="sxs-lookup"><span data-stu-id="94f21-158">Example 2: Get the properties of an email file assessment request</span></span>

#### <a name="request"></a><span data-ttu-id="94f21-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="94f21-159">Request</span></span>

<span data-ttu-id="94f21-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="94f21-160">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="94f21-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="94f21-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_emailfileassessmentrequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/informationProtection/threatAssessmentRequests/ab2ad9b3-2213-4091-ae0c-08d76ddbcacf
```
# <a name="c"></a>[<span data-ttu-id="94f21-162">C#</span><span class="sxs-lookup"><span data-stu-id="94f21-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-emailfileassessmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="94f21-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="94f21-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-emailfileassessmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="94f21-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="94f21-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-emailfileassessmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="94f21-165">Java</span><span class="sxs-lookup"><span data-stu-id="94f21-165">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-emailfileassessmentrequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="94f21-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="94f21-166">Response</span></span>

<span data-ttu-id="94f21-167">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="94f21-167">The following is an example of the response.</span></span>

> <span data-ttu-id="94f21-168">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="94f21-168">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-3-get-the-properties-of-a-file-assessment-request"></a><span data-ttu-id="94f21-169">Пример 3. Получить свойства запроса на оценку файлов</span><span class="sxs-lookup"><span data-stu-id="94f21-169">Example 3: Get the properties of a file assessment request</span></span>

#### <a name="request"></a><span data-ttu-id="94f21-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="94f21-170">Request</span></span>

<span data-ttu-id="94f21-171">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="94f21-171">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="94f21-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="94f21-172">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_fileassessmentrequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/informationProtection/threatAssessmentRequests/18406a56-7209-4720-a250-08d772fccdaa
```
# <a name="c"></a>[<span data-ttu-id="94f21-173">C#</span><span class="sxs-lookup"><span data-stu-id="94f21-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-fileassessmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="94f21-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="94f21-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-fileassessmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="94f21-175">Objective-C</span><span class="sxs-lookup"><span data-stu-id="94f21-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-fileassessmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="94f21-176">Java</span><span class="sxs-lookup"><span data-stu-id="94f21-176">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-fileassessmentrequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="94f21-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="94f21-177">Response</span></span>

<span data-ttu-id="94f21-178">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="94f21-178">The following is an example of the response.</span></span>

> <span data-ttu-id="94f21-179">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="94f21-179">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-4-get-the-properties-of-an-url-assessment-request"></a><span data-ttu-id="94f21-180">Пример 4. Получить свойства запроса на оценку URL-адреса</span><span class="sxs-lookup"><span data-stu-id="94f21-180">Example 4: Get the properties of an url assessment request</span></span>

#### <a name="request"></a><span data-ttu-id="94f21-181">Запрос</span><span class="sxs-lookup"><span data-stu-id="94f21-181">Request</span></span>

<span data-ttu-id="94f21-182">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="94f21-182">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="94f21-183">HTTP</span><span class="sxs-lookup"><span data-stu-id="94f21-183">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_urlassessmentrequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/informationProtection/threatAssessmentRequests/723c35be-8b5a-47ae-29c0-08d76ddb7f5b
```
# <a name="c"></a>[<span data-ttu-id="94f21-184">C#</span><span class="sxs-lookup"><span data-stu-id="94f21-184">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-urlassessmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="94f21-185">JavaScript</span><span class="sxs-lookup"><span data-stu-id="94f21-185">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-urlassessmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="94f21-186">Objective-C</span><span class="sxs-lookup"><span data-stu-id="94f21-186">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-urlassessmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="94f21-187">Java</span><span class="sxs-lookup"><span data-stu-id="94f21-187">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-urlassessmentrequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="94f21-188">Отклик</span><span class="sxs-lookup"><span data-stu-id="94f21-188">Response</span></span>

<span data-ttu-id="94f21-189">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="94f21-189">The following is an example of the response.</span></span>

> <span data-ttu-id="94f21-190">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="94f21-190">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-5-expand-threat-assessment-results-for-a-request"></a><span data-ttu-id="94f21-191">Пример 5. Расширение результатов оценки угроз для запроса</span><span class="sxs-lookup"><span data-stu-id="94f21-191">Example 5: Expand threat assessment results for a request</span></span>

#### <a name="request"></a><span data-ttu-id="94f21-192">Запрос</span><span class="sxs-lookup"><span data-stu-id="94f21-192">Request</span></span>

<span data-ttu-id="94f21-193">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="94f21-193">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="94f21-194">HTTP</span><span class="sxs-lookup"><span data-stu-id="94f21-194">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_threatassessmentrequest_expand_results"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/informationProtection/threatAssessmentRequests/11922306-b25b-4605-ff0d-08d772fcf996?$expand=results
```
# <a name="c"></a>[<span data-ttu-id="94f21-195">C#</span><span class="sxs-lookup"><span data-stu-id="94f21-195">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-threatassessmentrequest-expand-results-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="94f21-196">JavaScript</span><span class="sxs-lookup"><span data-stu-id="94f21-196">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-threatassessmentrequest-expand-results-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="94f21-197">Objective-C</span><span class="sxs-lookup"><span data-stu-id="94f21-197">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-threatassessmentrequest-expand-results-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="94f21-198">Java</span><span class="sxs-lookup"><span data-stu-id="94f21-198">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-threatassessmentrequest-expand-results-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="94f21-199">Отклик</span><span class="sxs-lookup"><span data-stu-id="94f21-199">Response</span></span>

<span data-ttu-id="94f21-200">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="94f21-200">The following is an example of the response.</span></span>

> <span data-ttu-id="94f21-201">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="94f21-201">**Note:** The response object shown here might be shortened for readability.</span></span>

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

