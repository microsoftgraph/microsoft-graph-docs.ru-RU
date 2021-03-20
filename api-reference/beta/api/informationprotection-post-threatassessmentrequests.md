---
title: Создание объекта threatAssessmentRequest
description: Создайте новый запрос на оценку угрозы.
localization_priority: Normal
author: hafen-ms
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: fd45facf81797a8b5f11024a7df9285db6ab227d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50944131"
---
# <a name="create-threatassessmentrequest"></a><span data-ttu-id="226fa-103">Создание объекта threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="226fa-103">Create threatAssessmentRequest</span></span>

<span data-ttu-id="226fa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="226fa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="226fa-105">Создайте новый запрос на оценку угрозы.</span><span class="sxs-lookup"><span data-stu-id="226fa-105">Create a new threat assessment request.</span></span>

<span data-ttu-id="226fa-106">Запрос на оценку угроз может быть одним из следующих типов:</span><span class="sxs-lookup"><span data-stu-id="226fa-106">A threat assessment request can be one of the following types:</span></span>

* [<span data-ttu-id="226fa-107">Почта</span><span class="sxs-lookup"><span data-stu-id="226fa-107">Mail</span></span>](../resources/mailAssessmentRequest.md)
* [<span data-ttu-id="226fa-108">Файл электронной почты</span><span class="sxs-lookup"><span data-stu-id="226fa-108">Email file</span></span>](../resources/emailFileAssessmentRequest.md)
* [<span data-ttu-id="226fa-109">File</span><span class="sxs-lookup"><span data-stu-id="226fa-109">File</span></span>](../resources/fileAssessmentRequest.md)
* [<span data-ttu-id="226fa-110">URL-адрес</span><span class="sxs-lookup"><span data-stu-id="226fa-110">URL</span></span>](../resources/urlAssessmentRequest.md)

## <a name="permissions"></a><span data-ttu-id="226fa-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="226fa-111">Permissions</span></span>

<span data-ttu-id="226fa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="226fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="226fa-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="226fa-114">Permission type</span></span>                        | <span data-ttu-id="226fa-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="226fa-115">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="226fa-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="226fa-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="226fa-117">ThreatAssessment.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="226fa-117">ThreatAssessment.ReadWrite.All</span></span>              |
| <span data-ttu-id="226fa-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="226fa-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="226fa-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="226fa-119">Not supported.</span></span>                              |
| <span data-ttu-id="226fa-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="226fa-120">Application</span></span>                            | <span data-ttu-id="226fa-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="226fa-121">Not supported.</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="226fa-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="226fa-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /informationProtection/threatAssessmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="226fa-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="226fa-123">Request headers</span></span>

| <span data-ttu-id="226fa-124">Имя</span><span class="sxs-lookup"><span data-stu-id="226fa-124">Name</span></span>          | <span data-ttu-id="226fa-125">Описание</span><span class="sxs-lookup"><span data-stu-id="226fa-125">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="226fa-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="226fa-126">Authorization</span></span> | <span data-ttu-id="226fa-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="226fa-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="226fa-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="226fa-129">Request body</span></span>

<span data-ttu-id="226fa-130">В теле запроса поставляем JSON представление [объекта threatAssessmentRequest.](../resources/threatassessmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="226fa-130">In the request body, supply a JSON representation of [threatAssessmentRequest](../resources/threatassessmentrequest.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="226fa-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="226fa-131">Response</span></span>

<span data-ttu-id="226fa-132">В случае успешного выполнения этот метод возвращает код ответа и новый объект `201, Created` [threatAssessmentRequest](../resources/threatassessmentrequest.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="226fa-132">If successful, this method returns a `201, Created` response code and a new [threatAssessmentRequest](../resources/threatassessmentrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="226fa-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="226fa-133">Examples</span></span>

### <a name="example-1-create-a-mail-assessment-request"></a><span data-ttu-id="226fa-134">Пример 1. Создание запроса на оценку почты</span><span class="sxs-lookup"><span data-stu-id="226fa-134">Example 1: Create a mail assessment request</span></span>

#### <a name="request"></a><span data-ttu-id="226fa-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="226fa-135">Request</span></span>

<span data-ttu-id="226fa-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="226fa-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="226fa-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="226fa-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_mailassessmentrequest_from_informationprotection"
}-->

```http
POST https://graph.microsoft.com/beta/informationProtection/threatAssessmentRequests
Content-type: application/json

{
  "@odata.type": "#microsoft.graph.mailAssessmentRequest",
  "recipientEmail": "tifc@a830edad9050849EQTPWBJZXODQ.onmicrosoft.com",
  "expectedAssessment": "block",
  "category": "spam",
  "messageUri": "https://graph.microsoft.com/beta/users/c52ce8db-3e4b-4181-93c4-7d6b6bffaf60/messages/AAMkADU3MWUxOTU0LWNlOTEt="
}
```
# <a name="c"></a>[<span data-ttu-id="226fa-138">C#</span><span class="sxs-lookup"><span data-stu-id="226fa-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-mailassessmentrequest-from-informationprotection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="226fa-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="226fa-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-mailassessmentrequest-from-informationprotection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="226fa-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="226fa-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-mailassessmentrequest-from-informationprotection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="226fa-141">Java</span><span class="sxs-lookup"><span data-stu-id="226fa-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-mailassessmentrequest-from-informationprotection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="226fa-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="226fa-142">Response</span></span>

<span data-ttu-id="226fa-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="226fa-143">The following is an example of the response.</span></span>

> <span data-ttu-id="226fa-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="226fa-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailAssessmentRequest"
} -->

```http
HTTP/1.1 201 Created
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

### <a name="example-2-create-an-email-assessment-request"></a><span data-ttu-id="226fa-146">Пример 2. Создание запроса на оценку электронной почты</span><span class="sxs-lookup"><span data-stu-id="226fa-146">Example 2: Create an email assessment request</span></span>

#### <a name="request"></a><span data-ttu-id="226fa-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="226fa-147">Request</span></span>

<span data-ttu-id="226fa-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="226fa-148">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="226fa-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="226fa-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_emailfileassessmentrequest_from_informationprotection"
}-->

```http
POST https://graph.microsoft.com/beta/informationProtection/threatAssessmentRequests
Content-type: application/json

{
  "@odata.type": "#microsoft.graph.emailFileAssessmentRequest",
  "recipientEmail": "tifc@a830edad9050849EQTPWBJZXODQ.onmicrosoft.com",
  "expectedAssessment": "block",
  "category": "malware",
  "contentData": "UmVjZWl2ZWQ6IGZyb20gTVcyUFIwME1CMDMxNC5uYW1wcmQwMC....."
}
```
# <a name="c"></a>[<span data-ttu-id="226fa-150">C#</span><span class="sxs-lookup"><span data-stu-id="226fa-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-emailfileassessmentrequest-from-informationprotection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="226fa-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="226fa-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-emailfileassessmentrequest-from-informationprotection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="226fa-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="226fa-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-emailfileassessmentrequest-from-informationprotection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="226fa-153">Java</span><span class="sxs-lookup"><span data-stu-id="226fa-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-emailfileassessmentrequest-from-informationprotection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="226fa-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="226fa-154">Response</span></span>

<span data-ttu-id="226fa-155">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="226fa-155">The following is an example of the response.</span></span>

> <span data-ttu-id="226fa-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="226fa-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailFileAssessmentRequest"
} -->

```http
HTTP/1.1 201 Created
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

### <a name="example-3-create-a-file-assessment-request"></a><span data-ttu-id="226fa-158">Пример 3. Создание запроса на оценку файлов</span><span class="sxs-lookup"><span data-stu-id="226fa-158">Example 3: Create a file assessment request</span></span>

#### <a name="request"></a><span data-ttu-id="226fa-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="226fa-159">Request</span></span>

<span data-ttu-id="226fa-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="226fa-160">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="226fa-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="226fa-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_fileassessmentrequest_from_informationprotection"
}-->

```http
POST https://graph.microsoft.com/beta/informationProtection/threatAssessmentRequests
Content-type: application/json

{
  "@odata.type": "#microsoft.graph.fileAssessmentRequest",
  "expectedAssessment": "block",
  "category": "malware",
  "fileName": "test.txt",
  "contentData": "VGhpcyBpcyBhIHRlc3QgZmlsZQ=="
}
```
# <a name="c"></a>[<span data-ttu-id="226fa-162">C#</span><span class="sxs-lookup"><span data-stu-id="226fa-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-fileassessmentrequest-from-informationprotection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="226fa-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="226fa-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-fileassessmentrequest-from-informationprotection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="226fa-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="226fa-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-fileassessmentrequest-from-informationprotection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="226fa-165">Java</span><span class="sxs-lookup"><span data-stu-id="226fa-165">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-fileassessmentrequest-from-informationprotection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="226fa-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="226fa-166">Response</span></span>

<span data-ttu-id="226fa-167">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="226fa-167">The following is an example of the response.</span></span>

> <span data-ttu-id="226fa-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="226fa-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.fileAssessmentRequest"
} -->

```http
HTTP/1.1 201 Created
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

### <a name="example-4-create-an-url-assessment-request"></a><span data-ttu-id="226fa-170">Пример 4. Создание запроса на оценку URL-адреса</span><span class="sxs-lookup"><span data-stu-id="226fa-170">Example 4: Create an url assessment request</span></span>

#### <a name="request"></a><span data-ttu-id="226fa-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="226fa-171">Request</span></span>

<span data-ttu-id="226fa-172">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="226fa-172">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="226fa-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="226fa-173">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_urlassessmentrequest_from_informationprotection"
}-->

```http
POST https://graph.microsoft.com/beta/informationProtection/threatAssessmentRequests
Content-type: application/json

{
  "@odata.type": "#microsoft.graph.urlAssessmentRequest",
  "url": "http://test.com",
  "expectedAssessment": "block",
  "category": "phishing"
}
```
# <a name="c"></a>[<span data-ttu-id="226fa-174">C#</span><span class="sxs-lookup"><span data-stu-id="226fa-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-urlassessmentrequest-from-informationprotection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="226fa-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="226fa-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-urlassessmentrequest-from-informationprotection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="226fa-176">Objective-C</span><span class="sxs-lookup"><span data-stu-id="226fa-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-urlassessmentrequest-from-informationprotection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="226fa-177">Java</span><span class="sxs-lookup"><span data-stu-id="226fa-177">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-urlassessmentrequest-from-informationprotection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="226fa-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="226fa-178">Response</span></span>

<span data-ttu-id="226fa-179">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="226fa-179">The following is an example of the response.</span></span>

> <span data-ttu-id="226fa-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="226fa-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.urlAssessmentRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#informationProtection/threatAssessmentRequests/$entity",
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


