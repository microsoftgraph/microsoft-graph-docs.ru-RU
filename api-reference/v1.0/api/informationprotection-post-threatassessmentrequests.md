---
title: Создание объекта threatAssessmentRequest
description: Создайте новый запрос на оценку угроз.
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ec60e8c0f23fe882a719114dee6f720a8c4419eb
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48059693"
---
# <a name="create-threatassessmentrequest"></a><span data-ttu-id="e9200-103">Создание объекта threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="e9200-103">Create threatAssessmentRequest</span></span>

<span data-ttu-id="e9200-104">Создайте новый запрос на оценку угроз.</span><span class="sxs-lookup"><span data-stu-id="e9200-104">Create a new threat assessment request.</span></span>

<span data-ttu-id="e9200-105">Запрос на оценку угроз может иметь один из следующих типов:</span><span class="sxs-lookup"><span data-stu-id="e9200-105">A threat assessment request can be one of the following types:</span></span>

* [<span data-ttu-id="e9200-106">Почта</span><span class="sxs-lookup"><span data-stu-id="e9200-106">Mail</span></span>](../resources/mailAssessmentRequest.md)
* [<span data-ttu-id="e9200-107">Файл электронной почты</span><span class="sxs-lookup"><span data-stu-id="e9200-107">Email file</span></span>](../resources/emailFileAssessmentRequest.md)
* [<span data-ttu-id="e9200-108">File</span><span class="sxs-lookup"><span data-stu-id="e9200-108">File</span></span>](../resources/fileAssessmentRequest.md)
* [<span data-ttu-id="e9200-109">URL-адрес</span><span class="sxs-lookup"><span data-stu-id="e9200-109">URL</span></span>](../resources/urlAssessmentRequest.md)

## <a name="permissions"></a><span data-ttu-id="e9200-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e9200-110">Permissions</span></span>

<span data-ttu-id="e9200-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e9200-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e9200-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e9200-113">Permission type</span></span>                        | <span data-ttu-id="e9200-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e9200-114">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e9200-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e9200-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="e9200-116">Среатассессмент. ReadWrite. ALL.</span><span class="sxs-lookup"><span data-stu-id="e9200-116">ThreatAssessment.ReadWrite.All.</span></span>             |
| <span data-ttu-id="e9200-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e9200-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e9200-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e9200-118">Not supported.</span></span>                              |
| <span data-ttu-id="e9200-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e9200-119">Application</span></span>                            | <span data-ttu-id="e9200-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e9200-120">Not supported.</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="e9200-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e9200-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /informationProtection/threatAssessmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="e9200-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e9200-122">Request headers</span></span>

| <span data-ttu-id="e9200-123">Имя</span><span class="sxs-lookup"><span data-stu-id="e9200-123">Name</span></span>          | <span data-ttu-id="e9200-124">Описание</span><span class="sxs-lookup"><span data-stu-id="e9200-124">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="e9200-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e9200-125">Authorization</span></span> | <span data-ttu-id="e9200-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e9200-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e9200-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e9200-128">Request body</span></span>

<span data-ttu-id="e9200-129">В тексте запроса добавьте представление объекта [среатассессментрекуест](../resources/threatassessmentrequest.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e9200-129">In the request body, supply a JSON representation of a [threatAssessmentRequest](../resources/threatassessmentrequest.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e9200-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="e9200-130">Response</span></span>

<span data-ttu-id="e9200-131">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и новый объект [среатассессментрекуест](../resources/threatassessmentrequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e9200-131">If successful, this method returns a `201 Created` response code and a new [threatAssessmentRequest](../resources/threatassessmentrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e9200-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="e9200-132">Examples</span></span>

### <a name="example-1-create-a-mail-assessment-request"></a><span data-ttu-id="e9200-133">Пример 1: Создание запроса на оценку почты</span><span class="sxs-lookup"><span data-stu-id="e9200-133">Example 1: Create a mail assessment request</span></span>

#### <a name="request"></a><span data-ttu-id="e9200-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="e9200-134">Request</span></span>

<span data-ttu-id="e9200-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e9200-135">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e9200-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="e9200-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_mailassessmentrequest_from_informationprotection"
}-->

```http
POST https://graph.microsoft.com/v1.0/informationProtection/threatAssessmentRequests
Content-type: application/json

{
  "@odata.type": "#microsoft.graph.mailAssessmentRequest",
  "recipientEmail": "tifc@a830edad9050849EQTPWBJZXODQ.onmicrosoft.com",
  "expectedAssessment": "block",
  "category": "spam",
  "messageUri": "https://graph.microsoft.com/v1.0/users/c52ce8db-3e4b-4181-93c4-7d6b6bffaf60/messages/AAMkADU3MWUxOTU0LWNlOTEt="
}
```
# <a name="c"></a>[<span data-ttu-id="e9200-137">C#</span><span class="sxs-lookup"><span data-stu-id="e9200-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-mailassessmentrequest-from-informationprotection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e9200-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e9200-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-mailassessmentrequest-from-informationprotection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e9200-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e9200-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-mailassessmentrequest-from-informationprotection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e9200-140">Java</span><span class="sxs-lookup"><span data-stu-id="e9200-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-mailassessmentrequest-from-informationprotection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e9200-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="e9200-141">Response</span></span>

<span data-ttu-id="e9200-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e9200-142">The following is an example of the response.</span></span>

> <span data-ttu-id="e9200-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e9200-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailAssessmentRequest"
} -->

```http
HTTP/1.1 201 Created
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

### <a name="example-2-create-an-email-assessment-request"></a><span data-ttu-id="e9200-145">Пример 2: Создание запроса на оценку электронной почты</span><span class="sxs-lookup"><span data-stu-id="e9200-145">Example 2: Create an email assessment request</span></span>

#### <a name="request"></a><span data-ttu-id="e9200-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="e9200-146">Request</span></span>

<span data-ttu-id="e9200-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e9200-147">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e9200-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="e9200-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_emailfileassessmentrequest_from_informationprotection"
}-->

```http
POST https://graph.microsoft.com/v1.0/informationProtection/threatAssessmentRequests
Content-type: application/json

{
  "@odata.type": "#microsoft.graph.emailFileAssessmentRequest",
  "recipientEmail": "tifc@a830edad9050849EQTPWBJZXODQ.onmicrosoft.com",
  "expectedAssessment": "block",
  "category": "malware",
  "contentData": "UmVjZWl2ZWQ6IGZyb20gTVcyUFIwME1CMDMxNC5uYW1wcmQwMC....."
}
```
# <a name="c"></a>[<span data-ttu-id="e9200-149">C#</span><span class="sxs-lookup"><span data-stu-id="e9200-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-emailfileassessmentrequest-from-informationprotection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e9200-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e9200-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-emailfileassessmentrequest-from-informationprotection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e9200-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e9200-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-emailfileassessmentrequest-from-informationprotection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e9200-152">Java</span><span class="sxs-lookup"><span data-stu-id="e9200-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-emailfileassessmentrequest-from-informationprotection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e9200-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="e9200-153">Response</span></span>

<span data-ttu-id="e9200-154">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e9200-154">The following is an example of the response.</span></span>

> <span data-ttu-id="e9200-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e9200-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailFileAssessmentRequest"
} -->

```http
HTTP/1.1 201 Created
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

### <a name="example-3-create-a-file-assessment-request"></a><span data-ttu-id="e9200-157">Пример 3: Создание запроса на оценку файла</span><span class="sxs-lookup"><span data-stu-id="e9200-157">Example 3: Create a file assessment request</span></span>

#### <a name="request"></a><span data-ttu-id="e9200-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="e9200-158">Request</span></span>

<span data-ttu-id="e9200-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e9200-159">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e9200-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="e9200-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_fileassessmentrequest_from_informationprotection"
}-->

```http
POST https://graph.microsoft.com/v1.0/informationProtection/threatAssessmentRequests
Content-type: application/json

{
  "@odata.type": "#microsoft.graph.fileAssessmentRequest",
  "expectedAssessment": "block",
  "category": "malware",
  "fileName": "test.txt",
  "contentData": "VGhpcyBpcyBhIHRlc3QgZmlsZQ=="
}
```
# <a name="c"></a>[<span data-ttu-id="e9200-161">C#</span><span class="sxs-lookup"><span data-stu-id="e9200-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-fileassessmentrequest-from-informationprotection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e9200-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e9200-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-fileassessmentrequest-from-informationprotection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e9200-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e9200-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-fileassessmentrequest-from-informationprotection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e9200-164">Java</span><span class="sxs-lookup"><span data-stu-id="e9200-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-fileassessmentrequest-from-informationprotection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e9200-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="e9200-165">Response</span></span>

<span data-ttu-id="e9200-166">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e9200-166">The following is an example of the response.</span></span>

> <span data-ttu-id="e9200-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e9200-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.fileAssessmentRequest"
} -->

```http
HTTP/1.1 201 Created
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

### <a name="example-4-create-an-url-assessment-request"></a><span data-ttu-id="e9200-169">Пример 4: Создание запроса на оценку URL-адреса</span><span class="sxs-lookup"><span data-stu-id="e9200-169">Example 4: Create an url assessment request</span></span>

#### <a name="request"></a><span data-ttu-id="e9200-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="e9200-170">Request</span></span>

<span data-ttu-id="e9200-171">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e9200-171">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e9200-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="e9200-172">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_urlassessmentrequest_from_informationprotection"
}-->

```http
POST https://graph.microsoft.com/v1.0/informationProtection/threatAssessmentRequests
Content-type: application/json

{
  "@odata.type": "#microsoft.graph.urlAssessmentRequest",
  "url": "http://test.com",
  "expectedAssessment": "block",
  "category": "phishing"
}
```
# <a name="c"></a>[<span data-ttu-id="e9200-173">C#</span><span class="sxs-lookup"><span data-stu-id="e9200-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-urlassessmentrequest-from-informationprotection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e9200-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e9200-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-urlassessmentrequest-from-informationprotection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e9200-175">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e9200-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-urlassessmentrequest-from-informationprotection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e9200-176">Java</span><span class="sxs-lookup"><span data-stu-id="e9200-176">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-urlassessmentrequest-from-informationprotection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e9200-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="e9200-177">Response</span></span>

<span data-ttu-id="e9200-178">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e9200-178">The following is an example of the response.</span></span>

> <span data-ttu-id="e9200-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e9200-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.urlAssessmentRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#informationProtection/threatAssessmentRequests/$entity",
  "@odata.type": "#microsoft.graph.urlAssessmentRequest",
  "id": "8d87d2b2-ca4d-422c-f8df-08d774a5c9ac",
  "createdDateTime": "2019-11-29T08:26:09.8196703Z",
  "contentType": "url",
  "expectedAssessment": "block",
  "category": "phishing",
  "status": "pending",
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

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create threatAssessmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

