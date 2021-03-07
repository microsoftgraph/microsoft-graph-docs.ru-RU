---
title: Список printJobs для принтера
description: Извлечение списка заданий печати, связанных с принтером.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 064d95da16c80449a054006807a203a494e139d6
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517973"
---
# <a name="list-printjobs-for-a-printer"></a><span data-ttu-id="ddcc4-103">Список printJobs для принтера</span><span class="sxs-lookup"><span data-stu-id="ddcc4-103">List printJobs for a printer</span></span>
<span data-ttu-id="ddcc4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ddcc4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="ddcc4-105">Извлечение списка заданий печати, связанных с [принтером.](../resources/printer.md)</span><span class="sxs-lookup"><span data-stu-id="ddcc4-105">Retrieve a list of print jobs associated with the [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ddcc4-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ddcc4-106">Permissions</span></span>
<span data-ttu-id="ddcc4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ddcc4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="ddcc4-109">Чтобы использовать службу универсальной печати, клиент пользователя или приложения должен иметь активную подписку на универсальную печать, разрешение на получение доступа к принтеру и одно из разрешений, перечисленных в следующей таблице. [](printer-get.md)</span><span class="sxs-lookup"><span data-stu-id="ddcc4-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, a permission that grants [Get printer](printer-get.md) access, and one of the permissions listed in the following table.</span></span> <span data-ttu-id="ddcc4-110">Подписанный пользователем должен быть [администратором принтера.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="ddcc4-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

<span data-ttu-id="ddcc4-111">Чтобы прочитать задания печати у другого пользователя, пользователь должен быть администратором печати и иметь разрешение PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic.All или PrintJob.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="ddcc4-111">To read print jobs from another user, the signed in user needs to be a print administrator and have the PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic.All, or PrintJob.ReadWrite.All permission.</span></span>

|<span data-ttu-id="ddcc4-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ddcc4-112">Permission type</span></span> | <span data-ttu-id="ddcc4-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ddcc4-113">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="ddcc4-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ddcc4-114">Delegated (work or school account)</span></span>| <span data-ttu-id="ddcc4-115">PrintJob.ReadBasic, PrintJob.Read, PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ddcc4-115">PrintJob.ReadBasic, PrintJob.Read, PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |
|<span data-ttu-id="ddcc4-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ddcc4-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ddcc4-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ddcc4-117">Not Supported.</span></span>|
|<span data-ttu-id="ddcc4-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="ddcc4-118">Application</span></span>| <span data-ttu-id="ddcc4-119">PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ddcc4-119">PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ddcc4-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ddcc4-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /print/printers/{printerId}/jobs
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ddcc4-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ddcc4-121">Optional query parameters</span></span>
<span data-ttu-id="ddcc4-122">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="ddcc4-122">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="ddcc4-123">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="ddcc4-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

* <span data-ttu-id="ddcc4-124">Свойство **documents** по умолчанию опущено из ответа.</span><span class="sxs-lookup"><span data-stu-id="ddcc4-124">The **documents** property is omitted from the response by default.</span></span> <span data-ttu-id="ddcc4-125">Чтобы также вернуть список [печатных документов](../resources/printdocument.md) для каждого задания печати, используйте `$expand=documents` .</span><span class="sxs-lookup"><span data-stu-id="ddcc4-125">To also return a list of [printDocuments](../resources/printdocument.md) for each print job, use `$expand=documents`.</span></span>
* <span data-ttu-id="ddcc4-126">Этот метод поддерживает фильтрацию заданий печати пользователем, который их создал.</span><span class="sxs-lookup"><span data-stu-id="ddcc4-126">This method supports filtering print jobs by the user who created them.</span></span> <span data-ttu-id="ddcc4-127">Используйте `$filter=createdBy/userPrincipalName eq '{upn}'` , **где {upn}** — это [основное имя](/azure/active-directory/hybrid/plan-connect-userprincipalname#what-is-userprincipalname) пользователя связанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="ddcc4-127">Use `$filter=createdBy/userPrincipalName eq '{upn}'`, where **{upn}** is the [user principal name](/azure/active-directory/hybrid/plan-connect-userprincipalname#what-is-userprincipalname) of the associated user.</span></span>

### <a name="exceptions"></a><span data-ttu-id="ddcc4-128">Exceptions</span><span class="sxs-lookup"><span data-stu-id="ddcc4-128">Exceptions</span></span>
<span data-ttu-id="ddcc4-129">Некоторые операторы не поддерживаются: `$count` , `$search` .</span><span class="sxs-lookup"><span data-stu-id="ddcc4-129">Some operators are not supported: `$count`, `$search`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ddcc4-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ddcc4-130">Request headers</span></span>
|<span data-ttu-id="ddcc4-131">Имя</span><span class="sxs-lookup"><span data-stu-id="ddcc4-131">Name</span></span>|<span data-ttu-id="ddcc4-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ddcc4-132">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ddcc4-133">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ddcc4-133">Authorization</span></span>|<span data-ttu-id="ddcc4-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ddcc4-p106">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ddcc4-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ddcc4-136">Request body</span></span>
<span data-ttu-id="ddcc4-137">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ddcc4-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ddcc4-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="ddcc4-138">Response</span></span>

<span data-ttu-id="ddcc4-139">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [printJob](../resources/printjob.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="ddcc4-139">If successful, this method returns a `200 OK` response code and a collection of [printJob](../resources/printjob.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ddcc4-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="ddcc4-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ddcc4-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="ddcc4-141">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_printjob"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/printers/{printerId}/jobs
```


### <a name="response"></a><span data-ttu-id="ddcc4-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="ddcc4-142">Response</span></span>
<span data-ttu-id="ddcc4-143">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ddcc4-143">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.printJob)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/printers('2f3453b7-4686-4b5b-9575-4f1e5b909ba7')/jobs",
  "value": [
    {
      "id": "103",
      "createdDateTime": "2020-02-04T00:00:00.0000000Z",
      "createdBy": {        
      },
      "status": {
        "state": "completed",
        "description": "The print job has completed successfully and no further processing will take place.",
        "details": [          
        ],
        "isAcquiredByPrinter": true
      },
      "configuration": {        
      },
      "redirectedTo": null,
      "redirectedFrom": null,
      "isFetchable": false     
    }
  ]
}
```

