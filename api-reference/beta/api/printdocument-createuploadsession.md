---
title: 'printDocument: createUploadSession'
description: Создайте сеанс отправки для итеративной отправки диапазонов двоичных файлов printDocument.
localization_priority: Normal
author: nilakhan
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 0dbb2a9101fbf5033d1c91f1254c6ea0ba00f6e4
ms.sourcegitcommit: a0a5690ad9c109149e0b8c8baba164648ff5c226
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/08/2021
ms.locfileid: "49784851"
---
# <a name="printdocument-createuploadsession"></a><span data-ttu-id="31567-103">printDocument: createUploadSession</span><span class="sxs-lookup"><span data-stu-id="31567-103">printDocument: createUploadSession</span></span>

<span data-ttu-id="31567-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="31567-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="31567-105">Создайте сеанс отправки, который позволяет приложению итеративно загружать диапазоны двоичного файла, связанного с документом печати.</span><span class="sxs-lookup"><span data-stu-id="31567-105">Create an upload session that allows an app to iteratively upload ranges of a binary file linked to the print document.</span></span>

<span data-ttu-id="31567-106">В рамках ответа это действие возвращает URL-адрес отправки, который можно использовать в последующих `PUT` последовательном запросах.</span><span class="sxs-lookup"><span data-stu-id="31567-106">As part of the response, this action returns an upload URL that can be used in subsequent sequential `PUT` queries.</span></span> <span data-ttu-id="31567-107">Для указания точного диапазона отгрузки можно использовать заготчики запросов для каждой `PUT` операции.</span><span class="sxs-lookup"><span data-stu-id="31567-107">Request headers for each `PUT` operation can be used to specify the exact range of bytes to be uploaded.</span></span> <span data-ttu-id="31567-108">Это позволяет возобновить передачу на случай, если сетевое подключение будет отброшено во время отправки.</span><span class="sxs-lookup"><span data-stu-id="31567-108">This allows transfer to be resumed, in case the network connection is dropped during upload.</span></span> 

## <a name="permissions"></a><span data-ttu-id="31567-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="31567-109">Permissions</span></span>

<span data-ttu-id="31567-110">Для вызова этого API требуется одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="31567-110">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="31567-111">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="31567-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>
<span data-ttu-id="31567-112">Помимо следующих разрешений, у пользователя или клиента приложения должна быть активная подписка [](printer-get.md) универсальной печати и разрешение, которое предоставляет доступ "Получить принтер" или "Получить [printerShare"](printershare-get.md) в зависимости от того, используется ли принтер или printerShare.</span><span class="sxs-lookup"><span data-stu-id="31567-112">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants [Get printer](printer-get.md) or [Get printerShare](printershare-get.md) access depending upon whether printer or printerShare is being used.</span></span>

| <span data-ttu-id="31567-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="31567-113">Permission type</span></span>                        | <span data-ttu-id="31567-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="31567-114">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="31567-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="31567-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="31567-116">PrintJob.Create, PrintJob.ReadWrite, PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31567-116">PrintJob.Create, PrintJob.ReadWrite, PrintJob.ReadWrite.All</span></span> |
| <span data-ttu-id="31567-117">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="31567-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="31567-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="31567-118">Not Supported.</span></span> |
| <span data-ttu-id="31567-119">Приложение</span><span class="sxs-lookup"><span data-stu-id="31567-119">Application</span></span>                            | <span data-ttu-id="31567-120">PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31567-120">PrintJob.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="31567-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="31567-121">HTTP request</span></span>

<span data-ttu-id="31567-122">Чтобы создать сеанс отправки с помощью **принтера:**</span><span class="sxs-lookup"><span data-stu-id="31567-122">To create an upload session using **printer**:</span></span> 

<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/{id}/jobs/{id}/documents/{id}/createUploadSession
```

<span data-ttu-id="31567-123">Чтобы создать сеанс отправки с помощью **printerShare:**</span><span class="sxs-lookup"><span data-stu-id="31567-123">To create an upload session using **printerShare**:</span></span> 

<!-- { "blockType": "ignored" } -->
```http
POST /print/shares/{id}/jobs/{id}/documents/{id}/createUploadSession
```

## <a name="request-headers"></a><span data-ttu-id="31567-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="31567-124">Request headers</span></span>

| <span data-ttu-id="31567-125">Имя</span><span class="sxs-lookup"><span data-stu-id="31567-125">Name</span></span>          | <span data-ttu-id="31567-126">Описание</span><span class="sxs-lookup"><span data-stu-id="31567-126">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="31567-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="31567-127">Authorization</span></span> | <span data-ttu-id="31567-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="31567-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="31567-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="31567-130">Content-type</span></span> | <span data-ttu-id="31567-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="31567-p104">application/json. Required.</span></span>|


## <a name="request-body"></a><span data-ttu-id="31567-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="31567-133">Request body</span></span>

<span data-ttu-id="31567-134">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="31567-134">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="31567-135">Параметр</span><span class="sxs-lookup"><span data-stu-id="31567-135">Parameter</span></span>    | <span data-ttu-id="31567-136">Тип</span><span class="sxs-lookup"><span data-stu-id="31567-136">Type</span></span>        | <span data-ttu-id="31567-137">Описание</span><span class="sxs-lookup"><span data-stu-id="31567-137">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="31567-138">properties</span><span class="sxs-lookup"><span data-stu-id="31567-138">properties</span></span>|[<span data-ttu-id="31567-139">printDocumentUploadProperties</span><span class="sxs-lookup"><span data-stu-id="31567-139">printDocumentUploadProperties</span></span>](../resources/printDocumentUploadProperties.md)|<span data-ttu-id="31567-140">Представляет свойства двоичного файла, который необходимо отправить.</span><span class="sxs-lookup"><span data-stu-id="31567-140">Represents properties of the binary file to be uploaded.</span></span>|

<span data-ttu-id="31567-141">Значение свойства **contentType** в теле запроса должно поддерживаться принтером или printerShare.</span><span class="sxs-lookup"><span data-stu-id="31567-141">The value of the **contentType** property in the request body should be supported by the printer/printerShare.</span></span> <span data-ttu-id="31567-142">Вы можете получить поддерживаемые типы контента, получив [printerCapabilities](../resources/printercapabilities.md) принтера или printerShare.</span><span class="sxs-lookup"><span data-stu-id="31567-142">You can get the supported content types by getting [printerCapabilities](../resources/printercapabilities.md) of the printer/printerShare.</span></span> 

<span data-ttu-id="31567-143">Для **преобразования OXPS** в ФОРМАТ PDF необходимо передать в качестве contentType для `application/oxps` принтера или принтераShare, который поддерживает `application/pdf` .</span><span class="sxs-lookup"><span data-stu-id="31567-143">For **OXPS to PDF** conversion, you need to pass `application/oxps` as contentType for printer/printerShare that supports `application/pdf`.</span></span> <span data-ttu-id="31567-144">Универсальная печать преобразует **OXPS в ФОРМАТ PDF** при **следующих** условиях:</span><span class="sxs-lookup"><span data-stu-id="31567-144">Universal Print converts **OXPS to PDF**, when **all** the following conditions are met:</span></span> 
1.  <span data-ttu-id="31567-145">В `application/pdf` **printerCapabilities** поддерживается совместное использования принтера или принтера.</span><span class="sxs-lookup"><span data-stu-id="31567-145">The printer/printer share supports `application/pdf` in **printerCapabilities**.</span></span> 
2.  <span data-ttu-id="31567-146">The printer/printer share does NOT support `application/oxps` in **printerCapabilities**.</span><span class="sxs-lookup"><span data-stu-id="31567-146">The printer/printer share does NOT support `application/oxps` in **printerCapabilities**.</span></span> 
3.  <span data-ttu-id="31567-147">Значение свойства **contentType** в теле запроса: `application/oxps` .</span><span class="sxs-lookup"><span data-stu-id="31567-147">The value for the **contentType** property in the request body is `application/oxps`.</span></span>

## <a name="response"></a><span data-ttu-id="31567-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="31567-148">Response</span></span>

<span data-ttu-id="31567-149">В случае успеха этот метод возвращает код отклика и новый объект `200 OK` [uploadSession](../resources/uploadsession.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="31567-149">If successful, this method returns a `200 OK` response code and a new [uploadSession](../resources/uploadsession.md) object in the response body.</span></span>

><span data-ttu-id="31567-150">**Примечание.** Свойство **uploadUrl,** возвращаемого в рамках объекта ответа **uploadSession,** является непрозрачным URL-адресом для последующих запросов на отправку диапазонов байтов `PUT` файла.</span><span class="sxs-lookup"><span data-stu-id="31567-150">**Note**: The **uploadUrl** property returned as part of the **uploadSession** response object is an opaque URL for subsequent `PUT` queries to upload byte ranges of the file.</span></span> <span data-ttu-id="31567-151">Он содержит соответствующий маркер auth для последующих запросов, срок действия `PUT` которых **истекает по истечении срока действия.**</span><span class="sxs-lookup"><span data-stu-id="31567-151">It contains the appropriate auth token for subsequent `PUT` queries that expire by **expirationDateTime**.</span></span> <span data-ttu-id="31567-152">Не изменяя этот URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="31567-152">Do not change this URL.</span></span>

## <a name="examples"></a><span data-ttu-id="31567-153">Примеры</span><span class="sxs-lookup"><span data-stu-id="31567-153">Examples</span></span>

<span data-ttu-id="31567-154">В следующем примере показано, как создать сеанс отправки, который можно использовать при последующих операциях отправки файлов в указанный printDocument.</span><span class="sxs-lookup"><span data-stu-id="31567-154">The following example shows how to create an upload session that you can use in subsequent file upload operations to the specified printDocument.</span></span>

### <a name="request"></a><span data-ttu-id="31567-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="31567-155">Request</span></span>

<!-- {
  "blockType": "request",
}-->
```http
POST https://graph.microsoft.com/beta/print/shares/1c879027-5120-4aaf-954a-ebfd509a3bcc/jobs/46207/documents/9001bcd9-e36a-4f51-bfc6-140c3ad7f9f7/createUploadSession
Content-type: application/json

{
  "properties": {
    "documentName": "TestFile.pdf",
    "contentType": "application/pdf", 
    "size": 4533322
  }
}
```

### <a name="response"></a><span data-ttu-id="31567-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="31567-156">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.uploadSession"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.uploadSession",
    "uploadUrl": "https://print.print.microsoft.com/uploadSessions/5400be13-5a4e-4c20-be70-90c85bfe5d6e?tempauthtoken={token}",
    "expirationDateTime": "2020-10-25T02:19:38.1694207Z",
    "nextExpectedRanges": [
        "0-4533321"
    ]
}
```
