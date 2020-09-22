---
title: 'printJob: redirect'
description: Перенаправление задания печати на другой принтер.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 9d0d9b4f65c8fb99c932348415109fde79370a38
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48035402"
---
# <a name="printjob-redirect"></a><span data-ttu-id="bc3cb-103">printJob: redirect</span><span class="sxs-lookup"><span data-stu-id="bc3cb-103">printJob: redirect</span></span>

<span data-ttu-id="bc3cb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bc3cb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bc3cb-105">Перенаправление [задания печати](../resources/printjob.md) на другой [принтер](../resources/printer.md).</span><span class="sxs-lookup"><span data-stu-id="bc3cb-105">Redirect a [print job](../resources/printjob.md) to a different [printer](../resources/printer.md).</span></span>

<span data-ttu-id="bc3cb-106">Сведения о том, как использовать этот API для добавления поддержки печати по запросу к универсальной печати, [можно узнать в статье расширение универсальной печати для поддержки печати по запросу](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span><span class="sxs-lookup"><span data-stu-id="bc3cb-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

> [!IMPORTANT]
> <span data-ttu-id="bc3cb-107">Приостановленные задания печати, которые не перенаправлены в течение 2 дней, будут удалены.</span><span class="sxs-lookup"><span data-stu-id="bc3cb-107">Paused print jobs that are not redirected within 2 days will be deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="bc3cb-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bc3cb-108">Permissions</span></span>
<span data-ttu-id="bc3cb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bc3cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="bc3cb-111">Чтобы использовать универсальную службу печати, пользователь или клиент приложения должен иметь активную универсальную подписку на печать, разрешение, предоставляющее доступ к [принтеру](printer-get.md) , а также одно из разрешений, перечисленных в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="bc3cb-111">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, a permission that grants [Get printer](printer-get.md) access, and one of the permissions listed in the following table.</span></span>

|<span data-ttu-id="bc3cb-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bc3cb-112">Permission type</span></span> | <span data-ttu-id="bc3cb-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bc3cb-113">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="bc3cb-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bc3cb-114">Delegated (work or school account)</span></span>| <span data-ttu-id="bc3cb-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc3cb-115">Not supported.</span></span> |
|<span data-ttu-id="bc3cb-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bc3cb-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bc3cb-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc3cb-117">Not Supported.</span></span>|
|<span data-ttu-id="bc3cb-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bc3cb-118">Application</span></span>| <span data-ttu-id="bc3cb-119">PrintJob.Manage.All</span><span class="sxs-lookup"><span data-stu-id="bc3cb-119">PrintJob.Manage.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bc3cb-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bc3cb-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/{id}/jobs/{id}/redirect
```
## <a name="request-headers"></a><span data-ttu-id="bc3cb-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bc3cb-121">Request headers</span></span>
| <span data-ttu-id="bc3cb-122">Имя</span><span class="sxs-lookup"><span data-stu-id="bc3cb-122">Name</span></span>          | <span data-ttu-id="bc3cb-123">Описание</span><span class="sxs-lookup"><span data-stu-id="bc3cb-123">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="bc3cb-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bc3cb-124">Authorization</span></span> | <span data-ttu-id="bc3cb-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bc3cb-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bc3cb-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bc3cb-127">Request body</span></span>
<span data-ttu-id="bc3cb-128">В тексте запроса укажите идентификатор принтера, на который необходимо перенаправить задание печати.</span><span class="sxs-lookup"><span data-stu-id="bc3cb-128">In the request body, supply the ID of the printer that the print job should be redirected to.</span></span>

| <span data-ttu-id="bc3cb-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="bc3cb-129">Property</span></span>     | <span data-ttu-id="bc3cb-130">Тип</span><span class="sxs-lookup"><span data-stu-id="bc3cb-130">Type</span></span>        | <span data-ttu-id="bc3cb-131">Описание</span><span class="sxs-lookup"><span data-stu-id="bc3cb-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="bc3cb-132">дестинатионпринтерид</span><span class="sxs-lookup"><span data-stu-id="bc3cb-132">destinationPrinterId</span></span>|<span data-ttu-id="bc3cb-133">String</span><span class="sxs-lookup"><span data-stu-id="bc3cb-133">String</span></span>|<span data-ttu-id="bc3cb-134">ИДЕНТИФИКАТОР принтера, на который необходимо перенаправить задание печати.</span><span class="sxs-lookup"><span data-stu-id="bc3cb-134">The ID of the printer the print job should be redirected to.</span></span>|

## <a name="response"></a><span data-ttu-id="bc3cb-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="bc3cb-135">Response</span></span>
<span data-ttu-id="bc3cb-136">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [printJob](../resources/printjob.md) , помещенные в очередь для конечного принтера.</span><span class="sxs-lookup"><span data-stu-id="bc3cb-136">If successful, this method returns a `200 OK` response code and a [printJob](../resources/printjob.md) object queued for the destination printer.</span></span>

## <a name="example"></a><span data-ttu-id="bc3cb-137">Пример</span><span class="sxs-lookup"><span data-stu-id="bc3cb-137">Example</span></span>
<span data-ttu-id="bc3cb-138">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="bc3cb-138">The following example shows how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="bc3cb-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="bc3cb-139">Request</span></span>
<span data-ttu-id="bc3cb-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bc3cb-140">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="bc3cb-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="bc3cb-141">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="bc3cb-142">C#</span><span class="sxs-lookup"><span data-stu-id="bc3cb-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/printjob-redirect-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bc3cb-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bc3cb-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/printjob-redirect-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bc3cb-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bc3cb-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/printjob-redirect-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="bc3cb-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="bc3cb-145">Response</span></span>
<span data-ttu-id="bc3cb-146">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="bc3cb-146">The following is an example of the response.</span></span> 
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


