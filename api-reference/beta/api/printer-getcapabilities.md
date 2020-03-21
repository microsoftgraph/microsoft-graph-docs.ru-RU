---
title: 'принтер: Capabilities'
description: Получение списка возможностей принтера.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 675b82605f4bde04b92702204693c3c81b4bd603
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/21/2020
ms.locfileid: "42896281"
---
# <a name="printer-getcapabilities"></a><span data-ttu-id="7c48b-103">принтер: Capabilities</span><span class="sxs-lookup"><span data-stu-id="7c48b-103">printer: getCapabilities</span></span>

<span data-ttu-id="7c48b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7c48b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7c48b-105">Получение списка возможностей [принтера](../resources/printer.md).</span><span class="sxs-lookup"><span data-stu-id="7c48b-105">Get a list of capabilities for the [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7c48b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7c48b-106">Permissions</span></span>
<span data-ttu-id="7c48b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7c48b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="7c48b-109">В дополнение к следующим разрешениям клиент пользователя должен иметь активную универсальную подписку на печать.</span><span class="sxs-lookup"><span data-stu-id="7c48b-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="7c48b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7c48b-110">Permission type</span></span> | <span data-ttu-id="7c48b-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7c48b-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="7c48b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7c48b-112">Delegated (work or school account)</span></span>| <span data-ttu-id="7c48b-113">Users. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="7c48b-113">Users.Read.All</span></span> |
|<span data-ttu-id="7c48b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7c48b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7c48b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c48b-115">Not Supported.</span></span>|
|<span data-ttu-id="7c48b-116">Для приложения</span><span class="sxs-lookup"><span data-stu-id="7c48b-116">Application</span></span>|<span data-ttu-id="7c48b-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c48b-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7c48b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7c48b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/{id}/getCapabilities
```
## <a name="request-headers"></a><span data-ttu-id="7c48b-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7c48b-119">Request headers</span></span>
| <span data-ttu-id="7c48b-120">Имя</span><span class="sxs-lookup"><span data-stu-id="7c48b-120">Name</span></span>          | <span data-ttu-id="7c48b-121">Описание</span><span class="sxs-lookup"><span data-stu-id="7c48b-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="7c48b-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7c48b-122">Authorization</span></span> | <span data-ttu-id="7c48b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7c48b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7c48b-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7c48b-125">Request body</span></span>

## <a name="response"></a><span data-ttu-id="7c48b-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="7c48b-126">Response</span></span>
<span data-ttu-id="7c48b-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [принтеркапабилитиес](../resources/printercapabilities.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7c48b-127">If successful, this method returns a `200 OK` response code and a [printerCapabilities](../resources/printercapabilities.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c48b-128">Пример</span><span class="sxs-lookup"><span data-stu-id="7c48b-128">Example</span></span>
<span data-ttu-id="7c48b-129">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="7c48b-129">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7c48b-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="7c48b-130">Request</span></span>
<span data-ttu-id="7c48b-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7c48b-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "printer-getCapabilities"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/{id}/getCapabilities
```

##### <a name="response"></a><span data-ttu-id="7c48b-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="7c48b-132">Response</span></span>
<span data-ttu-id="7c48b-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7c48b-133">The following is an example of the response.</span></span>
><span data-ttu-id="7c48b-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7c48b-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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