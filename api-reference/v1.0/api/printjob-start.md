---
title: 'printJob: начните'
description: Отправка задания печати на связанный принтер или принтерShare. Она будет напечатана после завершения, отмены или отмены существующих ожидающих заданий.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 187e62e1de9f380f651433596b7d76fd91161c2c
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50518024"
---
# <a name="printjob-start"></a><span data-ttu-id="abd04-104">printJob: начните</span><span class="sxs-lookup"><span data-stu-id="abd04-104">printJob: start</span></span>
<span data-ttu-id="abd04-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="abd04-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="abd04-106">Отправка задания печати на [связанный](../resources/printer.md) принтер или [принтерShare](../resources/printershare.md).</span><span class="sxs-lookup"><span data-stu-id="abd04-106">Submits the print job to the associated [printer](../resources/printer.md) or [printerShare](../resources/printershare.md).</span></span> <span data-ttu-id="abd04-107">Он будет напечатан после завершения, отмены или отмены существующих ожидающих заданий. </span><span class="sxs-lookup"><span data-stu-id="abd04-107">It will be printed after any existing pending **jobs** are completed, aborted, or canceled.</span></span>

## <a name="permissions"></a><span data-ttu-id="abd04-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="abd04-108">Permissions</span></span>
<span data-ttu-id="abd04-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="abd04-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="abd04-111">Помимо следующих разрешений, клиент пользователя или приложения должен иметь активную подписку на универсальную печать и иметь разрешение, которое предоставляет [get printer](printer-get.md) или Get printerShare в зависимости от того, используется принтер или [принтерShare.](printershare-get.md)</span><span class="sxs-lookup"><span data-stu-id="abd04-111">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants [Get printer](printer-get.md) or [Get printerShare](printershare-get.md) depending upon whether printer or printerShare is being used.</span></span>

|<span data-ttu-id="abd04-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="abd04-112">Permission type</span></span> | <span data-ttu-id="abd04-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="abd04-113">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="abd04-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="abd04-114">Delegated (work or school account)</span></span>| <span data-ttu-id="abd04-115">PrintJob.Create, PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="abd04-115">PrintJob.Create, PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |
|<span data-ttu-id="abd04-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="abd04-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="abd04-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="abd04-117">Not Supported.</span></span>|
|<span data-ttu-id="abd04-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="abd04-118">Application</span></span>| <span data-ttu-id="abd04-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="abd04-119">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="abd04-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="abd04-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /print/shares/{printerShareId}/jobs/{printJobId}/start
```

## <a name="request-headers"></a><span data-ttu-id="abd04-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="abd04-121">Request headers</span></span>
|<span data-ttu-id="abd04-122">Имя</span><span class="sxs-lookup"><span data-stu-id="abd04-122">Name</span></span>|<span data-ttu-id="abd04-123">Описание</span><span class="sxs-lookup"><span data-stu-id="abd04-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="abd04-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="abd04-124">Authorization</span></span>|<span data-ttu-id="abd04-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="abd04-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="abd04-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="abd04-127">Request body</span></span>
<span data-ttu-id="abd04-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="abd04-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="abd04-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="abd04-129">Response</span></span>
<span data-ttu-id="abd04-130">В случае успешной работы этот метод возвращает код отклика и `200 OK` объект [printJobStatus](../resources/printjobstatus.md) в теле.</span><span class="sxs-lookup"><span data-stu-id="abd04-130">If successful, this method returns a `200 OK` response code and a [printJobStatus](../resources/printjobstatus.md) object in the body.</span></span>

## <a name="examples"></a><span data-ttu-id="abd04-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="abd04-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="abd04-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="abd04-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "printjob_start"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/print/shares/{printerShareId}/jobs/{printJobId}/start
```

### <a name="response"></a><span data-ttu-id="abd04-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="abd04-133">Response</span></span>
<span data-ttu-id="abd04-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="abd04-134">**Note:** The response object shown here might be shortened for readability.</span></span>
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

