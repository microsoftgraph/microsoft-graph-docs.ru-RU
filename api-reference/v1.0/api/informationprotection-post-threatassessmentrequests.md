---
title: Создание объекта threatAssessmentRequest
description: Создайте новый запрос на оценку угроз.
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 44a8f786f4b492ae094c9b8ef12b9eff125d7218
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2020
ms.locfileid: "42591532"
---
# <a name="create-threatassessmentrequest"></a><span data-ttu-id="8e21b-103">Создание объекта threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="8e21b-103">Create threatAssessmentRequest</span></span>

<span data-ttu-id="8e21b-104">Создайте новый запрос на оценку угроз.</span><span class="sxs-lookup"><span data-stu-id="8e21b-104">Create a new threat assessment request.</span></span>

<span data-ttu-id="8e21b-105">Запрос на оценку угроз может иметь один из следующих типов:</span><span class="sxs-lookup"><span data-stu-id="8e21b-105">A threat assessment request can be one of the following types:</span></span>

* [<span data-ttu-id="8e21b-106">Почта</span><span class="sxs-lookup"><span data-stu-id="8e21b-106">Mail</span></span>](../resources/mailAssessmentRequest.md)
* [<span data-ttu-id="8e21b-107">Файл электронной почты</span><span class="sxs-lookup"><span data-stu-id="8e21b-107">Email file</span></span>](../resources/emailFileAssessmentRequest.md)
* [<span data-ttu-id="8e21b-108">Файл</span><span class="sxs-lookup"><span data-stu-id="8e21b-108">File</span></span>](../resources/fileAssessmentRequest.md)
* [<span data-ttu-id="8e21b-109">URL</span><span class="sxs-lookup"><span data-stu-id="8e21b-109">URL</span></span>](../resources/urlAssessmentRequest.md)

## <a name="permissions"></a><span data-ttu-id="8e21b-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8e21b-110">Permissions</span></span>

<span data-ttu-id="8e21b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e21b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8e21b-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8e21b-113">Permission type</span></span>                        | <span data-ttu-id="8e21b-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8e21b-114">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8e21b-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8e21b-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="8e21b-116">Среатассессмент. ReadWrite. ALL.</span><span class="sxs-lookup"><span data-stu-id="8e21b-116">ThreatAssessment.ReadWrite.All.</span></span>             |
| <span data-ttu-id="8e21b-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8e21b-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8e21b-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e21b-118">Not supported.</span></span>                              |
| <span data-ttu-id="8e21b-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8e21b-119">Application</span></span>                            | <span data-ttu-id="8e21b-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e21b-120">Not supported.</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="8e21b-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8e21b-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /informationProtection/threatAssessmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="8e21b-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8e21b-122">Request headers</span></span>

| <span data-ttu-id="8e21b-123">Имя</span><span class="sxs-lookup"><span data-stu-id="8e21b-123">Name</span></span>          | <span data-ttu-id="8e21b-124">Описание</span><span class="sxs-lookup"><span data-stu-id="8e21b-124">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="8e21b-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8e21b-125">Authorization</span></span> | <span data-ttu-id="8e21b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8e21b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8e21b-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8e21b-128">Request body</span></span>

<span data-ttu-id="8e21b-129">В тексте запроса добавьте представление объекта [среатассессментрекуест](../resources/threatassessmentrequest.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8e21b-129">In the request body, supply a JSON representation of a [threatAssessmentRequest](../resources/threatassessmentrequest.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="8e21b-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e21b-130">Response</span></span>

<span data-ttu-id="8e21b-131">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и новый объект [среатассессментрекуест](../resources/threatassessmentrequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8e21b-131">If successful, this method returns a `201 Created` response code and a new [threatAssessmentRequest](../resources/threatassessmentrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8e21b-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="8e21b-132">Examples</span></span>

### <a name="example-1-create-a-mail-assessment-request"></a><span data-ttu-id="8e21b-133">Пример 1: Создание запроса на оценку почты</span><span class="sxs-lookup"><span data-stu-id="8e21b-133">Example 1: Create a mail assessment request</span></span>

#### <a name="request"></a><span data-ttu-id="8e21b-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="8e21b-134">Request</span></span>

<span data-ttu-id="8e21b-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8e21b-135">The following is an example of the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="8e21b-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e21b-136">Response</span></span>

<span data-ttu-id="8e21b-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8e21b-137">The following is an example of the response.</span></span>

> <span data-ttu-id="8e21b-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8e21b-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-create-an-email-assessment-request"></a><span data-ttu-id="8e21b-140">Пример 2: Создание запроса на оценку электронной почты</span><span class="sxs-lookup"><span data-stu-id="8e21b-140">Example 2: Create an email assessment request</span></span>

#### <a name="request"></a><span data-ttu-id="8e21b-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="8e21b-141">Request</span></span>

<span data-ttu-id="8e21b-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8e21b-142">The following is an example of the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="8e21b-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e21b-143">Response</span></span>

<span data-ttu-id="8e21b-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8e21b-144">The following is an example of the response.</span></span>

> <span data-ttu-id="8e21b-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8e21b-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-3-create-a-file-assessment-request"></a><span data-ttu-id="8e21b-147">Пример 3: Создание запроса на оценку файла</span><span class="sxs-lookup"><span data-stu-id="8e21b-147">Example 3: Create a file assessment request</span></span>

#### <a name="request"></a><span data-ttu-id="8e21b-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="8e21b-148">Request</span></span>

<span data-ttu-id="8e21b-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8e21b-149">The following is an example of the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="8e21b-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e21b-150">Response</span></span>

<span data-ttu-id="8e21b-151">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8e21b-151">The following is an example of the response.</span></span>

> <span data-ttu-id="8e21b-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8e21b-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-4-create-an-url-assessment-request"></a><span data-ttu-id="8e21b-154">Пример 4: Создание запроса на оценку URL-адреса</span><span class="sxs-lookup"><span data-stu-id="8e21b-154">Example 4: Create an url assessment request</span></span>

#### <a name="request"></a><span data-ttu-id="8e21b-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="8e21b-155">Request</span></span>

<span data-ttu-id="8e21b-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8e21b-156">The following is an example of the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="8e21b-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e21b-157">Response</span></span>

<span data-ttu-id="8e21b-158">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8e21b-158">The following is an example of the response.</span></span>

> <span data-ttu-id="8e21b-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8e21b-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
