---
title: Создание метода printJob для принтера
description: Создание нового метода printJob для принтера.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 026905fb3d0dc2b0be71bcb5175c6741b63a9fba
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48979857"
---
# <a name="create-printjob-for-a-printer"></a><span data-ttu-id="f0929-103">Создание метода printJob для принтера</span><span class="sxs-lookup"><span data-stu-id="f0929-103">Create printJob for a printer</span></span>

<span data-ttu-id="f0929-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f0929-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0929-105">Создание нового [метода printJob](../resources/printJob.md) для [принтера](../resources/printer.md).</span><span class="sxs-lookup"><span data-stu-id="f0929-105">Create a new [printJob](../resources/printJob.md) for a [printer](../resources/printer.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="f0929-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f0929-106">Permissions</span></span>
<span data-ttu-id="f0929-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f0929-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="f0929-109">В дополнение к следующим разрешениям пользователь или клиент приложения должен иметь активную универсальную подписку на печать и иметь разрешение на получение доступа к [принтеру](printer-get.md) .</span><span class="sxs-lookup"><span data-stu-id="f0929-109">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants [Get printer](printer-get.md) access.</span></span> <span data-ttu-id="f0929-110">Пользователь, вошедшего в систему, должен быть [администратором принтера](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span><span class="sxs-lookup"><span data-stu-id="f0929-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="f0929-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f0929-111">Permission type</span></span> | <span data-ttu-id="f0929-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f0929-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="f0929-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f0929-113">Delegated (work or school account)</span></span>| <span data-ttu-id="f0929-114">PrintJob. Реадвритебасик, PrintJob. ReadWrite, PrintJob. Реадвритебасик. ALL, PrintJob. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="f0929-114">PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |
|<span data-ttu-id="f0929-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f0929-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f0929-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0929-116">Not Supported.</span></span>|
|<span data-ttu-id="f0929-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="f0929-117">Application</span></span>| <span data-ttu-id="f0929-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0929-118">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f0929-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f0929-119">HTTP request</span></span>

```http
POST print/printers/{id}/jobs
```

## <a name="request-headers"></a><span data-ttu-id="f0929-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f0929-120">Request headers</span></span>
| <span data-ttu-id="f0929-121">Имя</span><span class="sxs-lookup"><span data-stu-id="f0929-121">Name</span></span>      |<span data-ttu-id="f0929-122">Описание</span><span class="sxs-lookup"><span data-stu-id="f0929-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f0929-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f0929-123">Authorization</span></span> | <span data-ttu-id="f0929-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f0929-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f0929-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f0929-126">Content-type</span></span>  | <span data-ttu-id="f0929-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f0929-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0929-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f0929-129">Request body</span></span>
<span data-ttu-id="f0929-130">В тексте запроса добавьте представление объекта [printJob](../resources/printjob.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f0929-130">In the request body, supply a JSON representation of a [printJob](../resources/printjob.md) object.</span></span> <span data-ttu-id="f0929-131">Объект printJob должен содержать только **конфигурацию**.</span><span class="sxs-lookup"><span data-stu-id="f0929-131">The printJob object should only contain **configuration**.</span></span> <span data-ttu-id="f0929-132">Все свойства **конфигурации** допускают значение null.</span><span class="sxs-lookup"><span data-stu-id="f0929-132">All properties of **configuration** are nullable.</span></span> <span data-ttu-id="f0929-133">Все остальные поля, в том числе задания и идентификаторы документов, задаются автоматически при создании ресурса.</span><span class="sxs-lookup"><span data-stu-id="f0929-133">All other fields, including job and document IDs, are set automatically during resource creation.</span></span>

<span data-ttu-id="f0929-134">Теперь для универсальной печати поддерживается только один **printDocument** для каждого объекта **printJob** .</span><span class="sxs-lookup"><span data-stu-id="f0929-134">Right now, Universal Print supports only one **printDocument** per **printJob** object.</span></span>

## <a name="response"></a><span data-ttu-id="f0929-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="f0929-135">Response</span></span>
<span data-ttu-id="f0929-136">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [printJob](../resources/printjob.md) и связанный с [printDocument](../resources/printDocument.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f0929-136">If successful, this method returns a `201 Created` response code and a [printJob](../resources/printjob.md) object and associated [printDocument](../resources/printDocument.md) in the response body.</span></span> 
## <a name="example"></a><span data-ttu-id="f0929-137">Пример</span><span class="sxs-lookup"><span data-stu-id="f0929-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="f0929-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="f0929-138">Request</span></span>
<span data-ttu-id="f0929-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f0929-139">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f0929-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="f0929-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_printjob"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/{id}/jobs
Content-type: application/json

{
  "configuration": {
    "feedOrientation": "longEdgeFirst",
    "pageRanges": [
      {
        "start": 1,
        "end": 1
      }
    ],
    "quality": "medium",
    "dpi": 600,
    "orientation": "landscape",
    "copies": 1,
    "duplexMode": "oneSided",
    "colorMode": "blackAndWhite",
    "inputBin": "by-pass-tray",
    "outputBin": "output-tray",
    "mediaSize": "A4",
    "margin": {
      "top": 0,
      "bottom": 0,
      "left": 0,
      "right": 0
    },
    "mediaType": "stationery",
    "finishings": null,
    "pagesPerSheet": 1,
    "multipageLayout": "clockwiseFromBottomLeft",
    "collate": false,
    "scaling": "shrinkToFit",
    "fitPdfToPage": false
  }
}
```
# <a name="c"></a>[<span data-ttu-id="f0929-141">C#</span><span class="sxs-lookup"><span data-stu-id="f0929-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-printjob-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f0929-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f0929-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-printjob-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f0929-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f0929-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-printjob-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f0929-144">Java</span><span class="sxs-lookup"><span data-stu-id="f0929-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-printjob-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="f0929-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="f0929-145">Response</span></span>
<span data-ttu-id="f0929-146">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f0929-146">The following is an example of the response.</span></span>
><span data-ttu-id="f0929-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f0929-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printJob"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 1065

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/printJobs/$entity",
  "id": "1825",
  "createdDateTime": "2020-10-14T05:16:49-07:00",
  "isFetchable": false,
  "redirectedFrom": null,
  "redirectedTo": null,
  "createdBy": {
    "id": "{userId}",
    "displayName": "{username}",
    "ipAddress": null,
    "userPrincipalName": "{userupn}"
  },
  "status": {
    "state": "paused",
    "description": "The job is not a candidate for processing yet.",
    "isAcquiredByPrinter": false,
    "details": [
      "uploadPending"
    ]
  },
  "configuration": {
    "quality": "medium",
    "dpi": 600,
    "feedOrientation": "longEdgeFirst",
    "orientation": "landscape",
    "duplexMode": "oneSided",
    "copies": 1,
    "colorMode": "blackAndWhite",
    "inputBin": "by-pass-tray",
    "outputBin": "output-tray",
    "mediaSize": "A4",
    "mediaType": "stationery",
    "finishings": null,
    "pagesPerSheet": 1,
    "multipageLayout": "clockwiseFromBottomLeft",
    "collate": false,
    "scaling": "shrinkToFit",
    "fitPdfToPage": false,
    "pageRanges": [
      {
        "start": 1,
        "end": 1
      }
    ],
    "margin": {
      "top": 0,
      "bottom": 0,
      "left": 0,
      "right": 0
    }
  },
  "documents": [
    {
      "id": "1477576d-5dab-4ea9-865c-c0b82cd70bd5",
      "displayName": "",
      "contentType": "",
      "size": 0
    }
  ]
}
```
