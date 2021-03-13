---
title: Скачайте двоичный файл printDocument
description: Скачайте двоичный файл, связанный с документом.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 51997302289a3998192e104c9b025678de680857
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772088"
---
# <a name="download-printdocument-binary-file"></a><span data-ttu-id="60b13-103">Скачайте двоичный файл printDocument</span><span class="sxs-lookup"><span data-stu-id="60b13-103">Download printDocument binary file</span></span>

<span data-ttu-id="60b13-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="60b13-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="60b13-105">Скачайте двоичный файл, связанный с [печатьюDocument](../resources/printdocument.md).</span><span class="sxs-lookup"><span data-stu-id="60b13-105">Download the binary file associated with a [printDocument](../resources/printdocument.md).</span></span> <span data-ttu-id="60b13-106">Вызов этого метода дает ответ на перенаправление с предварительно заверяемым URL-адресом, который можно использовать для загрузки полезной нагрузки.</span><span class="sxs-lookup"><span data-stu-id="60b13-106">Calling this method yields a redirect response with a pre-authenticated URL that can be used to download the payload.</span></span>

## <a name="permissions"></a><span data-ttu-id="60b13-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="60b13-107">Permissions</span></span>
<span data-ttu-id="60b13-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="60b13-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="60b13-110">Помимо следующих разрешений, клиент пользователя или приложения должен иметь активную подписку на универсальную печать и иметь разрешение, да которое предоставляет доступ [к принтеру Get.](printer-get.md)</span><span class="sxs-lookup"><span data-stu-id="60b13-110">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants grants [Get printer](printer-get.md) access.</span></span>

| <span data-ttu-id="60b13-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="60b13-111">Permission type</span></span>                        | <span data-ttu-id="60b13-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="60b13-112">Permissions (from least to most privileged)</span></span>                  |
| :------------------------------------- | :----------------------------------------------------------- |
| <span data-ttu-id="60b13-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="60b13-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="60b13-114">PrintJob.Read, PrintJob.Read.All, PrintJob.ReadWrite, PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60b13-114">PrintJob.Read, PrintJob.Read.All, PrintJob.ReadWrite, PrintJob.ReadWrite.All</span></span> |
| <span data-ttu-id="60b13-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="60b13-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="60b13-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="60b13-116">Not Supported.</span></span>                                               |
| <span data-ttu-id="60b13-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="60b13-117">Application</span></span>                            | <span data-ttu-id="60b13-118">PrintJob.Read.All, PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60b13-118">PrintJob.Read.All, PrintJob.ReadWrite.All</span></span>                    |

## <a name="http-request"></a><span data-ttu-id="60b13-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="60b13-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers/{printerId}/jobs/{printJobId}/documents/{printDocumentId}/$value
```
## <a name="request-headers"></a><span data-ttu-id="60b13-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="60b13-120">Request headers</span></span>
| <span data-ttu-id="60b13-121">Имя</span><span class="sxs-lookup"><span data-stu-id="60b13-121">Name</span></span>          | <span data-ttu-id="60b13-122">Описание</span><span class="sxs-lookup"><span data-stu-id="60b13-122">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="60b13-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="60b13-123">Authorization</span></span> | <span data-ttu-id="60b13-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="60b13-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="60b13-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="60b13-126">Request body</span></span>
<span data-ttu-id="60b13-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="60b13-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="60b13-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="60b13-128">Response</span></span>
<span data-ttu-id="60b13-129">В случае успешной работы этот метод возвращает и `302 Found` предварительно заверяется URL-адрес загрузки в загонах Location.</span><span class="sxs-lookup"><span data-stu-id="60b13-129">If successful, this method returns `302 Found` and the pre-authenticated download URL in the Location header.</span></span>

## <a name="examples"></a><span data-ttu-id="60b13-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="60b13-130">Examples</span></span>
<span data-ttu-id="60b13-131">В следующем примере показано, как вызвать этот API для получения предварительно заверяемого URL-адреса загрузки.</span><span class="sxs-lookup"><span data-stu-id="60b13-131">The following example shows how to call this API to acquire a pre-authenticated download URL.</span></span> <span data-ttu-id="60b13-132">Чтобы начать скачивание, выполните URL-адрес перенаправления в ответе.</span><span class="sxs-lookup"><span data-stu-id="60b13-132">To start the download, follow the redirect URL in the response.</span></span>

### <a name="request"></a><span data-ttu-id="60b13-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="60b13-133">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="60b13-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="60b13-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_document_value"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/print/printers/{printerId}/jobs/{printJobId}/documents/{printDocumentId}/$value
```
# <a name="c"></a>[<span data-ttu-id="60b13-135">C#</span><span class="sxs-lookup"><span data-stu-id="60b13-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-document-value-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="60b13-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="60b13-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-document-value-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="60b13-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="60b13-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-document-value-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="60b13-138">Java</span><span class="sxs-lookup"><span data-stu-id="60b13-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-document-value-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="60b13-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="60b13-139">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 302 Found
Location: https://print.print.microsoft.com/downloads/bd260b1a-044e-4ca6-afa9-17d9a587d254?tempauthtoken={accesstoken}
```
