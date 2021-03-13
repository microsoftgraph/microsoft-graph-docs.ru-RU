---
title: Обновление printJob
description: Обновлениеконфигурациизадания печати.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 6405acd01be075c44c4271c4c3395a83889f9d0e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50777687"
---
# <a name="update-printjob"></a><span data-ttu-id="e3546-103">Обновление printJob</span><span class="sxs-lookup"><span data-stu-id="e3546-103">Update printJob</span></span>

<span data-ttu-id="e3546-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3546-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e3546-105">Обновление [задания печати](../resources/printjob.md).</span><span class="sxs-lookup"><span data-stu-id="e3546-105">Update a [print job](../resources/printjob.md).</span></span> <span data-ttu-id="e3546-106">Только свойство **конфигурации** может быть обновлено.</span><span class="sxs-lookup"><span data-stu-id="e3546-106">Only the **configuration** property can be updated.</span></span>

<span data-ttu-id="e3546-107">Обновление задания печати будет успешным только в том случае, если задание [printTask](../resources/printTask.md) в состоянии, начатое с триггера, созданного `processing` приложением-запросом, связано с заданием печати.</span><span class="sxs-lookup"><span data-stu-id="e3546-107">Updating a print job will only succeed if a [printTask](../resources/printTask.md) in a `processing` state, started by a trigger that the requesting app created, is associated with the print job.</span></span> <span data-ttu-id="e3546-108">Подробные сведения о регистрации триггера задач см. в материале [Extending Universal Print to support pull printing.](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)</span><span class="sxs-lookup"><span data-stu-id="e3546-108">For details about how to register a task trigger, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="e3546-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e3546-109">Permissions</span></span>
<span data-ttu-id="e3546-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e3546-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="e3546-112">Чтобы использовать службу универсальной печати, пользователь или клиент приложения должен иметь активную подписку на универсальную печать, либо разрешение принтера.Read.All или Printer.ReadWrite.All, а также одно из разрешений, указанных в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="e3546-112">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, either the Printer.Read.All or Printer.ReadWrite.All application permission, and one of the permissions listed in the following table.</span></span>

|<span data-ttu-id="e3546-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e3546-113">Permission type</span></span> | <span data-ttu-id="e3546-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e3546-114">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="e3546-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e3546-115">Delegated (work or school account)</span></span>| <span data-ttu-id="e3546-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3546-116">Not supported.</span></span> |
|<span data-ttu-id="e3546-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e3546-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e3546-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3546-118">Not Supported.</span></span>|
|<span data-ttu-id="e3546-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e3546-119">Application</span></span>| <span data-ttu-id="e3546-120">PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All, PrintJob.Manage.All</span><span class="sxs-lookup"><span data-stu-id="e3546-120">PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All, PrintJob.Manage.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e3546-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e3546-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /print/printers/{id}/jobs/{id}
```
## <a name="request-headers"></a><span data-ttu-id="e3546-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e3546-122">Request headers</span></span>
| <span data-ttu-id="e3546-123">Имя</span><span class="sxs-lookup"><span data-stu-id="e3546-123">Name</span></span>          | <span data-ttu-id="e3546-124">Описание</span><span class="sxs-lookup"><span data-stu-id="e3546-124">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="e3546-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e3546-125">Authorization</span></span> | <span data-ttu-id="e3546-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e3546-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e3546-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e3546-128">Request body</span></span>
<span data-ttu-id="e3546-129">В теле запроса укажи значения соответствующих [полей printJob.](../resources/printjob.md)</span><span class="sxs-lookup"><span data-stu-id="e3546-129">In the request body, supply the values of the relevant [printJob](../resources/printjob.md) fields.</span></span> <span data-ttu-id="e3546-130">Существующие свойства, не включенные в тело запроса, будут поддерживать прежние значения.</span><span class="sxs-lookup"><span data-stu-id="e3546-130">Existing properties that are not included in the request body will maintain their previous values.</span></span> <span data-ttu-id="e3546-131">Обновить можно только свойство "конфигурация".</span><span class="sxs-lookup"><span data-stu-id="e3546-131">Only the "configuration" property can be updated.</span></span>

## <a name="response"></a><span data-ttu-id="e3546-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="e3546-132">Response</span></span>
<span data-ttu-id="e3546-133">В случае успешной работы этот метод возвращает код ответа с обновленным объектом `200 OK` [printJob](../resources/printjob.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e3546-133">If successful, this method returns a `200 OK` response code with an updated [printJob](../resources/printjob.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e3546-134">Пример</span><span class="sxs-lookup"><span data-stu-id="e3546-134">Example</span></span>
<span data-ttu-id="e3546-135">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="e3546-135">The following example shows how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="e3546-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="e3546-136">Request</span></span>
<span data-ttu-id="e3546-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e3546-137">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e3546-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="e3546-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "printjob-update"
}-->
```http
PATCH https://graph.microsoft.com/beta/print/printers/d5ef6ec4-07ca-4212-baf9-d45be126bfbb/jobs/44353

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
# <a name="c"></a>[<span data-ttu-id="e3546-139">C#</span><span class="sxs-lookup"><span data-stu-id="e3546-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/printjob-update-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e3546-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e3546-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/printjob-update-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e3546-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e3546-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/printjob-update-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e3546-142">Java</span><span class="sxs-lookup"><span data-stu-id="e3546-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/printjob-update-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e3546-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="e3546-143">Response</span></span>
<span data-ttu-id="e3546-144">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="e3546-144">The following is an example of the response.</span></span> 
><span data-ttu-id="e3546-145">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e3546-145">**Note:** The response object shown here might be shortened for readability.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printJob"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 225

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/printers('d5ef6ec4-07ca-4212-baf9-d45be126bfbb')/jobs/$entity",
  "id": "44353",
  "createdDateTime": "2020-06-26T04:20:06.5715544Z",
  "createdBy": {
    "id": "",
    "displayName": "",
    "userPrincipalName": ""
  },
  "status": {
    "state": "paused",
    "description": "The job is not a candidate for processing yet."
  },
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update print job",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


