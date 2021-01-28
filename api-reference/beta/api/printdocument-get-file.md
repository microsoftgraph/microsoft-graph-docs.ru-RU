---
title: Скачивание двоичного файла printDocument
description: Скачайте двоичный файл, связанный с документом.
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 590b97c01623cba26407ca0a39ad7d0b3b7a1ca3
ms.sourcegitcommit: 9a03b719d1316729dd022bf4d268894e91515475
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/28/2021
ms.locfileid: "50034235"
---
# <a name="download-printdocument-binary-file"></a><span data-ttu-id="5ec80-103">Скачивание двоичного файла printDocument</span><span class="sxs-lookup"><span data-stu-id="5ec80-103">Download printDocument binary file</span></span>

<span data-ttu-id="5ec80-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5ec80-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5ec80-105">Скачайте двоичный файл, связанный с [printDocument.](../resources/printdocument.md)</span><span class="sxs-lookup"><span data-stu-id="5ec80-105">Download the binary file associated with a [printDocument](../resources/printdocument.md).</span></span> <span data-ttu-id="5ec80-106">Вызов этого метода дает отклик перенаправления с URL-адресом с предварительной проверкой подлинности, который можно использовать для скачивания полезной нагрузки.</span><span class="sxs-lookup"><span data-stu-id="5ec80-106">Calling this method yields a redirect response with a pre-authenticated URL that can be used to download the payload.</span></span>

## <a name="permissions"></a><span data-ttu-id="5ec80-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5ec80-107">Permissions</span></span>
<span data-ttu-id="5ec80-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ec80-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="5ec80-110">Помимо перечисленных ниже разрешений, у пользователя или клиента приложения должна быть активная подписка универсальной печати и разрешение, которое предоставляет доступ к [принтеру.](printer-get.md)</span><span class="sxs-lookup"><span data-stu-id="5ec80-110">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants grants [Get printer](printer-get.md) access.</span></span>

| <span data-ttu-id="5ec80-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5ec80-111">Permission type</span></span>                        | <span data-ttu-id="5ec80-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5ec80-112">Permissions (from least to most privileged)</span></span>                  |
| :------------------------------------- | :----------------------------------------------------------- |
| <span data-ttu-id="5ec80-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5ec80-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="5ec80-114">PrintJob.Read, PrintJob.Read.All, PrintJob.ReadWrite, PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ec80-114">PrintJob.Read, PrintJob.Read.All, PrintJob.ReadWrite, PrintJob.ReadWrite.All</span></span> |
| <span data-ttu-id="5ec80-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5ec80-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5ec80-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5ec80-116">Not Supported.</span></span>                                               |
| <span data-ttu-id="5ec80-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5ec80-117">Application</span></span>                            | <span data-ttu-id="5ec80-118">PrintJob.Read.All, PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ec80-118">PrintJob.Read.All, PrintJob.ReadWrite.All</span></span>                    |

## <a name="http-request"></a><span data-ttu-id="5ec80-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5ec80-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers/{id}/jobs/{id}/documents/{id}/$value
```
## <a name="request-headers"></a><span data-ttu-id="5ec80-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5ec80-120">Request headers</span></span>
| <span data-ttu-id="5ec80-121">Имя</span><span class="sxs-lookup"><span data-stu-id="5ec80-121">Name</span></span>          | <span data-ttu-id="5ec80-122">Описание</span><span class="sxs-lookup"><span data-stu-id="5ec80-122">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="5ec80-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5ec80-123">Authorization</span></span> | <span data-ttu-id="5ec80-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5ec80-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5ec80-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5ec80-126">Request body</span></span>
<span data-ttu-id="5ec80-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5ec80-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5ec80-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="5ec80-128">Response</span></span>
<span data-ttu-id="5ec80-129">В случае успеха этот метод возвращает URL-адрес скачивания с предварительной проверкой подлинности `302 Found` в заголке Location.</span><span class="sxs-lookup"><span data-stu-id="5ec80-129">If successful, this method returns `302 Found` and the pre-authenticated download URL in the Location header.</span></span>

## <a name="examples"></a><span data-ttu-id="5ec80-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="5ec80-130">Examples</span></span>
<span data-ttu-id="5ec80-131">В следующем примере показано, как вызвать этот API для получения URL-адреса скачивания с предварительной проверкой подлинности.</span><span class="sxs-lookup"><span data-stu-id="5ec80-131">The following example shows how to call this API to acquire a pre-authenticated download URL.</span></span> <span data-ttu-id="5ec80-132">Чтобы начать скачивание, следуйте URL-адресу перенаправления в ответе.</span><span class="sxs-lookup"><span data-stu-id="5ec80-132">To start the download, follow the redirect URL in the response.</span></span>

### <a name="request"></a><span data-ttu-id="5ec80-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="5ec80-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="5ec80-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="5ec80-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_document_value"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/fcb0bc53-a446-41d0-bfc3-5c56cdbb0f2a/jobs/46140/documents/bd260b1a-044e-4ca6-afa9-17d9a587d254/$value
```
# <a name="c"></a>[<span data-ttu-id="5ec80-135">C#</span><span class="sxs-lookup"><span data-stu-id="5ec80-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-document-value-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5ec80-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5ec80-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-document-value-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5ec80-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5ec80-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-document-value-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5ec80-138">Java</span><span class="sxs-lookup"><span data-stu-id="5ec80-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-document-value-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5ec80-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="5ec80-139">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 302 Accepted
Location: https://print.print.microsoft.com/downloads/bd260b1a-044e-4ca6-afa9-17d9a587d254?tempauthtoken={accesstoken}
```
