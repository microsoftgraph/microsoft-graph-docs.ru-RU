---
title: 'printDocument: uploadData'
description: Upload двоичный сегмент printDocument.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 6435a36e7713435dce3f38145d48083bdabcc532
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787599"
---
# <a name="printdocument-uploaddata"></a><span data-ttu-id="1c604-103">printDocument: uploadData</span><span class="sxs-lookup"><span data-stu-id="1c604-103">printDocument: uploadData</span></span>

<span data-ttu-id="1c604-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1c604-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1c604-105">Upload двоичный сегмент **printDocument**.</span><span class="sxs-lookup"><span data-stu-id="1c604-105">Upload a single binary segment of the **printDocument**.</span></span>

<span data-ttu-id="1c604-106">Вы можете загрузить весь файл или разделить его на несколько диапазонов byte, если размер запроса не превышает 1 МБ.</span><span class="sxs-lookup"><span data-stu-id="1c604-106">You can upload the entire file, or split the file into multiple byte ranges, as long as no request is larger than 1 MB.</span></span>

<span data-ttu-id="1c604-107">Сегменты файла можно отправлять в любом порядке, в том числе параллельно (до четырех параллельных запросов).</span><span class="sxs-lookup"><span data-stu-id="1c604-107">The segments of the file can be uploaded in any order and can be uploaded in parallel, with up to four concurrent requests.</span></span> <span data-ttu-id="1c604-108">При загрузке всех двоичных сегментов документа двоичный файл связан с **printJob.**</span><span class="sxs-lookup"><span data-stu-id="1c604-108">When all the binary segments of document are uploaded, the binary file is linked to the **printJob**.</span></span>

## <a name="permissions"></a><span data-ttu-id="1c604-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1c604-109">Permissions</span></span>
<span data-ttu-id="1c604-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c604-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="1c604-112">Помимо следующих разрешений, пользователь или клиент приложения должен иметь активную подписку на универсальную печать и иметь разрешение, которое предоставляет [доступ к принтеру Get.](printer-get.md)</span><span class="sxs-lookup"><span data-stu-id="1c604-112">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants [Get printer](printer-get.md) access.</span></span>

|<span data-ttu-id="1c604-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1c604-113">Permission type</span></span> | <span data-ttu-id="1c604-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1c604-114">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="1c604-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1c604-115">Delegated (work or school account)</span></span>| <span data-ttu-id="1c604-116">PrintJob.ReadWrite, PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c604-116">PrintJob.ReadWrite, PrintJob.ReadWrite.All</span></span> |
|<span data-ttu-id="1c604-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1c604-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1c604-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1c604-118">Not Supported.</span></span>|
|<span data-ttu-id="1c604-119">Приложение</span><span class="sxs-lookup"><span data-stu-id="1c604-119">Application</span></span>| <span data-ttu-id="1c604-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1c604-120">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1c604-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1c604-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/{id}/jobs/{id}/documents/{id}/uploadData
```
## <a name="request-headers"></a><span data-ttu-id="1c604-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1c604-122">Request headers</span></span>
| <span data-ttu-id="1c604-123">Имя</span><span class="sxs-lookup"><span data-stu-id="1c604-123">Name</span></span>          | <span data-ttu-id="1c604-124">Описание</span><span class="sxs-lookup"><span data-stu-id="1c604-124">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="1c604-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1c604-125">Authorization</span></span> | <span data-ttu-id="1c604-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1c604-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1c604-128">Range</span><span class="sxs-lookup"><span data-stu-id="1c604-128">Range</span></span> | <span data-ttu-id="1c604-129">bytes={startByteIndex}-{endByteIndex}</span><span class="sxs-lookup"><span data-stu-id="1c604-129">bytes={startByteIndex}-{endByteIndex}‬</span></span>  |
| <span data-ttu-id="1c604-130">Content-Length</span><span class="sxs-lookup"><span data-stu-id="1c604-130">Content-Length</span></span> | <span data-ttu-id="1c604-131">{contentLength}</span><span class="sxs-lookup"><span data-stu-id="1c604-131">{contentLength}‬</span></span>  |
| <span data-ttu-id="1c604-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1c604-132">Content-type</span></span>  | <span data-ttu-id="1c604-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1c604-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1c604-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1c604-135">Request body</span></span>
<span data-ttu-id="1c604-136">Текст запроса — это большой двоичный объект, содержащий байты документа, указанные как инклюзивный диапазон байтов, в заголовке `Range`.</span><span class="sxs-lookup"><span data-stu-id="1c604-136">The request body is a binary blob containing the bytes of the document that are specified as an inclusive byte range in the `Range` header.</span></span> 

## <a name="response"></a><span data-ttu-id="1c604-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="1c604-137">Response</span></span>
<span data-ttu-id="1c604-138">В случае успешной работы этот метод возвращает один из следующих ответов.</span><span class="sxs-lookup"><span data-stu-id="1c604-138">If successful, this method returns one of the following responses.</span></span> <span data-ttu-id="1c604-139">Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1c604-139">It does not return anything in the response body.</span></span>

| <span data-ttu-id="1c604-140">Условие</span><span class="sxs-lookup"><span data-stu-id="1c604-140">Condition</span></span>     | <span data-ttu-id="1c604-141">Код ответа</span><span class="sxs-lookup"><span data-stu-id="1c604-141">Response code</span></span> |
|:--------------|:--------------|
| <span data-ttu-id="1c604-142">Один или несколько двоичных сегментов по-прежнему необходимо загрузить</span><span class="sxs-lookup"><span data-stu-id="1c604-142">One or more binary segments still need to be uploaded</span></span> | `202 Accepted` |
| <span data-ttu-id="1c604-143">Все двоичные сегменты успешно загружены</span><span class="sxs-lookup"><span data-stu-id="1c604-143">All binary segments have been uploaded successfully</span></span> | `201 Created` |

## <a name="example"></a><span data-ttu-id="1c604-144">Пример</span><span class="sxs-lookup"><span data-stu-id="1c604-144">Example</span></span>
<span data-ttu-id="1c604-145">В следующем примере показано, как вызвать этот API, чтобы загрузить первые 72797 bytes документа.</span><span class="sxs-lookup"><span data-stu-id="1c604-145">The following example shows how to call this API to upload the first 72797 bytes of a document.</span></span>
##### <a name="request"></a><span data-ttu-id="1c604-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="1c604-146">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="1c604-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="1c604-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "printdocument-uploaddata"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/{id}/jobs/{id}/documents/{id}/uploadData
Range: bytes=0-72796
Content-Length: 72797
```
# <a name="c"></a>[<span data-ttu-id="1c604-148">C#</span><span class="sxs-lookup"><span data-stu-id="1c604-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/printdocument-uploaddata-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1c604-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1c604-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/printdocument-uploaddata-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1c604-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1c604-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/printdocument-uploaddata-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1c604-151">Java</span><span class="sxs-lookup"><span data-stu-id="1c604-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/printdocument-uploaddata-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="1c604-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="1c604-152">Response</span></span>

<span data-ttu-id="1c604-153">Отсутствуют один или несколько сегментов:</span><span class="sxs-lookup"><span data-stu-id="1c604-153">One or more segments missing:</span></span>
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 202 Accepted
```

<span data-ttu-id="1c604-154">Все полученные сегменты:</span><span class="sxs-lookup"><span data-stu-id="1c604-154">All segments received:</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printDocument"
} -->
```http
HTTP/1.1 201 Created
```


