---
title: 'printJob: перенаправление'
description: Перенаправить задание печати на другой принтер.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 2b99f9e2e6d0def97c1f2a23837f79e61b8e3341
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/16/2020
ms.locfileid: "49689367"
---
# <a name="printjob-redirect"></a><span data-ttu-id="8e707-103">printJob: перенаправление</span><span class="sxs-lookup"><span data-stu-id="8e707-103">printJob: redirect</span></span>

<span data-ttu-id="8e707-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8e707-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8e707-105">[Перенаправить задание печати](../resources/printjob.md) на другой [принтер.](../resources/printer.md)</span><span class="sxs-lookup"><span data-stu-id="8e707-105">Redirect a [print job](../resources/printjob.md) to a different [printer](../resources/printer.md).</span></span>

<span data-ttu-id="8e707-106">Дополнительные сведения о том, как использовать этот API для добавления поддержки печати потягивки в универсальную печать, см. в подразделе "Расширение универсальной печати для поддержки печати [с помощью оттягивать".](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)</span><span class="sxs-lookup"><span data-stu-id="8e707-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="8e707-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8e707-107">Permissions</span></span>
<span data-ttu-id="8e707-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e707-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="8e707-110">Чтобы использовать службу универсальной печати, у пользователя или клиента приложения должна быть [](printer-get.md) активная подписка универсальной печати, разрешение на получение доступа к принтеру и одно из разрешений, перечисленных в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="8e707-110">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, a permission that grants [Get printer](printer-get.md) access, and one of the permissions listed in the following table.</span></span>

|<span data-ttu-id="8e707-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8e707-111">Permission type</span></span> | <span data-ttu-id="8e707-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8e707-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="8e707-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8e707-113">Delegated (work or school account)</span></span>| <span data-ttu-id="8e707-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e707-114">Not supported.</span></span> |
|<span data-ttu-id="8e707-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8e707-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8e707-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e707-116">Not Supported.</span></span>|
|<span data-ttu-id="8e707-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="8e707-117">Application</span></span>| <span data-ttu-id="8e707-118">PrintJob.Manage.All</span><span class="sxs-lookup"><span data-stu-id="8e707-118">PrintJob.Manage.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8e707-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8e707-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/{id}/jobs/{id}/redirect
```
## <a name="request-headers"></a><span data-ttu-id="8e707-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8e707-120">Request headers</span></span>
| <span data-ttu-id="8e707-121">Имя</span><span class="sxs-lookup"><span data-stu-id="8e707-121">Name</span></span>          | <span data-ttu-id="8e707-122">Описание</span><span class="sxs-lookup"><span data-stu-id="8e707-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="8e707-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8e707-123">Authorization</span></span> | <span data-ttu-id="8e707-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8e707-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8e707-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8e707-126">Request body</span></span>
<span data-ttu-id="8e707-127">В теле запроса укавите ИД принтера, на который должно быть перенаправлено задание печати.</span><span class="sxs-lookup"><span data-stu-id="8e707-127">In the request body, supply the ID of the printer that the print job should be redirected to.</span></span>

| <span data-ttu-id="8e707-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="8e707-128">Property</span></span>     | <span data-ttu-id="8e707-129">Тип</span><span class="sxs-lookup"><span data-stu-id="8e707-129">Type</span></span>        | <span data-ttu-id="8e707-130">Описание</span><span class="sxs-lookup"><span data-stu-id="8e707-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8e707-131">destinationPrinterId</span><span class="sxs-lookup"><span data-stu-id="8e707-131">destinationPrinterId</span></span>|<span data-ttu-id="8e707-132">Строка</span><span class="sxs-lookup"><span data-stu-id="8e707-132">String</span></span>|<span data-ttu-id="8e707-133">ИД принтера, на который должно быть перенаправлено задание печати.</span><span class="sxs-lookup"><span data-stu-id="8e707-133">The ID of the printer the print job should be redirected to.</span></span>|
|<span data-ttu-id="8e707-134">configuration</span><span class="sxs-lookup"><span data-stu-id="8e707-134">configuration</span></span>|<span data-ttu-id="8e707-135">microsoft.graph.printJobConfiguration</span><span class="sxs-lookup"><span data-stu-id="8e707-135">microsoft.graph.printJobConfiguration</span></span>|<span data-ttu-id="8e707-136">Обновлена конфигурация задания печати.</span><span class="sxs-lookup"><span data-stu-id="8e707-136">Updated configuration of print job.</span></span>|

## <a name="response"></a><span data-ttu-id="8e707-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e707-137">Response</span></span>
<span data-ttu-id="8e707-138">В случае успеха этот метод возвращает код отклика и объект `200 OK` [printJob,](../resources/printjob.md) в очереди для принтера назначения.</span><span class="sxs-lookup"><span data-stu-id="8e707-138">If successful, this method returns a `200 OK` response code and a [printJob](../resources/printjob.md) object queued for the destination printer.</span></span>

## <a name="example"></a><span data-ttu-id="8e707-139">Пример</span><span class="sxs-lookup"><span data-stu-id="8e707-139">Example</span></span>
<span data-ttu-id="8e707-140">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="8e707-140">The following example shows how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="8e707-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="8e707-141">Request</span></span>
<span data-ttu-id="8e707-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8e707-142">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8e707-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="8e707-143">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="8e707-144">C#</span><span class="sxs-lookup"><span data-stu-id="8e707-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/printjob-redirect-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8e707-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8e707-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/printjob-redirect-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8e707-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8e707-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/printjob-redirect-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8e707-147">Java</span><span class="sxs-lookup"><span data-stu-id="8e707-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/printjob-redirect-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8e707-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e707-148">Response</span></span>
<span data-ttu-id="8e707-149">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8e707-149">The following is an example of the response.</span></span> 
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


