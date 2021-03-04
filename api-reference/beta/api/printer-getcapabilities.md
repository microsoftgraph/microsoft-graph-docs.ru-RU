---
title: 'принтер: getCapabilities'
description: Получите список возможностей для принтера.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: a9d9b1e21d26e39ea50020f56f48f496c83b609c
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447737"
---
# <a name="printer-getcapabilities"></a><span data-ttu-id="aee96-103">принтер: getCapabilities</span><span class="sxs-lookup"><span data-stu-id="aee96-103">printer: getCapabilities</span></span>

<span data-ttu-id="aee96-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aee96-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aee96-105">Получите список возможностей для [принтера.](../resources/printer.md)</span><span class="sxs-lookup"><span data-stu-id="aee96-105">Get a list of capabilities for the [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="aee96-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="aee96-106">Permissions</span></span>
<span data-ttu-id="aee96-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aee96-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="aee96-109">Чтобы использовать службу универсальной печати, пользователь или клиент приложения должен иметь активную подписку универсальной печати в дополнение к разрешениям, перечисленным в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="aee96-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="aee96-110">Подписанный пользователем должен быть [администратором принтера.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="aee96-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="aee96-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aee96-111">Permission type</span></span> | <span data-ttu-id="aee96-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="aee96-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="aee96-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aee96-113">Delegated (work or school account)</span></span>| <span data-ttu-id="aee96-114">Printer.Read.All, Printer.ReadWrite.All, Printer.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="aee96-114">Printer.Read.All, Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="aee96-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aee96-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aee96-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aee96-116">Not Supported.</span></span>|
|<span data-ttu-id="aee96-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="aee96-117">Application</span></span>| <span data-ttu-id="aee96-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aee96-118">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="aee96-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aee96-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers/{id}/getCapabilities
```
## <a name="request-headers"></a><span data-ttu-id="aee96-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="aee96-120">Request headers</span></span>
| <span data-ttu-id="aee96-121">Имя</span><span class="sxs-lookup"><span data-stu-id="aee96-121">Name</span></span>          | <span data-ttu-id="aee96-122">Описание</span><span class="sxs-lookup"><span data-stu-id="aee96-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="aee96-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="aee96-123">Authorization</span></span> | <span data-ttu-id="aee96-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aee96-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="aee96-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="aee96-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="aee96-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="aee96-127">Response</span></span>
<span data-ttu-id="aee96-128">В случае успешного использования этот метод возвращает код отклика и `200 OK` [объект printerCapabilities](../resources/printercapabilities.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="aee96-128">If successful, this method returns a `200 OK` response code and a [printerCapabilities](../resources/printercapabilities.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aee96-129">Пример</span><span class="sxs-lookup"><span data-stu-id="aee96-129">Example</span></span>
<span data-ttu-id="aee96-130">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="aee96-130">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="aee96-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="aee96-131">Request</span></span>
<span data-ttu-id="aee96-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aee96-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="aee96-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="aee96-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "printer-getCapabilities"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/{id}/getCapabilities
```
# <a name="c"></a>[<span data-ttu-id="aee96-134">C#</span><span class="sxs-lookup"><span data-stu-id="aee96-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/printer-getcapabilities-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="aee96-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="aee96-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/printer-getcapabilities-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="aee96-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="aee96-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/printer-getcapabilities-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="aee96-137">Java</span><span class="sxs-lookup"><span data-stu-id="aee96-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/printer-getcapabilities-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="aee96-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="aee96-138">Response</span></span>
<span data-ttu-id="aee96-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="aee96-139">The following is an example of the response.</span></span>
><span data-ttu-id="aee96-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="aee96-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
