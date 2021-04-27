---
title: Список printJobs для принтераShare
description: Извлечение списка заданий печати, связанных с совместной печатью.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: a7453677550e974536de20b6ad2b054d2040990e
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52037461"
---
# <a name="list-printjobs-for-a-printershare"></a><span data-ttu-id="e9dc3-103">Список printJobs для принтераShare</span><span class="sxs-lookup"><span data-stu-id="e9dc3-103">List printJobs for a printerShare</span></span>

<span data-ttu-id="e9dc3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e9dc3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e9dc3-105">Извлечение списка заданий печати, связанных с [принтеромShare.](../resources/printershare.md)</span><span class="sxs-lookup"><span data-stu-id="e9dc3-105">Retrieve a list of print jobs associated with the [printerShare](../resources/printershare.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e9dc3-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e9dc3-106">Permissions</span></span>
<span data-ttu-id="e9dc3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e9dc3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="e9dc3-109">Чтобы использовать службу универсальной печати, клиент пользователя или приложения должен иметь активную подписку на универсальную печать, разрешение, предоставляемую доступ [к принтеру Get PrinterShare,](printershare-get.md) и одно из разрешений, перечисленных в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="e9dc3-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, a permission that grants [Get printerShare](printershare-get.md) access, and one of the permissions listed in the following table.</span></span> 

<span data-ttu-id="e9dc3-110">Чтобы прочитать задания печати у другого пользователя, пользователь должен быть администратором печати и иметь разрешение PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic.All или PrintJob.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="e9dc3-110">To read print jobs from another user, the signed in user needs to be a print administrator and have the PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic.All, or PrintJob.ReadWrite.All permission.</span></span>

|<span data-ttu-id="e9dc3-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e9dc3-111">Permission type</span></span> | <span data-ttu-id="e9dc3-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e9dc3-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="e9dc3-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e9dc3-113">Delegated (work or school account)</span></span>| <span data-ttu-id="e9dc3-114">PrintJob.ReadBasic, PrintJob.Read, PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9dc3-114">PrintJob.ReadBasic, PrintJob.Read, PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |
|<span data-ttu-id="e9dc3-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e9dc3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e9dc3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e9dc3-116">Not Supported.</span></span>|
|<span data-ttu-id="e9dc3-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e9dc3-117">Application</span></span>| <span data-ttu-id="e9dc3-118">PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9dc3-118">PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e9dc3-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e9dc3-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/shares/{id}/jobs
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e9dc3-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e9dc3-120">Optional query parameters</span></span>
<span data-ttu-id="e9dc3-121">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="e9dc3-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="e9dc3-122">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="e9dc3-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

* <span data-ttu-id="e9dc3-123">Свойство **documents** по умолчанию опущено из ответа.</span><span class="sxs-lookup"><span data-stu-id="e9dc3-123">The **documents** property is omitted from the response by default.</span></span> <span data-ttu-id="e9dc3-124">Чтобы также вернуть список [печатных документов](../resources/printdocument.md) для каждого задания печати, используйте `$expand=documents` .</span><span class="sxs-lookup"><span data-stu-id="e9dc3-124">To also return a list of [printDocuments](../resources/printdocument.md) for each print job, use `$expand=documents`.</span></span>
* <span data-ttu-id="e9dc3-125">Этот метод поддерживает фильтрацию заданий печати пользователем, который их создал.</span><span class="sxs-lookup"><span data-stu-id="e9dc3-125">This method supports filtering print jobs by the user who created them.</span></span> <span data-ttu-id="e9dc3-126">Используйте `$filter=createdBy/userPrincipalName eq '{upn}'` , **где {upn}** — это [основное имя](/azure/active-directory/hybrid/plan-connect-userprincipalname#what-is-userprincipalname) пользователя связанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="e9dc3-126">Use `$filter=createdBy/userPrincipalName eq '{upn}'`, where **{upn}** is the [user principal name](/azure/active-directory/hybrid/plan-connect-userprincipalname#what-is-userprincipalname) of the associated user.</span></span>

### <a name="exceptions"></a><span data-ttu-id="e9dc3-127">Exceptions</span><span class="sxs-lookup"><span data-stu-id="e9dc3-127">Exceptions</span></span>
<span data-ttu-id="e9dc3-128">Некоторые операторы не поддерживаются: `$count` , `$search` .</span><span class="sxs-lookup"><span data-stu-id="e9dc3-128">Some operators are not supported: `$count`, `$search`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e9dc3-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e9dc3-129">Request headers</span></span>
| <span data-ttu-id="e9dc3-130">Имя</span><span class="sxs-lookup"><span data-stu-id="e9dc3-130">Name</span></span>      |<span data-ttu-id="e9dc3-131">Описание</span><span class="sxs-lookup"><span data-stu-id="e9dc3-131">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e9dc3-132">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e9dc3-132">Authorization</span></span> | <span data-ttu-id="e9dc3-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e9dc3-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e9dc3-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e9dc3-135">Request body</span></span>
<span data-ttu-id="e9dc3-136">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e9dc3-136">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="e9dc3-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="e9dc3-137">Response</span></span>
<span data-ttu-id="e9dc3-138">В случае успешной работы этот метод возвращает код ответа и `200 OK` коллекцию [объектов printJob](../resources/printjob.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e9dc3-138">If successful, this method returns a `200 OK` response code and collection of [printJob](../resources/printjob.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e9dc3-139">Пример</span><span class="sxs-lookup"><span data-stu-id="e9dc3-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="e9dc3-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="e9dc3-140">Request</span></span>
<span data-ttu-id="e9dc3-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e9dc3-141">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e9dc3-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="e9dc3-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_jobs_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/shares/{id}/jobs
```
# <a name="c"></a>[<span data-ttu-id="e9dc3-143">C#</span><span class="sxs-lookup"><span data-stu-id="e9dc3-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-jobs-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e9dc3-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e9dc3-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-jobs-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e9dc3-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e9dc3-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-jobs-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e9dc3-146">Java</span><span class="sxs-lookup"><span data-stu-id="e9dc3-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-jobs-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---

### <a name="response"></a><span data-ttu-id="e9dc3-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="e9dc3-147">Response</span></span>
<span data-ttu-id="e9dc3-148">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="e9dc3-148">The following is an example of the response.</span></span>
><span data-ttu-id="e9dc3-149">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e9dc3-149">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printJob",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 461

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/shares('f37141d9-0afb-484f-96d3-0ef0a679e6c1')/jobs",
  "value": [
    {
      "id": "103",
      "createdDateTime": "2020-02-04T00:00:00.0000000Z",
      "createdBy": {},
      "status": {
        "state": "completed",
        "description": "The print job has completed successfully and no further processing will take place.",
        "details" : [],
        "isAcquiredByPrinter": true
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List jobs",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
