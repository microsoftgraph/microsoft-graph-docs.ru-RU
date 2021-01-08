---
title: 'printJob: start'
description: Отправка задания печати на связанный принтер или printerShare. Он будет печататься после завершения всех ожидающих заданий, отмены или отмены.
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: d2cb4a5413d592d170e31a882be93d900deca8c1
ms.sourcegitcommit: a0a5690ad9c109149e0b8c8baba164648ff5c226
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/08/2021
ms.locfileid: "49784802"
---
# <a name="printjob-start"></a><span data-ttu-id="9e001-104">printJob: start</span><span class="sxs-lookup"><span data-stu-id="9e001-104">printJob: start</span></span>

<span data-ttu-id="9e001-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9e001-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9e001-106">Отправка задания печати на связанный [принтер](../resources/printer.md) или [printerShare.](../resources/printershare.md)</span><span class="sxs-lookup"><span data-stu-id="9e001-106">Submits the print job to the associated [printer](../resources/printer.md) or [printerShare](../resources/printershare.md).</span></span> <span data-ttu-id="9e001-107">Он будет печататься после  завершения, отмены или отмены всех ожидающих заданий.</span><span class="sxs-lookup"><span data-stu-id="9e001-107">It will be printed after any existing pending **jobs** are completed, aborted, or canceled.</span></span>

## <a name="permissions"></a><span data-ttu-id="9e001-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9e001-108">Permissions</span></span>
<span data-ttu-id="9e001-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9e001-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="9e001-111">Помимо следующих разрешений, у пользователя или клиента приложения должна быть активная подписка [](printer-get.md) универсальной печати и разрешение на получение принтера или [get printerShare](printershare-get.md) в зависимости от того, используется ли принтер или printerShare.</span><span class="sxs-lookup"><span data-stu-id="9e001-111">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants [Get printer](printer-get.md) or [Get printerShare](printershare-get.md) depending upon whether printer or printerShare is being used.</span></span>

|<span data-ttu-id="9e001-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9e001-112">Permission type</span></span> | <span data-ttu-id="9e001-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9e001-113">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="9e001-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9e001-114">Delegated (work or school account)</span></span>| <span data-ttu-id="9e001-115">PrintJob.Create, PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e001-115">PrintJob.Create, PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |
|<span data-ttu-id="9e001-116">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9e001-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9e001-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9e001-117">Not Supported.</span></span>|
|<span data-ttu-id="9e001-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="9e001-118">Application</span></span>| <span data-ttu-id="9e001-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9e001-119">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9e001-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9e001-120">HTTP request</span></span>
```http
POST /print/shares/{id}/jobs/{id}/start
```
## <a name="request-headers"></a><span data-ttu-id="9e001-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9e001-121">Request headers</span></span>
| <span data-ttu-id="9e001-122">Имя</span><span class="sxs-lookup"><span data-stu-id="9e001-122">Name</span></span>          | <span data-ttu-id="9e001-123">Описание</span><span class="sxs-lookup"><span data-stu-id="9e001-123">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="9e001-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9e001-124">Authorization</span></span> | <span data-ttu-id="9e001-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9e001-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9e001-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9e001-127">Request body</span></span>

<span data-ttu-id="9e001-128">Не отправлять тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9e001-128">Do not submit a request body for this method.</span></span> 

## <a name="response"></a><span data-ttu-id="9e001-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="9e001-129">Response</span></span>
<span data-ttu-id="9e001-130">В случае успеха этот метод возвращает код отклика и объект `200 OK` [printJobStatus](../resources/printjobstatus.md) в теле.</span><span class="sxs-lookup"><span data-stu-id="9e001-130">If successful, this method returns a `200 OK` response code and a [printJobStatus](../resources/printjobstatus.md) object in the body.</span></span>

## <a name="example"></a><span data-ttu-id="9e001-131">Пример</span><span class="sxs-lookup"><span data-stu-id="9e001-131">Example</span></span>
<span data-ttu-id="9e001-132">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="9e001-132">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9e001-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="9e001-133">Request</span></span>

```http
POST https://graph.microsoft.com/beta/print/shares/{id}/jobs/{id}/start
```

##### <a name="response"></a><span data-ttu-id="9e001-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="9e001-134">Response</span></span>
<span data-ttu-id="9e001-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9e001-135">The following is an example of the response.</span></span> 
><span data-ttu-id="9e001-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9e001-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK

{
    "state": "processing",
    "description": "The print job is currently being processed.",
    "isAcquiredByPrinter": false,
    "details": ["interpreting"]
}
```


