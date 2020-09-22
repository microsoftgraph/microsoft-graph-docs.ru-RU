---
title: 'printDocument: Уплоаддата'
description: Отправьте один двоичный сегмент printDocument.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 7a06f00b1ff024e116ed7d16cf416d23089f615e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48035815"
---
# <a name="printdocument-uploaddata"></a><span data-ttu-id="e4c04-103">printDocument: Уплоаддата</span><span class="sxs-lookup"><span data-stu-id="e4c04-103">printDocument: uploadData</span></span>

<span data-ttu-id="e4c04-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4c04-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e4c04-105">Отправьте один двоичный сегмент **printDocument**.</span><span class="sxs-lookup"><span data-stu-id="e4c04-105">Upload a single binary segment of the **printDocument**.</span></span>

<span data-ttu-id="e4c04-106">Вы можете отправить файл целиком или разбить его на несколько диапазонов байтов, если число запросов не превышает 1 МБ.</span><span class="sxs-lookup"><span data-stu-id="e4c04-106">You can upload the entire file, or split the file into multiple byte ranges, as long as no request is larger than 1 MB.</span></span>

<span data-ttu-id="e4c04-107">Сегменты файла можно отправить в любом порядке и можно отправить параллельно, используя до четырех одновременных запросов.</span><span class="sxs-lookup"><span data-stu-id="e4c04-107">The segments of the file can be uploaded in any order and can be uploaded in parallel, with up to four concurrent requests.</span></span> <span data-ttu-id="e4c04-108">После отправки всех двоичных сегментов документа двоичный файл связывается с **методом printJob**.</span><span class="sxs-lookup"><span data-stu-id="e4c04-108">When all the binary segments of document are uploaded, the binary file is linked to the **printJob**.</span></span>

## <a name="permissions"></a><span data-ttu-id="e4c04-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e4c04-109">Permissions</span></span>
<span data-ttu-id="e4c04-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4c04-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="e4c04-112">В дополнение к следующим разрешениям пользователь или клиент приложения должен иметь активную универсальную подписку на печать и иметь разрешение на получение доступа к [принтеру](printer-get.md) .</span><span class="sxs-lookup"><span data-stu-id="e4c04-112">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants [Get printer](printer-get.md) access.</span></span>

|<span data-ttu-id="e4c04-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e4c04-113">Permission type</span></span> | <span data-ttu-id="e4c04-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e4c04-114">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="e4c04-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e4c04-115">Delegated (work or school account)</span></span>| <span data-ttu-id="e4c04-116">PrintJob. ReadWrite, PrintJob. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="e4c04-116">PrintJob.ReadWrite, PrintJob.ReadWrite.All</span></span> |
|<span data-ttu-id="e4c04-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e4c04-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e4c04-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e4c04-118">Not Supported.</span></span>|
|<span data-ttu-id="e4c04-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e4c04-119">Application</span></span>| <span data-ttu-id="e4c04-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e4c04-120">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e4c04-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e4c04-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/{id}/jobs/{id}/documents/{id}/uploadData
```
## <a name="request-headers"></a><span data-ttu-id="e4c04-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e4c04-122">Request headers</span></span>
| <span data-ttu-id="e4c04-123">Имя</span><span class="sxs-lookup"><span data-stu-id="e4c04-123">Name</span></span>          | <span data-ttu-id="e4c04-124">Описание</span><span class="sxs-lookup"><span data-stu-id="e4c04-124">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="e4c04-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e4c04-125">Authorization</span></span> | <span data-ttu-id="e4c04-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e4c04-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e4c04-128">Range</span><span class="sxs-lookup"><span data-stu-id="e4c04-128">Range</span></span> | <span data-ttu-id="e4c04-129">байт = {Стартбитеиндекс} — {Ендбитеиндекс}</span><span class="sxs-lookup"><span data-stu-id="e4c04-129">bytes={startByteIndex}-{endByteIndex}‬</span></span>  |
| <span data-ttu-id="e4c04-130">Content-Length</span><span class="sxs-lookup"><span data-stu-id="e4c04-130">Content-Length</span></span> | <span data-ttu-id="e4c04-131">ContentLength</span><span class="sxs-lookup"><span data-stu-id="e4c04-131">{contentLength}‬</span></span>  |
| <span data-ttu-id="e4c04-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e4c04-132">Content-type</span></span>  | <span data-ttu-id="e4c04-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e4c04-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e4c04-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e4c04-135">Request body</span></span>
<span data-ttu-id="e4c04-136">Текст запроса представляет собой двоичный объект BLOB, содержащий байты документа, которые задаются в заголовке как инклюзивный диапазон байтов `Range` .</span><span class="sxs-lookup"><span data-stu-id="e4c04-136">The request body is a binary blob containing the bytes of the document that are specified as an inclusive byte range in the `Range` header.</span></span> 

## <a name="response"></a><span data-ttu-id="e4c04-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="e4c04-137">Response</span></span>
<span data-ttu-id="e4c04-138">В случае успешного выполнения этот метод возвращает один из следующих ответов.</span><span class="sxs-lookup"><span data-stu-id="e4c04-138">If successful, this method returns one of the following responses.</span></span> <span data-ttu-id="e4c04-139">В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="e4c04-139">It does not return anything in the response body.</span></span>

| <span data-ttu-id="e4c04-140">Condition</span><span class="sxs-lookup"><span data-stu-id="e4c04-140">Condition</span></span>     | <span data-ttu-id="e4c04-141">Код ответа</span><span class="sxs-lookup"><span data-stu-id="e4c04-141">Response code</span></span> |
|:--------------|:--------------|
| <span data-ttu-id="e4c04-142">Один или несколько двоичных сегментов по-прежнему необходимо отправить</span><span class="sxs-lookup"><span data-stu-id="e4c04-142">One or more binary segments still need to be uploaded</span></span> | `202 Accepted` |
| <span data-ttu-id="e4c04-143">Все двоичные сегменты успешно отправлены</span><span class="sxs-lookup"><span data-stu-id="e4c04-143">All binary segments have been uploaded successfully</span></span> | `201 Created` |

## <a name="example"></a><span data-ttu-id="e4c04-144">Пример</span><span class="sxs-lookup"><span data-stu-id="e4c04-144">Example</span></span>
<span data-ttu-id="e4c04-145">В приведенном ниже примере показано, как вызвать этот API, чтобы отправить первые 72797 байтов документа.</span><span class="sxs-lookup"><span data-stu-id="e4c04-145">The following example shows how to call this API to upload the first 72797 bytes of a document.</span></span>
##### <a name="request"></a><span data-ttu-id="e4c04-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="e4c04-146">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="e4c04-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="e4c04-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "printdocument-uploaddata"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/{id}/jobs/{id}/documents/{id}/uploadData
Range: bytes=0-72796
Content-Length: 72797
```
# <a name="c"></a>[<span data-ttu-id="e4c04-148">C#</span><span class="sxs-lookup"><span data-stu-id="e4c04-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/printdocument-uploaddata-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e4c04-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e4c04-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/printdocument-uploaddata-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e4c04-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e4c04-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/printdocument-uploaddata-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e4c04-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="e4c04-151">Response</span></span>

<span data-ttu-id="e4c04-152">Отсутствует один или несколько сегментов:</span><span class="sxs-lookup"><span data-stu-id="e4c04-152">One or more segments missing:</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printDocument"
} -->
```http
HTTP/1.1 202 Accepted
```

<span data-ttu-id="e4c04-153">Все принимаемые сегменты:</span><span class="sxs-lookup"><span data-stu-id="e4c04-153">All segments received:</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printDocument"
} -->
```http
HTTP/1.1 201 Created
```


