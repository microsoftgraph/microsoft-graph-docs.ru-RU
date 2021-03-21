---
title: Список printJobs для принтера
description: Извлечение списка заданий печати, связанных с принтером.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 8bda64c21c2f94a40115b24bc9297451efed417a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960912"
---
# <a name="list-printjobs-for-a-printer"></a><span data-ttu-id="8c097-103">Список printJobs для принтера</span><span class="sxs-lookup"><span data-stu-id="8c097-103">List printJobs for a printer</span></span>

<span data-ttu-id="8c097-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8c097-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c097-105">Извлечение списка заданий печати, связанных с [принтером.](../resources/printer.md)</span><span class="sxs-lookup"><span data-stu-id="8c097-105">Retrieve a list of print jobs associated with the [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8c097-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8c097-106">Permissions</span></span>
<span data-ttu-id="8c097-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c097-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="8c097-109">Чтобы использовать службу универсальной печати, клиент пользователя или приложения должен иметь активную подписку на универсальную печать, разрешение на получение доступа к принтеру и одно из разрешений, перечисленных в следующей таблице. [](printer-get.md)</span><span class="sxs-lookup"><span data-stu-id="8c097-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, a permission that grants [Get printer](printer-get.md) access, and one of the permissions listed in the following table.</span></span> <span data-ttu-id="8c097-110">Подписанный пользователем должен быть [администратором принтера.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="8c097-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

<span data-ttu-id="8c097-111">Чтобы прочитать задания печати у другого пользователя, пользователь должен быть администратором печати и иметь разрешение PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic.All или PrintJob.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="8c097-111">To read print jobs from another user, the signed in user needs to be a print administrator and have the PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic.All, or PrintJob.ReadWrite.All permission.</span></span>

|<span data-ttu-id="8c097-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8c097-112">Permission type</span></span> | <span data-ttu-id="8c097-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8c097-113">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="8c097-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8c097-114">Delegated (work or school account)</span></span>| <span data-ttu-id="8c097-115">PrintJob.ReadBasic, PrintJob.Read, PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c097-115">PrintJob.ReadBasic, PrintJob.Read, PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |
|<span data-ttu-id="8c097-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8c097-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8c097-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c097-117">Not Supported.</span></span>|
|<span data-ttu-id="8c097-118">Application</span><span class="sxs-lookup"><span data-stu-id="8c097-118">Application</span></span>| <span data-ttu-id="8c097-119">PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c097-119">PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8c097-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8c097-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers/{id}/jobs
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8c097-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8c097-121">Optional query parameters</span></span>
<span data-ttu-id="8c097-122">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="8c097-122">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="8c097-123">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="8c097-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

* <span data-ttu-id="8c097-124">Свойство **documents** по умолчанию опущено из ответа.</span><span class="sxs-lookup"><span data-stu-id="8c097-124">The **documents** property is omitted from the response by default.</span></span> <span data-ttu-id="8c097-125">Чтобы также вернуть список [печатных документов](../resources/printdocument.md) для каждого задания печати, используйте `$expand=documents` .</span><span class="sxs-lookup"><span data-stu-id="8c097-125">To also return a list of [printDocuments](../resources/printdocument.md) for each print job, use `$expand=documents`.</span></span>
* <span data-ttu-id="8c097-126">Этот метод поддерживает фильтрацию заданий печати пользователем, который их создал.</span><span class="sxs-lookup"><span data-stu-id="8c097-126">This method supports filtering print jobs by the user who created them.</span></span> <span data-ttu-id="8c097-127">Используйте `$filter=createdBy/userPrincipalName eq '{upn}'` , **где {upn}** — это [основное имя](/azure/active-directory/hybrid/plan-connect-userprincipalname#what-is-userprincipalname) пользователя связанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="8c097-127">Use `$filter=createdBy/userPrincipalName eq '{upn}'`, where **{upn}** is the [user principal name](/azure/active-directory/hybrid/plan-connect-userprincipalname#what-is-userprincipalname) of the associated user.</span></span>

### <a name="exceptions"></a><span data-ttu-id="8c097-128">Exceptions</span><span class="sxs-lookup"><span data-stu-id="8c097-128">Exceptions</span></span>
<span data-ttu-id="8c097-129">Некоторые операторы не поддерживаются: `$count` , `$search` `$filter` .</span><span class="sxs-lookup"><span data-stu-id="8c097-129">Some operators are not supported: `$count`, `$search`, `$filter`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8c097-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8c097-130">Request headers</span></span>
| <span data-ttu-id="8c097-131">Имя</span><span class="sxs-lookup"><span data-stu-id="8c097-131">Name</span></span>      |<span data-ttu-id="8c097-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8c097-132">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8c097-133">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8c097-133">Authorization</span></span> | <span data-ttu-id="8c097-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8c097-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8c097-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8c097-136">Request body</span></span>
<span data-ttu-id="8c097-137">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8c097-137">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="8c097-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c097-138">Response</span></span>
<span data-ttu-id="8c097-139">В случае успешной работы этот метод возвращает код ответа и `200 OK` коллекцию [объектов printJob](../resources/printjob.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8c097-139">If successful, this method returns a `200 OK` response code and collection of [printJob](../resources/printjob.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8c097-140">Пример</span><span class="sxs-lookup"><span data-stu-id="8c097-140">Example</span></span>
### <a name="request"></a><span data-ttu-id="8c097-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="8c097-141">Request</span></span>
<span data-ttu-id="8c097-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8c097-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8c097-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="8c097-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_jobs_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/{id}/jobs
```
# <a name="c"></a>[<span data-ttu-id="8c097-144">C#</span><span class="sxs-lookup"><span data-stu-id="8c097-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-jobs-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8c097-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8c097-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-jobs-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8c097-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8c097-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-jobs-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8c097-147">Java</span><span class="sxs-lookup"><span data-stu-id="8c097-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-jobs-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="8c097-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c097-148">Response</span></span>
<span data-ttu-id="8c097-149">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8c097-149">The following is an example of the response.</span></span>
><span data-ttu-id="8c097-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8c097-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/printers('c05f3726-0d4b-4aa1-8fe9-2eb981bb26fb')/jobs",
  "value": [
    {
      "id": "5182",
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
