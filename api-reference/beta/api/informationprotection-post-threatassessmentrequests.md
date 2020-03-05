---
title: Создание объекта threatAssessmentRequest
description: Создайте новый запрос на оценку угроз.
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0818b495c209fcd264d1ddcc2a8c9f146f2983c7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446396"
---
# <a name="create-threatassessmentrequest"></a><span data-ttu-id="82f99-103">Создание объекта threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="82f99-103">Create threatAssessmentRequest</span></span>

<span data-ttu-id="82f99-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="82f99-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="82f99-105">Создайте новый запрос на оценку угроз.</span><span class="sxs-lookup"><span data-stu-id="82f99-105">Create a new threat assessment request.</span></span>

<span data-ttu-id="82f99-106">Запрос на оценку угроз может иметь один из следующих типов:</span><span class="sxs-lookup"><span data-stu-id="82f99-106">A threat assessment request can be one of the following types:</span></span>

* <span data-ttu-id="82f99-107">[почта](../resources/mailAssessmentRequest.md);</span><span class="sxs-lookup"><span data-stu-id="82f99-107">[Mail](../resources/mailAssessmentRequest.md)</span></span>
* [<span data-ttu-id="82f99-108">Файл электронной почты</span><span class="sxs-lookup"><span data-stu-id="82f99-108">Email file</span></span>](../resources/emailFileAssessmentRequest.md)
* [<span data-ttu-id="82f99-109">Файл</span><span class="sxs-lookup"><span data-stu-id="82f99-109">File</span></span>](../resources/fileAssessmentRequest.md)
* [<span data-ttu-id="82f99-110">URL</span><span class="sxs-lookup"><span data-stu-id="82f99-110">URL</span></span>](../resources/urlAssessmentRequest.md)

## <a name="permissions"></a><span data-ttu-id="82f99-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="82f99-111">Permissions</span></span>

<span data-ttu-id="82f99-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="82f99-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="82f99-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="82f99-114">Permission type</span></span>                        | <span data-ttu-id="82f99-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="82f99-115">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="82f99-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="82f99-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="82f99-117">Среатассессмент. ReadWrite. ALL.</span><span class="sxs-lookup"><span data-stu-id="82f99-117">ThreatAssessment.ReadWrite.All.</span></span>             |
| <span data-ttu-id="82f99-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="82f99-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="82f99-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82f99-119">Not supported.</span></span>                              |
| <span data-ttu-id="82f99-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="82f99-120">Application</span></span>                            | <span data-ttu-id="82f99-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82f99-121">Not supported.</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="82f99-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="82f99-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /informationProtection/threatAssessmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="82f99-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="82f99-123">Request headers</span></span>

| <span data-ttu-id="82f99-124">Имя</span><span class="sxs-lookup"><span data-stu-id="82f99-124">Name</span></span>          | <span data-ttu-id="82f99-125">Описание</span><span class="sxs-lookup"><span data-stu-id="82f99-125">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="82f99-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="82f99-126">Authorization</span></span> | <span data-ttu-id="82f99-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="82f99-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="82f99-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="82f99-129">Request body</span></span>

<span data-ttu-id="82f99-130">В тексте запроса добавьте представление объекта [среатассессментрекуест](../resources/threatassessmentrequest.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="82f99-130">In the request body, supply a JSON representation of [threatAssessmentRequest](../resources/threatassessmentrequest.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="82f99-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="82f99-131">Response</span></span>

<span data-ttu-id="82f99-132">В случае успешного выполнения этот метод возвращает `201, Created` код отклика и новый объект [среатассессментрекуест](../resources/threatassessmentrequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="82f99-132">If successful, this method returns a `201, Created` response code and a new [threatAssessmentRequest](../resources/threatassessmentrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="82f99-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="82f99-133">Examples</span></span>

### <a name="example-1-create-a-mail-assessment-request"></a><span data-ttu-id="82f99-134">Пример 1: Создание запроса на оценку почты</span><span class="sxs-lookup"><span data-stu-id="82f99-134">Example 1: Create a mail assessment request</span></span>

#### <a name="request"></a><span data-ttu-id="82f99-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="82f99-135">Request</span></span>

<span data-ttu-id="82f99-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="82f99-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="82f99-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="82f99-137">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="82f99-138">C#</span><span class="sxs-lookup"><span data-stu-id="82f99-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-mailassessmentrequest-from-informationprotection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="82f99-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="82f99-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-mailassessmentrequest-from-informationprotection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="82f99-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="82f99-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-mailassessmentrequest-from-informationprotection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="82f99-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="82f99-141">Response</span></span>

<span data-ttu-id="82f99-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="82f99-142">The following is an example of the response.</span></span>

> <span data-ttu-id="82f99-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="82f99-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-create-an-email-assessment-request"></a><span data-ttu-id="82f99-145">Пример 2: Создание запроса на оценку электронной почты</span><span class="sxs-lookup"><span data-stu-id="82f99-145">Example 2: Create an email assessment request</span></span>

#### <a name="request"></a><span data-ttu-id="82f99-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="82f99-146">Request</span></span>

<span data-ttu-id="82f99-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="82f99-147">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="82f99-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="82f99-148">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="82f99-149">C#</span><span class="sxs-lookup"><span data-stu-id="82f99-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-emailfileassessmentrequest-from-informationprotection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="82f99-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="82f99-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-emailfileassessmentrequest-from-informationprotection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="82f99-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="82f99-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-emailfileassessmentrequest-from-informationprotection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="82f99-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="82f99-152">Response</span></span>

<span data-ttu-id="82f99-153">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="82f99-153">The following is an example of the response.</span></span>

> <span data-ttu-id="82f99-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="82f99-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-3-create-a-file-assessment-request"></a><span data-ttu-id="82f99-156">Пример 3: Создание запроса на оценку файла</span><span class="sxs-lookup"><span data-stu-id="82f99-156">Example 3: Create a file assessment request</span></span>

#### <a name="request"></a><span data-ttu-id="82f99-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="82f99-157">Request</span></span>

<span data-ttu-id="82f99-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="82f99-158">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="82f99-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="82f99-159">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="82f99-160">C#</span><span class="sxs-lookup"><span data-stu-id="82f99-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-fileassessmentrequest-from-informationprotection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="82f99-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="82f99-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-fileassessmentrequest-from-informationprotection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="82f99-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="82f99-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-fileassessmentrequest-from-informationprotection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="82f99-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="82f99-163">Response</span></span>

<span data-ttu-id="82f99-164">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="82f99-164">The following is an example of the response.</span></span>

> <span data-ttu-id="82f99-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="82f99-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-4-create-an-url-assessment-request"></a><span data-ttu-id="82f99-167">Пример 4: Создание запроса на оценку URL-адреса</span><span class="sxs-lookup"><span data-stu-id="82f99-167">Example 4: Create an url assessment request</span></span>

#### <a name="request"></a><span data-ttu-id="82f99-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="82f99-168">Request</span></span>

<span data-ttu-id="82f99-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="82f99-169">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="82f99-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="82f99-170">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="82f99-171">C#</span><span class="sxs-lookup"><span data-stu-id="82f99-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-urlassessmentrequest-from-informationprotection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="82f99-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="82f99-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-urlassessmentrequest-from-informationprotection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="82f99-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="82f99-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-urlassessmentrequest-from-informationprotection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="82f99-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="82f99-174">Response</span></span>

<span data-ttu-id="82f99-175">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="82f99-175">The following is an example of the response.</span></span>

> <span data-ttu-id="82f99-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="82f99-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
