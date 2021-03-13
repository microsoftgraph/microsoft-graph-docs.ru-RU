---
title: 'printJob: начните'
description: Отправка задания печати на связанный принтер или принтерShare. Она будет напечатана после завершения, отмены или отмены существующих ожидающих заданий.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: dd264c395538ee3d77fe22829edca27a6d7ad4b1
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50775922"
---
# <a name="printjob-start"></a><span data-ttu-id="86941-104">printJob: начните</span><span class="sxs-lookup"><span data-stu-id="86941-104">printJob: start</span></span>
<span data-ttu-id="86941-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="86941-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="86941-106">Отправка задания печати на [связанный](../resources/printer.md) принтер или [принтерShare](../resources/printershare.md).</span><span class="sxs-lookup"><span data-stu-id="86941-106">Submits the print job to the associated [printer](../resources/printer.md) or [printerShare](../resources/printershare.md).</span></span> <span data-ttu-id="86941-107">Он будет напечатан после завершения, отмены или отмены существующих ожидающих заданий. </span><span class="sxs-lookup"><span data-stu-id="86941-107">It will be printed after any existing pending **jobs** are completed, aborted, or canceled.</span></span>

## <a name="permissions"></a><span data-ttu-id="86941-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="86941-108">Permissions</span></span>
<span data-ttu-id="86941-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="86941-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="86941-111">Помимо следующих разрешений, клиент пользователя или приложения должен иметь активную подписку на универсальную печать и иметь разрешение, которое предоставляет [get printer](printer-get.md) или Get printerShare в зависимости от того, используется принтер или [принтерShare.](printershare-get.md)</span><span class="sxs-lookup"><span data-stu-id="86941-111">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants [Get printer](printer-get.md) or [Get printerShare](printershare-get.md) depending upon whether printer or printerShare is being used.</span></span>

|<span data-ttu-id="86941-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="86941-112">Permission type</span></span> | <span data-ttu-id="86941-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="86941-113">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="86941-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="86941-114">Delegated (work or school account)</span></span>| <span data-ttu-id="86941-115">PrintJob.Create, PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86941-115">PrintJob.Create, PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |
|<span data-ttu-id="86941-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="86941-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="86941-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="86941-117">Not Supported.</span></span>|
|<span data-ttu-id="86941-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="86941-118">Application</span></span>| <span data-ttu-id="86941-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="86941-119">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="86941-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="86941-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /print/shares/{printerShareId}/jobs/{printJobId}/start
```

## <a name="request-headers"></a><span data-ttu-id="86941-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="86941-121">Request headers</span></span>
|<span data-ttu-id="86941-122">Имя</span><span class="sxs-lookup"><span data-stu-id="86941-122">Name</span></span>|<span data-ttu-id="86941-123">Описание</span><span class="sxs-lookup"><span data-stu-id="86941-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="86941-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="86941-124">Authorization</span></span>|<span data-ttu-id="86941-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="86941-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="86941-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="86941-127">Request body</span></span>
<span data-ttu-id="86941-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="86941-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="86941-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="86941-129">Response</span></span>
<span data-ttu-id="86941-130">В случае успешной работы этот метод возвращает код отклика и `200 OK` объект [printJobStatus](../resources/printjobstatus.md) в теле.</span><span class="sxs-lookup"><span data-stu-id="86941-130">If successful, this method returns a `200 OK` response code and a [printJobStatus](../resources/printjobstatus.md) object in the body.</span></span>

## <a name="examples"></a><span data-ttu-id="86941-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="86941-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="86941-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="86941-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="86941-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="86941-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "printjob_start"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/print/shares/{printerShareId}/jobs/{printJobId}/start
```
# <a name="c"></a>[<span data-ttu-id="86941-134">C#</span><span class="sxs-lookup"><span data-stu-id="86941-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/printjob-start-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="86941-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="86941-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/printjob-start-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="86941-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="86941-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/printjob-start-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="86941-137">Java</span><span class="sxs-lookup"><span data-stu-id="86941-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/printjob-start-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="86941-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="86941-138">Response</span></span>
<span data-ttu-id="86941-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="86941-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printJobStatus"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "state": "processing",
    "description": "The print job is currently being processed.",
    "isAcquiredByPrinter": false,
    "details": ["interpreting"]
}
```

