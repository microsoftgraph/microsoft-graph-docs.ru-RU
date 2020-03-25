---
title: 'принтер: Capabilities'
description: Получение списка возможностей принтера.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: d3ed6f5f57bc528abaec2661d7bd8d88cba7d75e
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/25/2020
ms.locfileid: "42947982"
---
# <a name="printer-getcapabilities"></a><span data-ttu-id="fd35b-103">принтер: Capabilities</span><span class="sxs-lookup"><span data-stu-id="fd35b-103">printer: getCapabilities</span></span>

<span data-ttu-id="fd35b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fd35b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fd35b-105">Получение списка возможностей [принтера](../resources/printer.md).</span><span class="sxs-lookup"><span data-stu-id="fd35b-105">Get a list of capabilities for the [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="fd35b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fd35b-106">Permissions</span></span>
<span data-ttu-id="fd35b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fd35b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="fd35b-109">В дополнение к следующим разрешениям клиент пользователя должен иметь активную универсальную подписку на печать.</span><span class="sxs-lookup"><span data-stu-id="fd35b-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="fd35b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fd35b-110">Permission type</span></span> | <span data-ttu-id="fd35b-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fd35b-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="fd35b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fd35b-112">Delegated (work or school account)</span></span>| <span data-ttu-id="fd35b-113">Users. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="fd35b-113">Users.Read.All</span></span> |
|<span data-ttu-id="fd35b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fd35b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fd35b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fd35b-115">Not Supported.</span></span>|
|<span data-ttu-id="fd35b-116">Для приложения</span><span class="sxs-lookup"><span data-stu-id="fd35b-116">Application</span></span>|<span data-ttu-id="fd35b-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fd35b-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fd35b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fd35b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/{id}/getCapabilities
```
## <a name="request-headers"></a><span data-ttu-id="fd35b-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fd35b-119">Request headers</span></span>
| <span data-ttu-id="fd35b-120">Имя</span><span class="sxs-lookup"><span data-stu-id="fd35b-120">Name</span></span>          | <span data-ttu-id="fd35b-121">Описание</span><span class="sxs-lookup"><span data-stu-id="fd35b-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="fd35b-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fd35b-122">Authorization</span></span> | <span data-ttu-id="fd35b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fd35b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fd35b-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fd35b-125">Request body</span></span>

## <a name="response"></a><span data-ttu-id="fd35b-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="fd35b-126">Response</span></span>
<span data-ttu-id="fd35b-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [принтеркапабилитиес](../resources/printercapabilities.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fd35b-127">If successful, this method returns a `200 OK` response code and a [printerCapabilities](../resources/printercapabilities.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fd35b-128">Пример</span><span class="sxs-lookup"><span data-stu-id="fd35b-128">Example</span></span>
<span data-ttu-id="fd35b-129">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="fd35b-129">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="fd35b-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="fd35b-130">Request</span></span>
<span data-ttu-id="fd35b-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fd35b-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="fd35b-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="fd35b-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "printer-getCapabilities"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/{id}/getCapabilities
```
# <a name="c"></a>[<span data-ttu-id="fd35b-133">C#</span><span class="sxs-lookup"><span data-stu-id="fd35b-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/printer-getcapabilities-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fd35b-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fd35b-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/printer-getcapabilities-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fd35b-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fd35b-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/printer-getcapabilities-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="fd35b-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="fd35b-136">Response</span></span>
<span data-ttu-id="fd35b-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fd35b-137">The following is an example of the response.</span></span>
><span data-ttu-id="fd35b-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fd35b-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printerCapabilities"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1159

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.printerCapabilities",
    "isColorPrintingSupported": true,
    "supportsFitPdfToPage": false,
    "supportedDocumentMimeTypes": [
        "application/oxps"
    ],
    "supportedFinishings": [
        "none"
    ],
    "supportedMediaColors": [],
    "supportedMediaTypes": [],
    "supportedMediaSizes": [
        "North America Letter",
        "North America Ledger",
        "North America Legal",
        "North America Invoice",
        "North America Executive",
        "A3",
        "A4",
        "A5",
        "JIS B4",
        "JIS B5"
    ],
    "supportedOrientations": [
        "portrait",
        "landscape"
    ],
    "supportedOutputBins": [
        "tray-1"
    ],
    "supportedDuplexConfigurations": [
        "oneSided"
    ],
    "supportedPresentationDirections": [],
    "supportedColorConfigurations": [
        "color"
    ],
    "supportedPrintQualities": [
        "medium"
    ],
    "supportedPagesPerSheet": null,
    "supportedCopiesPerJob": {
        "minimum": 1,
        "maximum": 1
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printer: getCapabilities",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
