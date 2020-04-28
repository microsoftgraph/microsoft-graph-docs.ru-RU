---
title: 'printDocument: Уплоаддата'
description: Отправьте один двоичный сегмент printDocument.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 10bf87d66126d85bdc52c69659647c7728084ac5
ms.sourcegitcommit: 9edfcf99706c8490cd5832a1c706a88a89e24db1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/07/2020
ms.locfileid: "42948102"
---
# <a name="printdocument-uploaddata"></a><span data-ttu-id="be11d-103">printDocument: Уплоаддата</span><span class="sxs-lookup"><span data-stu-id="be11d-103">printDocument: uploadData</span></span>

<span data-ttu-id="be11d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="be11d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="be11d-105">Отправьте один двоичный сегмент **printDocument**.</span><span class="sxs-lookup"><span data-stu-id="be11d-105">Upload a single binary segment of the **printDocument**.</span></span>

<span data-ttu-id="be11d-106">Вы можете отправить файл целиком или разбить его на несколько диапазонов байтов, если число запросов не превышает 1 МБ.</span><span class="sxs-lookup"><span data-stu-id="be11d-106">You can upload the entire file, or split the file into multiple byte ranges, as long as no request is larger than 1 MB.</span></span>

<span data-ttu-id="be11d-107">Сегменты файла можно отправить в любом порядке и можно отправить параллельно, используя до четырех одновременных запросов.</span><span class="sxs-lookup"><span data-stu-id="be11d-107">The segments of the file can be uploaded in any order and can be uploaded in parallel, with up to four concurrent requests.</span></span> <span data-ttu-id="be11d-108">После отправки всех двоичных сегментов документа двоичный файл связывается с **методом printJob**.</span><span class="sxs-lookup"><span data-stu-id="be11d-108">When all the binary segments of document are uploaded, the binary file is linked to the **printJob**.</span></span>

## <a name="permissions"></a><span data-ttu-id="be11d-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="be11d-109">Permissions</span></span>
<span data-ttu-id="be11d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be11d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="be11d-112">В дополнение к следующим разрешениям клиент пользователя должен иметь активную универсальную подписку на печать.</span><span class="sxs-lookup"><span data-stu-id="be11d-112">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="be11d-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="be11d-113">Permission type</span></span> | <span data-ttu-id="be11d-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="be11d-114">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="be11d-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="be11d-115">Delegated (work or school account)</span></span>| <span data-ttu-id="be11d-116">Users. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="be11d-116">Users.Read.All</span></span> |
|<span data-ttu-id="be11d-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="be11d-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="be11d-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be11d-118">Not Supported.</span></span>|
|<span data-ttu-id="be11d-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="be11d-119">Application</span></span>|<span data-ttu-id="be11d-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be11d-120">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="be11d-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="be11d-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/{id}/jobs/{id}/documents/{id}/uploadData
```
## <a name="request-headers"></a><span data-ttu-id="be11d-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="be11d-122">Request headers</span></span>
| <span data-ttu-id="be11d-123">Имя</span><span class="sxs-lookup"><span data-stu-id="be11d-123">Name</span></span>          | <span data-ttu-id="be11d-124">Описание</span><span class="sxs-lookup"><span data-stu-id="be11d-124">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="be11d-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="be11d-125">Authorization</span></span> | <span data-ttu-id="be11d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="be11d-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="be11d-128">Диапазон</span><span class="sxs-lookup"><span data-stu-id="be11d-128">Range</span></span> | <span data-ttu-id="be11d-129">байт = {Стартбитеиндекс} — {Ендбитеиндекс}</span><span class="sxs-lookup"><span data-stu-id="be11d-129">bytes={startByteIndex}-{endByteIndex}‬</span></span>  |
| <span data-ttu-id="be11d-130">Content-Length</span><span class="sxs-lookup"><span data-stu-id="be11d-130">Content-Length</span></span> | <span data-ttu-id="be11d-131">ContentLength</span><span class="sxs-lookup"><span data-stu-id="be11d-131">{contentLength}‬</span></span>  |
| <span data-ttu-id="be11d-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="be11d-132">Content-type</span></span>  | <span data-ttu-id="be11d-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="be11d-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="be11d-135">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="be11d-135">Request body</span></span>
<span data-ttu-id="be11d-136">Текст запроса представляет собой двоичный объект BLOB, содержащий байты документа, которые задаются в `Range` заголовке как инклюзивный диапазон байтов.</span><span class="sxs-lookup"><span data-stu-id="be11d-136">The request body is a binary blob containing the bytes of the document that are specified as an inclusive byte range in the `Range` header.</span></span> 

## <a name="response"></a><span data-ttu-id="be11d-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="be11d-137">Response</span></span>
<span data-ttu-id="be11d-138">В случае успешного выполнения этот метод возвращает один из следующих ответов.</span><span class="sxs-lookup"><span data-stu-id="be11d-138">If successful, this method returns one of the following responses.</span></span> <span data-ttu-id="be11d-139">В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="be11d-139">It does not return anything in the response body.</span></span>

| <span data-ttu-id="be11d-140">Условие</span><span class="sxs-lookup"><span data-stu-id="be11d-140">Condition</span></span>     | <span data-ttu-id="be11d-141">Код ответа</span><span class="sxs-lookup"><span data-stu-id="be11d-141">Response code</span></span> |
|:--------------|:--------------|
| <span data-ttu-id="be11d-142">Один или несколько двоичных сегментов по-прежнему необходимо отправить</span><span class="sxs-lookup"><span data-stu-id="be11d-142">One or more binary segments still need to be uploaded</span></span> | `202 Accepted` |
| <span data-ttu-id="be11d-143">Все двоичные сегменты успешно отправлены</span><span class="sxs-lookup"><span data-stu-id="be11d-143">All binary segments have been uploaded successfully</span></span> | `201 Created` |

## <a name="example"></a><span data-ttu-id="be11d-144">Пример</span><span class="sxs-lookup"><span data-stu-id="be11d-144">Example</span></span>
<span data-ttu-id="be11d-145">В приведенном ниже примере показано, как вызвать этот API, чтобы отправить первые 72797 байтов документа.</span><span class="sxs-lookup"><span data-stu-id="be11d-145">The following example shows how to call this API to upload the first 72797 bytes of a document.</span></span>
##### <a name="request"></a><span data-ttu-id="be11d-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="be11d-146">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="be11d-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="be11d-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "printdocument-uploaddata"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/{id}/jobs/{id}/documents/{id}/uploadData
Range: bytes=0-72796
Content-Length: 72797
```
# <a name="c"></a>[<span data-ttu-id="be11d-148">C#</span><span class="sxs-lookup"><span data-stu-id="be11d-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/printdocument-uploaddata-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="be11d-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="be11d-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/printdocument-uploaddata-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="be11d-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="be11d-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/printdocument-uploaddata-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="be11d-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="be11d-151">Response</span></span>

<span data-ttu-id="be11d-152">Отсутствует один или несколько сегментов:</span><span class="sxs-lookup"><span data-stu-id="be11d-152">One or more segments missing:</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printDocument"
} -->
```http
HTTP/1.1 202 Accepted
```

<span data-ttu-id="be11d-153">Все принимаемые сегменты:</span><span class="sxs-lookup"><span data-stu-id="be11d-153">All segments received:</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printDocument"
} -->
```http
HTTP/1.1 201 Created
```
