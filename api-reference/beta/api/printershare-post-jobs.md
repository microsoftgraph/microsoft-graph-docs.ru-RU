---
title: Создание printJob для принтераShare
description: Создайте новый printJob для принтераShare.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 643038023af0a805e32d88ea6d315a111541d2e8
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50955626"
---
# <a name="create-printjob-for-a-printershare"></a><span data-ttu-id="a2810-103">Создание printJob для принтераShare</span><span class="sxs-lookup"><span data-stu-id="a2810-103">Create printJob for a printerShare</span></span>

<span data-ttu-id="a2810-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2810-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a2810-105">Создайте новый [printJob](../resources/printJob.md) для [принтераShare](../resources/printerShare.md).</span><span class="sxs-lookup"><span data-stu-id="a2810-105">Create a new [printJob](../resources/printJob.md) for a [printerShare](../resources/printerShare.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="a2810-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a2810-106">Permissions</span></span>
<span data-ttu-id="a2810-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a2810-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="a2810-109">Помимо следующих разрешений, пользователь или клиент приложения должен иметь активную подписку на универсальную печать и иметь разрешение, дава которое предоставляет доступ [get printerShare.](printerShare-get.md)</span><span class="sxs-lookup"><span data-stu-id="a2810-109">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants [Get printerShare](printerShare-get.md) access.</span></span> <span data-ttu-id="a2810-110">Подписанный пользователем должен быть [администратором принтера.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="a2810-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="a2810-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a2810-111">Permission type</span></span> | <span data-ttu-id="a2810-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a2810-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="a2810-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a2810-113">Delegated (work or school account)</span></span>| <span data-ttu-id="a2810-114">PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2810-114">PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |
|<span data-ttu-id="a2810-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a2810-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a2810-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2810-116">Not Supported.</span></span>|
|<span data-ttu-id="a2810-117">Application</span><span class="sxs-lookup"><span data-stu-id="a2810-117">Application</span></span>| <span data-ttu-id="a2810-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2810-118">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a2810-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a2810-119">HTTP request</span></span>

```http
POST print/shares/{id}/jobs
```

## <a name="request-headers"></a><span data-ttu-id="a2810-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a2810-120">Request headers</span></span>
| <span data-ttu-id="a2810-121">Имя</span><span class="sxs-lookup"><span data-stu-id="a2810-121">Name</span></span>      |<span data-ttu-id="a2810-122">Описание</span><span class="sxs-lookup"><span data-stu-id="a2810-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a2810-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a2810-123">Authorization</span></span> | <span data-ttu-id="a2810-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a2810-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a2810-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a2810-126">Content-type</span></span>  | <span data-ttu-id="a2810-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a2810-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a2810-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a2810-129">Request body</span></span>
<span data-ttu-id="a2810-130">В теле запроса поставляем представление JSON объекта [printJob.](../resources/printjob.md)</span><span class="sxs-lookup"><span data-stu-id="a2810-130">In the request body, supply a JSON representation of a [printJob](../resources/printjob.md) object.</span></span>
<span data-ttu-id="a2810-131">Объект printJob должен содержать только **конфигурацию.**</span><span class="sxs-lookup"><span data-stu-id="a2810-131">The printJob object should only contain **configuration**.</span></span> <span data-ttu-id="a2810-132">Все свойства **конфигурации** являются недействительными.</span><span class="sxs-lookup"><span data-stu-id="a2810-132">All properties of **configuration** are nullable.</span></span>
<span data-ttu-id="a2810-133">Все остальные поля, включая ИД рабочих мест и документов, задаются автоматически во время создания ресурсов.</span><span class="sxs-lookup"><span data-stu-id="a2810-133">All other fields including job and document IDs are set automatically during resource creation.</span></span>

<span data-ttu-id="a2810-134">Сейчас универсальный шрифт поддерживает только одну **печатьDocument на** **объект printJob.**</span><span class="sxs-lookup"><span data-stu-id="a2810-134">Right now, Universal Print supports only one **printDocument** per **printJob** object.</span></span>

## <a name="response"></a><span data-ttu-id="a2810-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="a2810-135">Response</span></span>
<span data-ttu-id="a2810-136">В случае успешного выполнения этот метод возвращает код отклика и объект printJob и связанный с ним `201 Created` [шрифтDocument](../resources/printDocument.md) в тексте ответа. [](../resources/printjob.md)</span><span class="sxs-lookup"><span data-stu-id="a2810-136">If successful, this method returns a `201 Created` response code and a [printJob](../resources/printjob.md) object and associated [printDocument](../resources/printDocument.md) in the response body.</span></span> 
## <a name="example"></a><span data-ttu-id="a2810-137">Пример</span><span class="sxs-lookup"><span data-stu-id="a2810-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="a2810-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="a2810-138">Request</span></span>
<span data-ttu-id="a2810-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a2810-139">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a2810-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="a2810-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_printjob_2"
}-->
```http
POST https://graph.microsoft.com/beta/print/shares/{id}/jobs
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
# <a name="c"></a>[<span data-ttu-id="a2810-141">C#</span><span class="sxs-lookup"><span data-stu-id="a2810-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-printjob-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a2810-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a2810-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-printjob-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a2810-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a2810-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-printjob-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a2810-144">Java</span><span class="sxs-lookup"><span data-stu-id="a2810-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-printjob-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="a2810-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="a2810-145">Response</span></span>
<span data-ttu-id="a2810-146">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a2810-146">The following is an example of the response.</span></span>
><span data-ttu-id="a2810-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a2810-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
