---
title: Создание объекта threatAssessmentRequest
description: Создайте новый запрос на оценку угроз.
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4bf7996f84ade6668e6ce70720656158320af06a
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48952991"
---
# <a name="create-threatassessmentrequest"></a><span data-ttu-id="afd2d-103">Создание объекта threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="afd2d-103">Create threatAssessmentRequest</span></span>

<span data-ttu-id="afd2d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="afd2d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="afd2d-105">Создайте новый запрос на оценку угроз.</span><span class="sxs-lookup"><span data-stu-id="afd2d-105">Create a new threat assessment request.</span></span>

<span data-ttu-id="afd2d-106">Запрос на оценку угроз может иметь один из следующих типов:</span><span class="sxs-lookup"><span data-stu-id="afd2d-106">A threat assessment request can be one of the following types:</span></span>

* [<span data-ttu-id="afd2d-107">Почта</span><span class="sxs-lookup"><span data-stu-id="afd2d-107">Mail</span></span>](../resources/mailAssessmentRequest.md)
* [<span data-ttu-id="afd2d-108">Файл электронной почты</span><span class="sxs-lookup"><span data-stu-id="afd2d-108">Email file</span></span>](../resources/emailFileAssessmentRequest.md)
* [<span data-ttu-id="afd2d-109">File</span><span class="sxs-lookup"><span data-stu-id="afd2d-109">File</span></span>](../resources/fileAssessmentRequest.md)
* [<span data-ttu-id="afd2d-110">URL-адрес</span><span class="sxs-lookup"><span data-stu-id="afd2d-110">URL</span></span>](../resources/urlAssessmentRequest.md)

## <a name="permissions"></a><span data-ttu-id="afd2d-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="afd2d-111">Permissions</span></span>

<span data-ttu-id="afd2d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="afd2d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="afd2d-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="afd2d-114">Permission type</span></span>                        | <span data-ttu-id="afd2d-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="afd2d-115">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="afd2d-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="afd2d-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="afd2d-117">ThreatAssessment.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="afd2d-117">ThreatAssessment.ReadWrite.All</span></span>              |
| <span data-ttu-id="afd2d-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="afd2d-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="afd2d-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="afd2d-119">Not supported.</span></span>                              |
| <span data-ttu-id="afd2d-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="afd2d-120">Application</span></span>                            | <span data-ttu-id="afd2d-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="afd2d-121">Not supported.</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="afd2d-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="afd2d-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /informationProtection/threatAssessmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="afd2d-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="afd2d-123">Request headers</span></span>

| <span data-ttu-id="afd2d-124">Имя</span><span class="sxs-lookup"><span data-stu-id="afd2d-124">Name</span></span>          | <span data-ttu-id="afd2d-125">Описание</span><span class="sxs-lookup"><span data-stu-id="afd2d-125">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="afd2d-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="afd2d-126">Authorization</span></span> | <span data-ttu-id="afd2d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="afd2d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="afd2d-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="afd2d-129">Request body</span></span>

<span data-ttu-id="afd2d-130">В тексте запроса добавьте представление объекта [среатассессментрекуест](../resources/threatassessmentrequest.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="afd2d-130">In the request body, supply a JSON representation of [threatAssessmentRequest](../resources/threatassessmentrequest.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="afd2d-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="afd2d-131">Response</span></span>

<span data-ttu-id="afd2d-132">В случае успешного выполнения этот метод возвращает `201, Created` код отклика и новый объект [среатассессментрекуест](../resources/threatassessmentrequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="afd2d-132">If successful, this method returns a `201, Created` response code and a new [threatAssessmentRequest](../resources/threatassessmentrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="afd2d-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="afd2d-133">Examples</span></span>

### <a name="example-1-create-a-mail-assessment-request"></a><span data-ttu-id="afd2d-134">Пример 1: Создание запроса на оценку почты</span><span class="sxs-lookup"><span data-stu-id="afd2d-134">Example 1: Create a mail assessment request</span></span>

#### <a name="request"></a><span data-ttu-id="afd2d-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="afd2d-135">Request</span></span>

<span data-ttu-id="afd2d-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="afd2d-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="afd2d-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="afd2d-137">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="afd2d-138">C#</span><span class="sxs-lookup"><span data-stu-id="afd2d-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-mailassessmentrequest-from-informationprotection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="afd2d-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="afd2d-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-mailassessmentrequest-from-informationprotection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="afd2d-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="afd2d-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-mailassessmentrequest-from-informationprotection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="afd2d-141">Java</span><span class="sxs-lookup"><span data-stu-id="afd2d-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-mailassessmentrequest-from-informationprotection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="afd2d-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="afd2d-142">Response</span></span>

<span data-ttu-id="afd2d-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="afd2d-143">The following is an example of the response.</span></span>

> <span data-ttu-id="afd2d-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="afd2d-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-create-an-email-assessment-request"></a><span data-ttu-id="afd2d-146">Пример 2: Создание запроса на оценку электронной почты</span><span class="sxs-lookup"><span data-stu-id="afd2d-146">Example 2: Create an email assessment request</span></span>

#### <a name="request"></a><span data-ttu-id="afd2d-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="afd2d-147">Request</span></span>

<span data-ttu-id="afd2d-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="afd2d-148">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="afd2d-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="afd2d-149">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="afd2d-150">C#</span><span class="sxs-lookup"><span data-stu-id="afd2d-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-emailfileassessmentrequest-from-informationprotection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="afd2d-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="afd2d-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-emailfileassessmentrequest-from-informationprotection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="afd2d-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="afd2d-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-emailfileassessmentrequest-from-informationprotection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="afd2d-153">Java</span><span class="sxs-lookup"><span data-stu-id="afd2d-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-emailfileassessmentrequest-from-informationprotection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="afd2d-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="afd2d-154">Response</span></span>

<span data-ttu-id="afd2d-155">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="afd2d-155">The following is an example of the response.</span></span>

> <span data-ttu-id="afd2d-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="afd2d-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-3-create-a-file-assessment-request"></a><span data-ttu-id="afd2d-158">Пример 3: Создание запроса на оценку файла</span><span class="sxs-lookup"><span data-stu-id="afd2d-158">Example 3: Create a file assessment request</span></span>

#### <a name="request"></a><span data-ttu-id="afd2d-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="afd2d-159">Request</span></span>

<span data-ttu-id="afd2d-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="afd2d-160">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="afd2d-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="afd2d-161">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="afd2d-162">C#</span><span class="sxs-lookup"><span data-stu-id="afd2d-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-fileassessmentrequest-from-informationprotection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="afd2d-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="afd2d-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-fileassessmentrequest-from-informationprotection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="afd2d-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="afd2d-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-fileassessmentrequest-from-informationprotection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="afd2d-165">Java</span><span class="sxs-lookup"><span data-stu-id="afd2d-165">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-fileassessmentrequest-from-informationprotection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="afd2d-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="afd2d-166">Response</span></span>

<span data-ttu-id="afd2d-167">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="afd2d-167">The following is an example of the response.</span></span>

> <span data-ttu-id="afd2d-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="afd2d-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-4-create-an-url-assessment-request"></a><span data-ttu-id="afd2d-170">Пример 4: Создание запроса на оценку URL-адреса</span><span class="sxs-lookup"><span data-stu-id="afd2d-170">Example 4: Create an url assessment request</span></span>

#### <a name="request"></a><span data-ttu-id="afd2d-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="afd2d-171">Request</span></span>

<span data-ttu-id="afd2d-172">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="afd2d-172">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="afd2d-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="afd2d-173">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="afd2d-174">C#</span><span class="sxs-lookup"><span data-stu-id="afd2d-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-urlassessmentrequest-from-informationprotection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="afd2d-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="afd2d-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-urlassessmentrequest-from-informationprotection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="afd2d-176">Objective-C</span><span class="sxs-lookup"><span data-stu-id="afd2d-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-urlassessmentrequest-from-informationprotection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="afd2d-177">Java</span><span class="sxs-lookup"><span data-stu-id="afd2d-177">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-urlassessmentrequest-from-informationprotection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="afd2d-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="afd2d-178">Response</span></span>

<span data-ttu-id="afd2d-179">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="afd2d-179">The following is an example of the response.</span></span>

> <span data-ttu-id="afd2d-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="afd2d-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


