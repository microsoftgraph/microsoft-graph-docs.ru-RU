---
title: Создание printJob для принтера
description: Создайте новый printJob для принтера.
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: da2a664a6748f73b7dd5df78b7f5e75850860794
ms.sourcegitcommit: a0a5690ad9c109149e0b8c8baba164648ff5c226
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/08/2021
ms.locfileid: "49784864"
---
# <a name="create-printjob-for-a-printer"></a><span data-ttu-id="1ed1b-103">Создание printJob для принтера</span><span class="sxs-lookup"><span data-stu-id="1ed1b-103">Create printJob for a printer</span></span>

<span data-ttu-id="1ed1b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1ed1b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1ed1b-105">Создайте новый [printJob](../resources/printJob.md) для [принтера.](../resources/printer.md)</span><span class="sxs-lookup"><span data-stu-id="1ed1b-105">Create a new [printJob](../resources/printJob.md) for a [printer](../resources/printer.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="1ed1b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1ed1b-106">Permissions</span></span>
<span data-ttu-id="1ed1b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1ed1b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="1ed1b-109">Помимо следующих разрешений, у пользователя или клиента приложения должна быть активная подписка на универсальную печать и разрешение, которое предоставляет [доступ к принтеру.](printer-get.md)</span><span class="sxs-lookup"><span data-stu-id="1ed1b-109">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants [Get printer](printer-get.md) access.</span></span> <span data-ttu-id="1ed1b-110">Пользователь, выписав его, должен быть [администратором принтера.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="1ed1b-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="1ed1b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1ed1b-111">Permission type</span></span> | <span data-ttu-id="1ed1b-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1ed1b-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="1ed1b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1ed1b-113">Delegated (work or school account)</span></span>| <span data-ttu-id="1ed1b-114">PrintJob.Create, PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ed1b-114">PrintJob.Create, PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |
|<span data-ttu-id="1ed1b-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1ed1b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1ed1b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1ed1b-116">Not Supported.</span></span>|
|<span data-ttu-id="1ed1b-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="1ed1b-117">Application</span></span>| <span data-ttu-id="1ed1b-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1ed1b-118">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1ed1b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1ed1b-119">HTTP request</span></span>

```http
POST print/printers/{id}/jobs
```

## <a name="request-headers"></a><span data-ttu-id="1ed1b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1ed1b-120">Request headers</span></span>
| <span data-ttu-id="1ed1b-121">Имя</span><span class="sxs-lookup"><span data-stu-id="1ed1b-121">Name</span></span>      |<span data-ttu-id="1ed1b-122">Описание</span><span class="sxs-lookup"><span data-stu-id="1ed1b-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1ed1b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1ed1b-123">Authorization</span></span> | <span data-ttu-id="1ed1b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1ed1b-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1ed1b-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1ed1b-126">Content-type</span></span>  | <span data-ttu-id="1ed1b-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1ed1b-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1ed1b-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1ed1b-129">Request body</span></span>
<span data-ttu-id="1ed1b-130">В теле запроса укажийте представление объекта [printJob](../resources/printjob.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="1ed1b-130">In the request body, supply a JSON representation of a [printJob](../resources/printjob.md) object.</span></span> <span data-ttu-id="1ed1b-131">Объект printJob должен содержать только **конфигурацию.**</span><span class="sxs-lookup"><span data-stu-id="1ed1b-131">The printJob object should only contain **configuration**.</span></span> <span data-ttu-id="1ed1b-132">Все свойства **конфигурации имеют** null.</span><span class="sxs-lookup"><span data-stu-id="1ed1b-132">All properties of **configuration** are nullable.</span></span> <span data-ttu-id="1ed1b-133">Все остальные поля, включая задания и ИД документов, задаются автоматически во время создания ресурса.</span><span class="sxs-lookup"><span data-stu-id="1ed1b-133">All other fields, including job and document IDs, are set automatically during resource creation.</span></span>

<span data-ttu-id="1ed1b-134">Сейчас универсальная печать поддерживает только один **объект printDocument для** **каждого объекта printJob.**</span><span class="sxs-lookup"><span data-stu-id="1ed1b-134">Right now, Universal Print supports only one **printDocument** per **printJob** object.</span></span>

## <a name="response"></a><span data-ttu-id="1ed1b-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="1ed1b-135">Response</span></span>
<span data-ttu-id="1ed1b-136">В случае успешного выполнения этот метод возвращает код ответа, объект `201 Created` [printJob](../resources/printjob.md) и связанный объект [printDocument](../resources/printDocument.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1ed1b-136">If successful, this method returns a `201 Created` response code and a [printJob](../resources/printjob.md) object and associated [printDocument](../resources/printDocument.md) in the response body.</span></span> 
## <a name="example"></a><span data-ttu-id="1ed1b-137">Пример</span><span class="sxs-lookup"><span data-stu-id="1ed1b-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="1ed1b-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="1ed1b-138">Request</span></span>
<span data-ttu-id="1ed1b-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1ed1b-139">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1ed1b-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="1ed1b-140">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="1ed1b-141">C#</span><span class="sxs-lookup"><span data-stu-id="1ed1b-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-printjob-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1ed1b-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1ed1b-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-printjob-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1ed1b-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1ed1b-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-printjob-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1ed1b-144">Java</span><span class="sxs-lookup"><span data-stu-id="1ed1b-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-printjob-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="1ed1b-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="1ed1b-145">Response</span></span>
<span data-ttu-id="1ed1b-146">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1ed1b-146">The following is an example of the response.</span></span>
><span data-ttu-id="1ed1b-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1ed1b-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
