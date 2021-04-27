---
title: 'printJob: начните'
description: Отправка задания печати на связанный принтер или принтерShare. Она будет напечатана после завершения, отмены или отмены существующих ожидающих заданий.
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 288e3b8cfcd1458f7d71c8fb43ae57ac97237e56
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049879"
---
# <a name="printjob-start"></a><span data-ttu-id="9a561-104">printJob: начните</span><span class="sxs-lookup"><span data-stu-id="9a561-104">printJob: start</span></span>

<span data-ttu-id="9a561-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9a561-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9a561-106">Отправка задания печати на [связанный](../resources/printer.md) принтер или [принтерShare](../resources/printershare.md).</span><span class="sxs-lookup"><span data-stu-id="9a561-106">Submits the print job to the associated [printer](../resources/printer.md) or [printerShare](../resources/printershare.md).</span></span> <span data-ttu-id="9a561-107">Он будет напечатан после завершения, отмены или отмены существующих ожидающих заданий. </span><span class="sxs-lookup"><span data-stu-id="9a561-107">It will be printed after any existing pending **jobs** are completed, aborted, or canceled.</span></span>

## <a name="permissions"></a><span data-ttu-id="9a561-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9a561-108">Permissions</span></span>
<span data-ttu-id="9a561-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9a561-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="9a561-111">Помимо следующих разрешений, клиент пользователя или приложения должен иметь активную подписку на универсальную печать и иметь разрешение, которое предоставляет [get printer](printer-get.md) или Get printerShare в зависимости от того, используется принтер или [принтерShare.](printershare-get.md)</span><span class="sxs-lookup"><span data-stu-id="9a561-111">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants [Get printer](printer-get.md) or [Get printerShare](printershare-get.md) depending upon whether printer or printerShare is being used.</span></span>

|<span data-ttu-id="9a561-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9a561-112">Permission type</span></span> | <span data-ttu-id="9a561-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9a561-113">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="9a561-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9a561-114">Delegated (work or school account)</span></span>| <span data-ttu-id="9a561-115">PrintJob.Create, PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a561-115">PrintJob.Create, PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |
|<span data-ttu-id="9a561-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9a561-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9a561-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9a561-117">Not Supported.</span></span>|
|<span data-ttu-id="9a561-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="9a561-118">Application</span></span>| <span data-ttu-id="9a561-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9a561-119">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9a561-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9a561-120">HTTP request</span></span>
```http
POST /print/shares/{id}/jobs/{id}/start
```
## <a name="request-headers"></a><span data-ttu-id="9a561-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9a561-121">Request headers</span></span>
| <span data-ttu-id="9a561-122">Имя</span><span class="sxs-lookup"><span data-stu-id="9a561-122">Name</span></span>          | <span data-ttu-id="9a561-123">Описание</span><span class="sxs-lookup"><span data-stu-id="9a561-123">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="9a561-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9a561-124">Authorization</span></span> | <span data-ttu-id="9a561-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9a561-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9a561-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9a561-127">Request body</span></span>

<span data-ttu-id="9a561-128">Не отправлять тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9a561-128">Do not submit a request body for this method.</span></span> 

## <a name="response"></a><span data-ttu-id="9a561-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="9a561-129">Response</span></span>
<span data-ttu-id="9a561-130">В случае успешной работы этот метод возвращает код отклика и `200 OK` объект [printJobStatus](../resources/printjobstatus.md) в теле.</span><span class="sxs-lookup"><span data-stu-id="9a561-130">If successful, this method returns a `200 OK` response code and a [printJobStatus](../resources/printjobstatus.md) object in the body.</span></span>

## <a name="example"></a><span data-ttu-id="9a561-131">Пример</span><span class="sxs-lookup"><span data-stu-id="9a561-131">Example</span></span>
<span data-ttu-id="9a561-132">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="9a561-132">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9a561-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="9a561-133">Request</span></span>

```http
POST https://graph.microsoft.com/beta/print/shares/{id}/jobs/{id}/start
```

##### <a name="response"></a><span data-ttu-id="9a561-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="9a561-134">Response</span></span>
<span data-ttu-id="9a561-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="9a561-135">The following is an example of the response.</span></span> 
><span data-ttu-id="9a561-136">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="9a561-136">**Note:** The response object shown here might be shortened for readability.</span></span>

```http
HTTP/1.1 200 OK

{
    "state": "processing",
    "description": "The print job is currently being processed.",
    "isAcquiredByPrinter": false,
    "details": ["interpreting"]
}
```


