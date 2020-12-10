---
title: 'printJob: redirect'
description: Перенаправление задания печати на другой принтер.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: a3c09827b349b2402aeb8f1a37be64643b87d1d5
ms.sourcegitcommit: d9c167f6be71bdb4a023c5ace2733b9854c846d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2020
ms.locfileid: "49617075"
---
# <a name="printjob-redirect"></a><span data-ttu-id="cd95c-103">printJob: redirect</span><span class="sxs-lookup"><span data-stu-id="cd95c-103">printJob: redirect</span></span>

<span data-ttu-id="cd95c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cd95c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cd95c-105">Перенаправление [задания печати](../resources/printjob.md) на другой [принтер](../resources/printer.md).</span><span class="sxs-lookup"><span data-stu-id="cd95c-105">Redirect a [print job](../resources/printjob.md) to a different [printer](../resources/printer.md).</span></span>

<span data-ttu-id="cd95c-106">Сведения о том, как использовать этот API для добавления поддержки печати по запросу к универсальной печати, [можно узнать в статье расширение универсальной печати для поддержки печати по запросу](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span><span class="sxs-lookup"><span data-stu-id="cd95c-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="cd95c-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cd95c-107">Permissions</span></span>
<span data-ttu-id="cd95c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cd95c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="cd95c-110">Чтобы использовать универсальную службу печати, пользователь или клиент приложения должен иметь активную универсальную подписку на печать, разрешение, предоставляющее доступ к [принтеру](printer-get.md) , а также одно из разрешений, перечисленных в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="cd95c-110">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, a permission that grants [Get printer](printer-get.md) access, and one of the permissions listed in the following table.</span></span>

|<span data-ttu-id="cd95c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cd95c-111">Permission type</span></span> | <span data-ttu-id="cd95c-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cd95c-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="cd95c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cd95c-113">Delegated (work or school account)</span></span>| <span data-ttu-id="cd95c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cd95c-114">Not supported.</span></span> |
|<span data-ttu-id="cd95c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cd95c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cd95c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cd95c-116">Not Supported.</span></span>|
|<span data-ttu-id="cd95c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cd95c-117">Application</span></span>| <span data-ttu-id="cd95c-118">PrintJob.Manage.All</span><span class="sxs-lookup"><span data-stu-id="cd95c-118">PrintJob.Manage.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cd95c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cd95c-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/{id}/jobs/{id}/redirect
```
## <a name="request-headers"></a><span data-ttu-id="cd95c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cd95c-120">Request headers</span></span>
| <span data-ttu-id="cd95c-121">Имя</span><span class="sxs-lookup"><span data-stu-id="cd95c-121">Name</span></span>          | <span data-ttu-id="cd95c-122">Описание</span><span class="sxs-lookup"><span data-stu-id="cd95c-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="cd95c-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cd95c-123">Authorization</span></span> | <span data-ttu-id="cd95c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cd95c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cd95c-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cd95c-126">Request body</span></span>
<span data-ttu-id="cd95c-127">В тексте запроса укажите идентификатор принтера, на который необходимо перенаправить задание печати.</span><span class="sxs-lookup"><span data-stu-id="cd95c-127">In the request body, supply the ID of the printer that the print job should be redirected to.</span></span>

| <span data-ttu-id="cd95c-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="cd95c-128">Property</span></span>     | <span data-ttu-id="cd95c-129">Тип</span><span class="sxs-lookup"><span data-stu-id="cd95c-129">Type</span></span>        | <span data-ttu-id="cd95c-130">Описание</span><span class="sxs-lookup"><span data-stu-id="cd95c-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="cd95c-131">дестинатионпринтерид</span><span class="sxs-lookup"><span data-stu-id="cd95c-131">destinationPrinterId</span></span>|<span data-ttu-id="cd95c-132">String</span><span class="sxs-lookup"><span data-stu-id="cd95c-132">String</span></span>|<span data-ttu-id="cd95c-133">ИДЕНТИФИКАТОР принтера, на который необходимо перенаправить задание печати.</span><span class="sxs-lookup"><span data-stu-id="cd95c-133">The ID of the printer the print job should be redirected to.</span></span>|
|<span data-ttu-id="cd95c-134">configuration</span><span class="sxs-lookup"><span data-stu-id="cd95c-134">configuration</span></span>|<span data-ttu-id="cd95c-135">Microsoft. Graph. Принтжобконфигуратион</span><span class="sxs-lookup"><span data-stu-id="cd95c-135">microsoft.graph.printJobConfiguration</span></span>|<span data-ttu-id="cd95c-136">Обновлена конфигурация задания печати.</span><span class="sxs-lookup"><span data-stu-id="cd95c-136">Updated configuration of print job.</span></span>|

## <a name="response"></a><span data-ttu-id="cd95c-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="cd95c-137">Response</span></span>
<span data-ttu-id="cd95c-138">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [printJob](../resources/printjob.md) , помещенные в очередь для конечного принтера.</span><span class="sxs-lookup"><span data-stu-id="cd95c-138">If successful, this method returns a `200 OK` response code and a [printJob](../resources/printjob.md) object queued for the destination printer.</span></span>

## <a name="example"></a><span data-ttu-id="cd95c-139">Пример</span><span class="sxs-lookup"><span data-stu-id="cd95c-139">Example</span></span>
<span data-ttu-id="cd95c-140">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="cd95c-140">The following example shows how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="cd95c-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="cd95c-141">Request</span></span>
<span data-ttu-id="cd95c-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cd95c-142">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "printjob-redirect"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/d5ef6ec4-07ca-4212-baf9-d45be126bfbb/jobs/44353/redirect

{
  "destinationPrinterId": "9a3b3956-ce5b-4d06-a605-5b0bd3e9ddea"
}
```

### <a name="response"></a><span data-ttu-id="cd95c-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="cd95c-143">Response</span></span>
<span data-ttu-id="cd95c-144">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="cd95c-144">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printJob"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 437

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#printJob",
  "@odata.type": "#microsoft.graph.printJob",
  "id": "44354",
  "createdDateTime": "2020-06-30T17:19:09Z",
  "createdBy": {
    "id": "",
    "displayName": "",
    "userPrincipalName": ""
  },
  "status": {
    "processingState": "processing",
    "processingStateDescription": "The print job is currently being processed by the printer."
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printJob: redirect",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


