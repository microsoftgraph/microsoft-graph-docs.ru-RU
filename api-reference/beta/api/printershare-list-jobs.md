---
title: Список printJobs для принтераShare
description: Извлечение списка заданий печати, связанных с совместной печатью.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 7a2c7969a5900410eeb195025391c4b3b413ce26
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50950690"
---
# <a name="list-printjobs-for-a-printershare"></a><span data-ttu-id="c6bdb-103">Список printJobs для принтераShare</span><span class="sxs-lookup"><span data-stu-id="c6bdb-103">List printJobs for a printerShare</span></span>

<span data-ttu-id="c6bdb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c6bdb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c6bdb-105">Извлечение списка заданий печати, связанных с [принтеромShare.](../resources/printershare.md)</span><span class="sxs-lookup"><span data-stu-id="c6bdb-105">Retrieve a list of print jobs associated with the [printerShare](../resources/printershare.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c6bdb-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c6bdb-106">Permissions</span></span>
<span data-ttu-id="c6bdb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c6bdb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="c6bdb-109">Чтобы использовать службу универсальной печати, клиент пользователя или приложения должен иметь активную подписку на универсальную печать, разрешение, предоставляемую доступ [к принтеру Get PrinterShare,](printershare-get.md) и одно из разрешений, перечисленных в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="c6bdb-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, a permission that grants [Get printerShare](printershare-get.md) access, and one of the permissions listed in the following table.</span></span> <span data-ttu-id="c6bdb-110">Подписанный пользователем должен быть [администратором принтера.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="c6bdb-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

<span data-ttu-id="c6bdb-111">Чтобы прочитать задания печати у другого пользователя, пользователь должен быть администратором печати и иметь разрешение PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic.All или PrintJob.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="c6bdb-111">To read print jobs from another user, the signed in user needs to be a print administrator and have the PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic.All, or PrintJob.ReadWrite.All permission.</span></span>

|<span data-ttu-id="c6bdb-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c6bdb-112">Permission type</span></span> | <span data-ttu-id="c6bdb-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c6bdb-113">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="c6bdb-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c6bdb-114">Delegated (work or school account)</span></span>| <span data-ttu-id="c6bdb-115">PrintJob.ReadBasic, PrintJob.Read, PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6bdb-115">PrintJob.ReadBasic, PrintJob.Read, PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |
|<span data-ttu-id="c6bdb-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c6bdb-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c6bdb-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c6bdb-117">Not Supported.</span></span>|
|<span data-ttu-id="c6bdb-118">Application</span><span class="sxs-lookup"><span data-stu-id="c6bdb-118">Application</span></span>| <span data-ttu-id="c6bdb-119">PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6bdb-119">PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c6bdb-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c6bdb-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/shares/{id}/jobs
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c6bdb-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c6bdb-121">Optional query parameters</span></span>
<span data-ttu-id="c6bdb-122">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="c6bdb-122">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="c6bdb-123">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="c6bdb-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

* <span data-ttu-id="c6bdb-124">Свойство **documents** по умолчанию опущено из ответа.</span><span class="sxs-lookup"><span data-stu-id="c6bdb-124">The **documents** property is omitted from the response by default.</span></span> <span data-ttu-id="c6bdb-125">Чтобы также вернуть список [печатных документов](../resources/printdocument.md) для каждого задания печати, используйте `$expand=documents` .</span><span class="sxs-lookup"><span data-stu-id="c6bdb-125">To also return a list of [printDocuments](../resources/printdocument.md) for each print job, use `$expand=documents`.</span></span>
* <span data-ttu-id="c6bdb-126">Этот метод поддерживает фильтрацию заданий печати пользователем, который их создал.</span><span class="sxs-lookup"><span data-stu-id="c6bdb-126">This method supports filtering print jobs by the user who created them.</span></span> <span data-ttu-id="c6bdb-127">Используйте `$filter=createdBy/userPrincipalName eq '{upn}'` , **где {upn}** — это [основное имя](/azure/active-directory/hybrid/plan-connect-userprincipalname#what-is-userprincipalname) пользователя связанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="c6bdb-127">Use `$filter=createdBy/userPrincipalName eq '{upn}'`, where **{upn}** is the [user principal name](/azure/active-directory/hybrid/plan-connect-userprincipalname#what-is-userprincipalname) of the associated user.</span></span>

### <a name="exceptions"></a><span data-ttu-id="c6bdb-128">Exceptions</span><span class="sxs-lookup"><span data-stu-id="c6bdb-128">Exceptions</span></span>
<span data-ttu-id="c6bdb-129">Некоторые операторы не поддерживаются: `$count` , `$search` `$filter` .</span><span class="sxs-lookup"><span data-stu-id="c6bdb-129">Some operators are not supported: `$count`, `$search`, `$filter`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c6bdb-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c6bdb-130">Request headers</span></span>
| <span data-ttu-id="c6bdb-131">Имя</span><span class="sxs-lookup"><span data-stu-id="c6bdb-131">Name</span></span>      |<span data-ttu-id="c6bdb-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c6bdb-132">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c6bdb-133">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c6bdb-133">Authorization</span></span> | <span data-ttu-id="c6bdb-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c6bdb-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c6bdb-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c6bdb-136">Request body</span></span>
<span data-ttu-id="c6bdb-137">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c6bdb-137">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="c6bdb-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="c6bdb-138">Response</span></span>
<span data-ttu-id="c6bdb-139">В случае успешной работы этот метод возвращает код ответа и `200 OK` коллекцию [объектов printJob](../resources/printjob.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c6bdb-139">If successful, this method returns a `200 OK` response code and collection of [printJob](../resources/printjob.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c6bdb-140">Пример</span><span class="sxs-lookup"><span data-stu-id="c6bdb-140">Example</span></span>
### <a name="request"></a><span data-ttu-id="c6bdb-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="c6bdb-141">Request</span></span>
<span data-ttu-id="c6bdb-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c6bdb-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c6bdb-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="c6bdb-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_jobs_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/shares/{id}/jobs
```
# <a name="c"></a>[<span data-ttu-id="c6bdb-144">C#</span><span class="sxs-lookup"><span data-stu-id="c6bdb-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-jobs-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c6bdb-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c6bdb-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-jobs-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c6bdb-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c6bdb-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-jobs-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c6bdb-147">Java</span><span class="sxs-lookup"><span data-stu-id="c6bdb-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-jobs-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---

### <a name="response"></a><span data-ttu-id="c6bdb-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="c6bdb-148">Response</span></span>
<span data-ttu-id="c6bdb-149">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c6bdb-149">The following is an example of the response.</span></span>
><span data-ttu-id="c6bdb-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c6bdb-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
        "processingState": "completed",
        "processingStateDescription": "The print job has completed successfully and no further processing will take place."
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
