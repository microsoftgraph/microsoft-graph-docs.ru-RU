---
title: 'принтер: getCapabilities'
description: Получите список возможностей для принтера.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 2e3720014b3094d8d8696b6931f37586590b7d8a
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049914"
---
# <a name="printer-getcapabilities"></a><span data-ttu-id="80971-103">принтер: getCapabilities</span><span class="sxs-lookup"><span data-stu-id="80971-103">printer: getCapabilities</span></span>

<span data-ttu-id="80971-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="80971-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="80971-105">Получите список возможностей для [принтера.](../resources/printer.md)</span><span class="sxs-lookup"><span data-stu-id="80971-105">Get a list of capabilities for the [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="80971-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="80971-106">Permissions</span></span>
<span data-ttu-id="80971-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="80971-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="80971-109">Чтобы использовать службу универсальной печати, пользователь или клиент приложения должен иметь активную подписку универсальной печати в дополнение к разрешениям, перечисленным в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="80971-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="80971-110">Подписанный пользователем должен быть [администратором принтера.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="80971-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="80971-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="80971-111">Permission type</span></span> | <span data-ttu-id="80971-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="80971-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="80971-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="80971-113">Delegated (work or school account)</span></span>| <span data-ttu-id="80971-114">Printer.Read.All, Printer.ReadWrite.All, Printer.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="80971-114">Printer.Read.All, Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="80971-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="80971-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="80971-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="80971-116">Not Supported.</span></span>|
|<span data-ttu-id="80971-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="80971-117">Application</span></span>| <span data-ttu-id="80971-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="80971-118">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="80971-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="80971-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers/{id}/getCapabilities
```
## <a name="request-headers"></a><span data-ttu-id="80971-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="80971-120">Request headers</span></span>
| <span data-ttu-id="80971-121">Имя</span><span class="sxs-lookup"><span data-stu-id="80971-121">Name</span></span>          | <span data-ttu-id="80971-122">Описание</span><span class="sxs-lookup"><span data-stu-id="80971-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="80971-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="80971-123">Authorization</span></span> | <span data-ttu-id="80971-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="80971-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="80971-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="80971-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="80971-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="80971-127">Response</span></span>
<span data-ttu-id="80971-128">В случае успешного использования этот метод возвращает код отклика и `200 OK` [объект printerCapabilities](../resources/printercapabilities.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="80971-128">If successful, this method returns a `200 OK` response code and a [printerCapabilities](../resources/printercapabilities.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="80971-129">Пример</span><span class="sxs-lookup"><span data-stu-id="80971-129">Example</span></span>
<span data-ttu-id="80971-130">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="80971-130">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="80971-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="80971-131">Request</span></span>
<span data-ttu-id="80971-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="80971-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="80971-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="80971-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "printer-getCapabilities"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/{id}/getCapabilities
```
# <a name="c"></a>[<span data-ttu-id="80971-134">C#</span><span class="sxs-lookup"><span data-stu-id="80971-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/printer-getcapabilities-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="80971-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="80971-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/printer-getcapabilities-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="80971-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="80971-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/printer-getcapabilities-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="80971-137">Java</span><span class="sxs-lookup"><span data-stu-id="80971-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/printer-getcapabilities-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="80971-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="80971-138">Response</span></span>
<span data-ttu-id="80971-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="80971-139">The following is an example of the response.</span></span>
><span data-ttu-id="80971-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="80971-140">**Note:** The response object shown here might be shortened for readability.</span></span>
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
