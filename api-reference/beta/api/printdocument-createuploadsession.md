---
title: 'printDocument: createUploadSession'
description: Создайте сеанс отправки для последовательной отправки диапазонов двоичного файла printDocument.
localization_priority: Normal
author: nilakhan
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 47043b64806cfa9ef3a66026a60b84ae11112168
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48705142"
---
# <a name="printdocument-createuploadsession"></a><span data-ttu-id="b941d-103">printDocument: createUploadSession</span><span class="sxs-lookup"><span data-stu-id="b941d-103">printDocument: createUploadSession</span></span>

<span data-ttu-id="b941d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b941d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b941d-105">Создайте сеанс отправки, позволяющий приложению итеративно отправлять диапазоны двоичного файла, связанного с печатным документом.</span><span class="sxs-lookup"><span data-stu-id="b941d-105">Create an upload session that allows an app to iteratively upload ranges of a binary file linked to the print document.</span></span>

<span data-ttu-id="b941d-106">В качестве части ответа это действие возвращает URL-адрес отправки, который можно использовать в последующих последовательных `PUT` запросах.</span><span class="sxs-lookup"><span data-stu-id="b941d-106">As part of the response, this action returns an upload URL that can be used in subsequent sequential `PUT` queries.</span></span> <span data-ttu-id="b941d-107">Заголовков запросов для каждой `PUT` операции можно использовать для указания точного диапазона байтов, которые необходимо отправить.</span><span class="sxs-lookup"><span data-stu-id="b941d-107">Request headers for each `PUT` operation can be used to specify the exact range of bytes to be uploaded.</span></span> <span data-ttu-id="b941d-108">Это позволяет возобновить передачу в случае, если сетевое подключение будет разорвано во время отправки.</span><span class="sxs-lookup"><span data-stu-id="b941d-108">This allows transfer to be resumed, in case the network connection is dropped during upload.</span></span> 

## <a name="permissions"></a><span data-ttu-id="b941d-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b941d-109">Permissions</span></span>

<span data-ttu-id="b941d-110">Для вызова этого API требуется одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="b941d-110">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="b941d-111">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b941d-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>
<span data-ttu-id="b941d-112">В дополнение к следующим разрешениям пользователь или клиент приложения должен иметь активную универсальную подписку на печать и иметь разрешение на получение доступа к [принтеру](printer-get.md) или [Получение](printershare-get.md) доступа к принтершаре в зависимости от того, используется ли принтер или принтершаре.</span><span class="sxs-lookup"><span data-stu-id="b941d-112">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants [Get printer](printer-get.md) or [Get printerShare](printershare-get.md) access depending upon whether printer or printerShare is being used.</span></span>

| <span data-ttu-id="b941d-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b941d-113">Permission type</span></span>                        | <span data-ttu-id="b941d-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b941d-114">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b941d-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b941d-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="b941d-116">PrintJob. ReadWrite, PrintJob. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="b941d-116">PrintJob.ReadWrite, PrintJob.ReadWrite.All</span></span> |
| <span data-ttu-id="b941d-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b941d-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b941d-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b941d-118">Not Supported.</span></span> |
| <span data-ttu-id="b941d-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b941d-119">Application</span></span>                            | <span data-ttu-id="b941d-120">PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b941d-120">PrintJob.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b941d-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b941d-121">HTTP request</span></span>

<span data-ttu-id="b941d-122">Чтобы создать сеанс отправки с помощью **принтера**, выполните следующие действия:</span><span class="sxs-lookup"><span data-stu-id="b941d-122">To create an upload session using **printer**:</span></span> 

<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/{id}/jobs/{id}/documents/{id}/createUploadSession
```

<span data-ttu-id="b941d-123">Чтобы создать сеанс отправки с помощью **принтершаре**, выполните указанные ниже действия.</span><span class="sxs-lookup"><span data-stu-id="b941d-123">To create an upload session using **printerShare**:</span></span> 

<!-- { "blockType": "ignored" } -->
```http
POST /print/shares/{id}/jobs/{id}/documents/{id}/createUploadSession
```

## <a name="request-headers"></a><span data-ttu-id="b941d-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b941d-124">Request headers</span></span>

| <span data-ttu-id="b941d-125">Имя</span><span class="sxs-lookup"><span data-stu-id="b941d-125">Name</span></span>          | <span data-ttu-id="b941d-126">Описание</span><span class="sxs-lookup"><span data-stu-id="b941d-126">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="b941d-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b941d-127">Authorization</span></span> | <span data-ttu-id="b941d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b941d-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b941d-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b941d-130">Content-type</span></span> | <span data-ttu-id="b941d-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b941d-p104">application/json. Required.</span></span>|


## <a name="request-body"></a><span data-ttu-id="b941d-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b941d-133">Request body</span></span>

<span data-ttu-id="b941d-134">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="b941d-134">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b941d-135">Параметр</span><span class="sxs-lookup"><span data-stu-id="b941d-135">Parameter</span></span>    | <span data-ttu-id="b941d-136">Тип</span><span class="sxs-lookup"><span data-stu-id="b941d-136">Type</span></span>        | <span data-ttu-id="b941d-137">Описание</span><span class="sxs-lookup"><span data-stu-id="b941d-137">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b941d-138">properties</span><span class="sxs-lookup"><span data-stu-id="b941d-138">properties</span></span>|[<span data-ttu-id="b941d-139">принтдокументуплоадпропертиес</span><span class="sxs-lookup"><span data-stu-id="b941d-139">printDocumentUploadProperties</span></span>](../resources/printDocumentUploadProperties.md)|<span data-ttu-id="b941d-140">Представляет свойства двоичного файла, который необходимо отправить.</span><span class="sxs-lookup"><span data-stu-id="b941d-140">Represents properties of the binary file to be uploaded.</span></span>|

## <a name="response"></a><span data-ttu-id="b941d-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="b941d-141">Response</span></span>

<span data-ttu-id="b941d-142">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и новый объект [uploadSession](../resources/uploadsession.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b941d-142">If successful, this method returns a `200 OK` response code and a new [uploadSession](../resources/uploadsession.md) object in the response body.</span></span>

><span data-ttu-id="b941d-143">**Note**: свойство **адрес uploadurl** , возвращаемое как часть объекта Response **uploadSession** , является непрозрачным URL-адресом для последующих `PUT` запросов на отправку диапазонов байтов файла.</span><span class="sxs-lookup"><span data-stu-id="b941d-143">**Note**: The **uploadUrl** property returned as part of the **uploadSession** response object is an opaque URL for subsequent `PUT` queries to upload byte ranges of the file.</span></span> <span data-ttu-id="b941d-144">Он содержит соответствующий маркер проверки подлинности для последующих `PUT` запросов, срок действия которых истечет через **expirationDateTime**.</span><span class="sxs-lookup"><span data-stu-id="b941d-144">It contains the appropriate auth token for subsequent `PUT` queries that expire by **expirationDateTime**.</span></span> <span data-ttu-id="b941d-145">Не изменяйте этот URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="b941d-145">Do not change this URL.</span></span>

## <a name="examples"></a><span data-ttu-id="b941d-146">Примеры</span><span class="sxs-lookup"><span data-stu-id="b941d-146">Examples</span></span>

<span data-ttu-id="b941d-147">В приведенном ниже примере показано, как создать сеанс отправки, который можно использовать в последующих операциях отправки файлов для указанного элемента printDocument.</span><span class="sxs-lookup"><span data-stu-id="b941d-147">The following example shows how to create an upload session that you can use in subsequent file upload operations to the specified printDocument.</span></span>

### <a name="request"></a><span data-ttu-id="b941d-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="b941d-148">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="b941d-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="b941d-149">Response</span></span>

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
