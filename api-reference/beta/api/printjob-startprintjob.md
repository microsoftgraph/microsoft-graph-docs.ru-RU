---
title: 'printJob: Стартпринтжоб'
description: Отправит задание печати на связанный принтер. Оно будет напечатано после выполнения всех ожидающих заданий, прерванных или отмененных.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: a5c558be384fcecad72e08e9d8aa45b0b397da06
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/21/2020
ms.locfileid: "42896203"
---
# <a name="printjob-startprintjob"></a><span data-ttu-id="bb1f3-104">printJob: Стартпринтжоб</span><span class="sxs-lookup"><span data-stu-id="bb1f3-104">printJob: startPrintJob</span></span>

<span data-ttu-id="bb1f3-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bb1f3-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bb1f3-106">Отправит задание печати на связанный [принтер](../resources/printer.md).</span><span class="sxs-lookup"><span data-stu-id="bb1f3-106">Submits the print job to the associated [printer](../resources/printer.md).</span></span> <span data-ttu-id="bb1f3-107">Оно будет напечатано после выполнения всех ожидающих **заданий** , прерванных или отмененных.</span><span class="sxs-lookup"><span data-stu-id="bb1f3-107">It will be printed after any existing pending **jobs** are completed, aborted, or canceled.</span></span>

## <a name="permissions"></a><span data-ttu-id="bb1f3-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bb1f3-108">Permissions</span></span>
<span data-ttu-id="bb1f3-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bb1f3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="bb1f3-111">В дополнение к следующим разрешениям клиент пользователя должен иметь активную универсальную подписку на печать.</span><span class="sxs-lookup"><span data-stu-id="bb1f3-111">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="bb1f3-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bb1f3-112">Permission type</span></span> | <span data-ttu-id="bb1f3-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bb1f3-113">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="bb1f3-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bb1f3-114">Delegated (work or school account)</span></span>| <span data-ttu-id="bb1f3-115">Users. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="bb1f3-115">Users.Read.All</span></span> |
|<span data-ttu-id="bb1f3-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bb1f3-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bb1f3-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb1f3-117">Not Supported.</span></span>|
|<span data-ttu-id="bb1f3-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bb1f3-118">Application</span></span>|<span data-ttu-id="bb1f3-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb1f3-119">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bb1f3-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bb1f3-120">HTTP request</span></span>
```http
POST /print/printers/{id}/jobs/{id}/startPrintJob
```
## <a name="request-headers"></a><span data-ttu-id="bb1f3-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bb1f3-121">Request headers</span></span>
| <span data-ttu-id="bb1f3-122">Имя</span><span class="sxs-lookup"><span data-stu-id="bb1f3-122">Name</span></span>          | <span data-ttu-id="bb1f3-123">Описание</span><span class="sxs-lookup"><span data-stu-id="bb1f3-123">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="bb1f3-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bb1f3-124">Authorization</span></span> | <span data-ttu-id="bb1f3-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bb1f3-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bb1f3-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="bb1f3-127">Request body</span></span>

<span data-ttu-id="bb1f3-128">Не отправляйте текст запроса для этого Месо.</span><span class="sxs-lookup"><span data-stu-id="bb1f3-128">Do not submit a request body for this metho.</span></span> 

## <a name="response"></a><span data-ttu-id="bb1f3-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="bb1f3-129">Response</span></span>
<span data-ttu-id="bb1f3-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [принтжобстатус](../resources/printjobstatus.md) в теле.</span><span class="sxs-lookup"><span data-stu-id="bb1f3-130">If successful, this method returns a `200 OK` response code and a [printJobStatus](../resources/printjobstatus.md) object in the body.</span></span>

## <a name="example"></a><span data-ttu-id="bb1f3-131">Пример</span><span class="sxs-lookup"><span data-stu-id="bb1f3-131">Example</span></span>
<span data-ttu-id="bb1f3-132">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="bb1f3-132">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="bb1f3-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="bb1f3-133">Request</span></span>

```http
POST https://graph.microsoft.com/beta/print/printers/{id}/jobs/{id}/startPrintJob
```

##### <a name="response"></a><span data-ttu-id="bb1f3-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="bb1f3-134">Response</span></span>
<span data-ttu-id="bb1f3-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bb1f3-135">The following is an example of the response.</span></span> 
><span data-ttu-id="bb1f3-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bb1f3-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK

{
    "processingState": "processing",
    "processingStateDescription": "The print job is currently being processed.",
    "acquiredByPrinter": false
}
```
