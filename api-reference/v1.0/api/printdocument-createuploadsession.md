---
title: 'printDocument: createUploadSession'
description: Создайте сеанс загрузки для итеративных диапазонов загрузки двоичного файла printDocument.
localization_priority: Normal
author: nilakhan
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 9de1372e4c4e9bb6819c06a563eda6763a407d0e
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50518044"
---
# <a name="printdocument-createuploadsession"></a><span data-ttu-id="03f63-103">printDocument: createUploadSession</span><span class="sxs-lookup"><span data-stu-id="03f63-103">printDocument: createUploadSession</span></span>
<span data-ttu-id="03f63-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="03f63-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="03f63-105">Создайте сеанс загрузки, который позволяет приложению итеративным образом загружать диапазоны двоичного файла, связанного с документом печати.</span><span class="sxs-lookup"><span data-stu-id="03f63-105">Create an upload session that allows an app to iteratively upload ranges of a binary file linked to the print document.</span></span>

<span data-ttu-id="03f63-106">В рамках ответа это действие возвращает URL-адрес загрузки, который можно использовать в последующих последовательном `PUT` запросах.</span><span class="sxs-lookup"><span data-stu-id="03f63-106">As part of the response, this action returns an upload URL that can be used in subsequent sequential `PUT` queries.</span></span> <span data-ttu-id="03f63-107">Для каждой операции можно указать точный диапазон отгрузки `PUT` bytes.</span><span class="sxs-lookup"><span data-stu-id="03f63-107">Request headers for each `PUT` operation can be used to specify the exact range of bytes to be uploaded.</span></span> <span data-ttu-id="03f63-108">Это позволяет возобновить передачу, если подключение к сети будет отброшено во время загрузки.</span><span class="sxs-lookup"><span data-stu-id="03f63-108">This allows transfer to be resumed, in case the network connection is dropped during upload.</span></span> 

## <a name="permissions"></a><span data-ttu-id="03f63-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="03f63-109">Permissions</span></span>
<span data-ttu-id="03f63-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03f63-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="03f63-112">Помимо следующих разрешений, клиент пользователя или приложения должен иметь активную подписку на универсальную печать и иметь разрешение, которое предоставляет доступ [к принтеру Get](printer-get.md) или [Get printerShare](printershare-get.md) в зависимости от того, используется ли принтер или принтер.</span><span class="sxs-lookup"><span data-stu-id="03f63-112">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants [Get printer](printer-get.md) or [Get printerShare](printershare-get.md) access depending upon whether printer or printerShare is being used.</span></span>

| <span data-ttu-id="03f63-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="03f63-113">Permission type</span></span>                        | <span data-ttu-id="03f63-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="03f63-114">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="03f63-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="03f63-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="03f63-116">PrintJob.Create, PrintJob.ReadWrite, PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03f63-116">PrintJob.Create, PrintJob.ReadWrite, PrintJob.ReadWrite.All</span></span> |
| <span data-ttu-id="03f63-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="03f63-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="03f63-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03f63-118">Not Supported.</span></span> |
| <span data-ttu-id="03f63-119">Приложение</span><span class="sxs-lookup"><span data-stu-id="03f63-119">Application</span></span>                            | <span data-ttu-id="03f63-120">PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03f63-120">PrintJob.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="03f63-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="03f63-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

<span data-ttu-id="03f63-122">Создание сеанса загрузки с помощью **принтера:**</span><span class="sxs-lookup"><span data-stu-id="03f63-122">To create an upload session using **printer**:</span></span> 

<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/{id}/jobs/{id}/documents/{id}/createUploadSession
```

<span data-ttu-id="03f63-123">Создание сеанса загрузки с **помощью printerShare:**</span><span class="sxs-lookup"><span data-stu-id="03f63-123">To create an upload session using **printerShare**:</span></span> 

<!-- { "blockType": "ignored" } -->
```http
POST /print/shares/{id}/jobs/{id}/documents/{id}/createUploadSession
```

## <a name="request-headers"></a><span data-ttu-id="03f63-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="03f63-124">Request headers</span></span>
|<span data-ttu-id="03f63-125">Имя</span><span class="sxs-lookup"><span data-stu-id="03f63-125">Name</span></span>|<span data-ttu-id="03f63-126">Описание</span><span class="sxs-lookup"><span data-stu-id="03f63-126">Description</span></span>|
|:---|:---|
|<span data-ttu-id="03f63-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="03f63-127">Authorization</span></span>|<span data-ttu-id="03f63-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="03f63-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="03f63-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="03f63-130">Content-Type</span></span>|<span data-ttu-id="03f63-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="03f63-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="03f63-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="03f63-133">Request body</span></span>
<span data-ttu-id="03f63-134">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="03f63-134">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="03f63-135">Параметр</span><span class="sxs-lookup"><span data-stu-id="03f63-135">Parameter</span></span>    | <span data-ttu-id="03f63-136">Тип</span><span class="sxs-lookup"><span data-stu-id="03f63-136">Type</span></span>        | <span data-ttu-id="03f63-137">Описание</span><span class="sxs-lookup"><span data-stu-id="03f63-137">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="03f63-138">properties</span><span class="sxs-lookup"><span data-stu-id="03f63-138">properties</span></span>|[<span data-ttu-id="03f63-139">printDocumentUploadProperties</span><span class="sxs-lookup"><span data-stu-id="03f63-139">printDocumentUploadProperties</span></span>](../resources/printDocumentUploadProperties.md)|<span data-ttu-id="03f63-140">Представляет свойства двоичного файла, который будет загружен.</span><span class="sxs-lookup"><span data-stu-id="03f63-140">Represents properties of the binary file to be uploaded.</span></span>|

<span data-ttu-id="03f63-141">Значение свойства **contentType** в теле запроса должно поддерживаться принтером или принтеромShare.</span><span class="sxs-lookup"><span data-stu-id="03f63-141">The value of the **contentType** property in the request body should be supported by the printer/printerShare.</span></span> <span data-ttu-id="03f63-142">Поддерживаемые типы контента можно получить с помощью [принтераCapabilities](../resources/printercapabilities.md) принтера или принтераShare.</span><span class="sxs-lookup"><span data-stu-id="03f63-142">You can get the supported content types by getting [printerCapabilities](../resources/printercapabilities.md) of the printer/printerShare.</span></span> 

<span data-ttu-id="03f63-143">Для **преобразования OXPS в PDF** необходимо передать в качестве `application/oxps` contentType для принтера или принтераShare, который поддерживает `application/pdf` .</span><span class="sxs-lookup"><span data-stu-id="03f63-143">For **OXPS to PDF** conversion, you need to pass `application/oxps` as contentType for printer/printerShare that supports `application/pdf`.</span></span> <span data-ttu-id="03f63-144">Universal Print преобразует **OXPS в PDF,** когда **будут** выполнены все следующие условия:</span><span class="sxs-lookup"><span data-stu-id="03f63-144">Universal Print converts **OXPS to PDF**, when **all** the following conditions are met:</span></span> 
1.  <span data-ttu-id="03f63-145">В printerCapabilities поддерживается совместное использования `application/pdf` **принтера и принтера.**</span><span class="sxs-lookup"><span data-stu-id="03f63-145">The printer/printer share supports `application/pdf` in **printerCapabilities**.</span></span> 
2.  <span data-ttu-id="03f63-146">Доля принтера и принтера не поддерживается `application/oxps` в **printerCapabilities.**</span><span class="sxs-lookup"><span data-stu-id="03f63-146">The printer/printer share does NOT support `application/oxps` in **printerCapabilities**.</span></span> 
3.  <span data-ttu-id="03f63-147">Значение свойства **contentType** в теле запроса `application/oxps` : .</span><span class="sxs-lookup"><span data-stu-id="03f63-147">The value for the **contentType** property in the request body is `application/oxps`.</span></span>

## <a name="response"></a><span data-ttu-id="03f63-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="03f63-148">Response</span></span>

<span data-ttu-id="03f63-149">В случае успешной работы этот метод возвращает код ответа и новый объект `200 OK` [uploadSession](../resources/uploadsession.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="03f63-149">If successful, this method returns a `200 OK` response code and a new [uploadSession](../resources/uploadsession.md) object in the response body.</span></span>

><span data-ttu-id="03f63-150">**Примечание.** Свойство **uploadUrl,** возвращенное в рамках объекта ответа **uploadSession,** является непрозрачной URL-адресом для последующих запросов для загрузки байт-диапазонов `PUT` файла.</span><span class="sxs-lookup"><span data-stu-id="03f63-150">**Note**: The **uploadUrl** property returned as part of the **uploadSession** response object is an opaque URL for subsequent `PUT` queries to upload byte ranges of the file.</span></span> <span data-ttu-id="03f63-151">Он содержит соответствующий маркер auth для последующих запросов, срок действия `PUT` которых **истекает по истечении срока действияDateTime.**</span><span class="sxs-lookup"><span data-stu-id="03f63-151">It contains the appropriate auth token for subsequent `PUT` queries that expire by **expirationDateTime**.</span></span> <span data-ttu-id="03f63-152">Не измените этот URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="03f63-152">Do not change this URL.</span></span>

## <a name="examples"></a><span data-ttu-id="03f63-153">Примеры</span><span class="sxs-lookup"><span data-stu-id="03f63-153">Examples</span></span>

<span data-ttu-id="03f63-154">В следующем примере показано, как создать сеанс загрузки, который можно использовать в последующих операциях по отправке файлов в указанный printDocument.</span><span class="sxs-lookup"><span data-stu-id="03f63-154">The following example shows how to create an upload session that you can use in subsequent file upload operations to the specified printDocument.</span></span>

### <a name="request"></a><span data-ttu-id="03f63-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="03f63-155">Request</span></span>
<!-- {
  "blockType": "request"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/print/printers/{printerId}/jobs/{printJobId}/documents/{printDocumentId}/createUploadSession
Content-Type: application/json
Content-length: 96

{
  "properties": {
    "documentName": "TestFile.pdf",
    "contentType": "application/pdf", 
    "size": 4533322
  }
}
```


### <a name="response"></a><span data-ttu-id="03f63-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="03f63-156">Response</span></span>
<span data-ttu-id="03f63-157">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="03f63-157">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.uploadSession"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#microsoft.graph.uploadSession",
    "uploadUrl": "https://print.print.microsoft.com/uploadSessions/5400be13-5a4e-4c20-be70-90c85bfe5d6e?tempauthtoken={token}",
    "expirationDateTime": "2020-10-25T02:19:38.1694207Z",
    "nextExpectedRanges": [
        "0-4533321"
    ]
}
```

