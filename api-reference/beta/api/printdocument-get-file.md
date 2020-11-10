---
title: Загрузка двоичного файла printDocument
description: Скачайте двоичный файл, связанный с документом.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 8986b704a8d7c36d510d4c4859003df1f5a7e94b
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48981504"
---
# <a name="download-printdocument-binary-file"></a><span data-ttu-id="f0a9a-103">Загрузка двоичного файла printDocument</span><span class="sxs-lookup"><span data-stu-id="f0a9a-103">Download printDocument binary file</span></span>

<span data-ttu-id="f0a9a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f0a9a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0a9a-105">Скачайте двоичный файл, связанный с [printDocument](../resources/printdocument.md).</span><span class="sxs-lookup"><span data-stu-id="f0a9a-105">Download the binary file associated with a [printDocument](../resources/printdocument.md).</span></span> <span data-ttu-id="f0a9a-106">При вызове этого метода выдается ответ перенаправления с URL-адресом, предварительно прошедший проверку подлинности, который можно использовать для загрузки полезных данных.</span><span class="sxs-lookup"><span data-stu-id="f0a9a-106">Calling this method yields a redirect response with a pre-authenticated URL that can be used to download the payload.</span></span>

## <a name="permissions"></a><span data-ttu-id="f0a9a-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f0a9a-107">Permissions</span></span>
<span data-ttu-id="f0a9a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f0a9a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="f0a9a-110">В дополнение к следующим разрешениям пользователь или клиент приложения должен иметь активную универсальную подписку на печать и иметь разрешение на получение доступа к [принтеру](printer-get.md) .</span><span class="sxs-lookup"><span data-stu-id="f0a9a-110">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants [Get printer](printer-get.md) access.</span></span>

| <span data-ttu-id="f0a9a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f0a9a-111">Permission type</span></span>                        | <span data-ttu-id="f0a9a-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f0a9a-112">Permissions (from least to most privileged)</span></span>                  |
| :------------------------------------- | :----------------------------------------------------------- |
| <span data-ttu-id="f0a9a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f0a9a-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="f0a9a-114">PrintJob. Read, PrintJob. Read. ALL, PrintJob. ReadWrite, PrintJob. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="f0a9a-114">PrintJob.Read, PrintJob.Read.All, PrintJob.ReadWrite, PrintJob.ReadWrite.All</span></span> |
| <span data-ttu-id="f0a9a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f0a9a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f0a9a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0a9a-116">Not Supported.</span></span>                                               |
| <span data-ttu-id="f0a9a-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="f0a9a-117">Application</span></span>                            | <span data-ttu-id="f0a9a-118">PrintJob. Read. ALL, PrintJob. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="f0a9a-118">PrintJob.Read.All, PrintJob.ReadWrite.All</span></span>                    |

## <a name="http-request"></a><span data-ttu-id="f0a9a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f0a9a-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers/{id}/jobs/{id}/documents/{id}/$value
```
## <a name="request-headers"></a><span data-ttu-id="f0a9a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f0a9a-120">Request headers</span></span>
| <span data-ttu-id="f0a9a-121">Имя</span><span class="sxs-lookup"><span data-stu-id="f0a9a-121">Name</span></span>          | <span data-ttu-id="f0a9a-122">Описание</span><span class="sxs-lookup"><span data-stu-id="f0a9a-122">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="f0a9a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f0a9a-123">Authorization</span></span> | <span data-ttu-id="f0a9a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f0a9a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f0a9a-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f0a9a-126">Request body</span></span>
<span data-ttu-id="f0a9a-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f0a9a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f0a9a-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="f0a9a-128">Response</span></span>
<span data-ttu-id="f0a9a-129">В случае успешного выполнения этот метод возвращает `302 Found` URL-адрес скачивания, предварительно прошедший проверку подлинности, в заголовке Location.</span><span class="sxs-lookup"><span data-stu-id="f0a9a-129">If successful, this method returns `302 Found` and the pre-authenticated download URL in the Location header.</span></span>

## <a name="examples"></a><span data-ttu-id="f0a9a-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="f0a9a-130">Examples</span></span>
<span data-ttu-id="f0a9a-131">В приведенном ниже примере показано, как вызвать этот API, чтобы получить URL-адрес для скачивания, прошедший проверку подлинности.</span><span class="sxs-lookup"><span data-stu-id="f0a9a-131">The following example shows how to call this API to acquire a pre-authenticated download URL.</span></span> <span data-ttu-id="f0a9a-132">Чтобы начать загрузку, следуйте указаниям URL-адреса перенаправления в ответе.</span><span class="sxs-lookup"><span data-stu-id="f0a9a-132">To start the download, follow the redirect URL in the response.</span></span>

### <a name="request"></a><span data-ttu-id="f0a9a-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="f0a9a-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="f0a9a-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="f0a9a-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_document_value"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/fcb0bc53-a446-41d0-bfc3-5c56cdbb0f2a/jobs/46140/documents/bd260b1a-044e-4ca6-afa9-17d9a587d254/$value
```
# <a name="c"></a>[<span data-ttu-id="f0a9a-135">C#</span><span class="sxs-lookup"><span data-stu-id="f0a9a-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-document-value-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f0a9a-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f0a9a-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-document-value-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f0a9a-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f0a9a-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-document-value-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f0a9a-138">Java</span><span class="sxs-lookup"><span data-stu-id="f0a9a-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-document-value-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f0a9a-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="f0a9a-139">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 302 Accepted
Location: https://print.print.microsoft.com/downloads/bd260b1a-044e-4ca6-afa9-17d9a587d254?tempauthtoken={accesstoken}
```
