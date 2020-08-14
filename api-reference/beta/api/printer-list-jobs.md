---
title: Список Принтжобс
description: Получение списка заданий печати, связанных с принтером.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: a7a219763c3efbea41c28e58a16358e7962dd04d
ms.sourcegitcommit: 5c3f4a3e2620d1d9e635e09231bbaa73cb0c3cdd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/14/2020
ms.locfileid: "46673779"
---
# <a name="list-printjobs"></a><span data-ttu-id="565ac-103">Список Принтжобс</span><span class="sxs-lookup"><span data-stu-id="565ac-103">List printJobs</span></span>

<span data-ttu-id="565ac-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="565ac-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="565ac-105">Получение списка заданий печати, связанных с [принтером](../resources/printer.md).</span><span class="sxs-lookup"><span data-stu-id="565ac-105">Retrieve a list of print jobs associated with the [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="565ac-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="565ac-106">Permissions</span></span>
<span data-ttu-id="565ac-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="565ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="565ac-109">Чтобы использовать универсальную службу печати, пользователь или клиент приложения должен иметь активную универсальную подписку на печать, разрешение, предоставляющее доступ к [принтеру](printer-get.md) , а также одно из разрешений, перечисленных в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="565ac-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, a permission that grants [Get printer](printer-get.md) access, and one of the permissions listed in the following table.</span></span> <span data-ttu-id="565ac-110">Пользователь, вошедшего в систему, должен быть [администратором принтера](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span><span class="sxs-lookup"><span data-stu-id="565ac-110">The signed in user must be a [Printer Administrator](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

<span data-ttu-id="565ac-111">Чтобы считывать задания печати от другого пользователя, пользователь, вошедшего в систему, должен быть администратором печати и иметь разрешение PrintJob. ReadBasic. ALL, PrintJob. Read. ALL, PrintJob. Реадвритебасик. ALL или PrintJob. ReadWrite. ALL.</span><span class="sxs-lookup"><span data-stu-id="565ac-111">To read print jobs from another user, the signed in user needs to be a print administrator and have the PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic.All, or PrintJob.ReadWrite.All permission.</span></span>

|<span data-ttu-id="565ac-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="565ac-112">Permission type</span></span> | <span data-ttu-id="565ac-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="565ac-113">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="565ac-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="565ac-114">Delegated (work or school account)</span></span>| <span data-ttu-id="565ac-115">PrintJob. ReadBasic, PrintJob. Read, PrintJob. ReadBasic. ALL, PrintJob. Read. ALL, PrintJob. Реадвритебасик, PrintJob. ReadWrite, PrintJob. Реадвритебасик. ALL, PrintJob. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="565ac-115">PrintJob.ReadBasic, PrintJob.Read, PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |
|<span data-ttu-id="565ac-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="565ac-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="565ac-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="565ac-117">Not Supported.</span></span>|
|<span data-ttu-id="565ac-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="565ac-118">Application</span></span>| <span data-ttu-id="565ac-119">PrintJob. ReadBasic. ALL, PrintJob. Read. ALL, PrintJob. Реадвритебасик. ALL, PrintJob. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="565ac-119">PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="565ac-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="565ac-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers/{id}/jobs
```

## <a name="optional-query-parameters"></a><span data-ttu-id="565ac-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="565ac-121">Optional query parameters</span></span>
<span data-ttu-id="565ac-122">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="565ac-122">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="565ac-123">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="565ac-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

### <a name="exceptions"></a><span data-ttu-id="565ac-124">Exceptions</span><span class="sxs-lookup"><span data-stu-id="565ac-124">Exceptions</span></span>
<span data-ttu-id="565ac-125">Некоторые операторы не поддерживаются: `$count` , `$search` , `$filter` .</span><span class="sxs-lookup"><span data-stu-id="565ac-125">Some operators are not supported: `$count`, `$search`, `$filter`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="565ac-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="565ac-126">Request headers</span></span>
| <span data-ttu-id="565ac-127">Имя</span><span class="sxs-lookup"><span data-stu-id="565ac-127">Name</span></span>      |<span data-ttu-id="565ac-128">Описание</span><span class="sxs-lookup"><span data-stu-id="565ac-128">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="565ac-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="565ac-129">Authorization</span></span> | <span data-ttu-id="565ac-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="565ac-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="565ac-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="565ac-132">Request body</span></span>
<span data-ttu-id="565ac-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="565ac-133">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="565ac-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="565ac-134">Response</span></span>
<span data-ttu-id="565ac-135">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [printJob](../resources/printjob.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="565ac-135">If successful, this method returns a `200 OK` response code and collection of [printJob](../resources/printjob.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="565ac-136">Пример</span><span class="sxs-lookup"><span data-stu-id="565ac-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="565ac-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="565ac-137">Request</span></span>
<span data-ttu-id="565ac-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="565ac-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="565ac-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="565ac-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_jobs"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/{id}/jobs
```
# <a name="c"></a>[<span data-ttu-id="565ac-140">C#</span><span class="sxs-lookup"><span data-stu-id="565ac-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-jobs-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="565ac-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="565ac-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-jobs-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="565ac-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="565ac-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-jobs-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="565ac-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="565ac-143">Response</span></span>
<span data-ttu-id="565ac-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="565ac-144">The following is an example of the response.</span></span>
><span data-ttu-id="565ac-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="565ac-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
