---
title: 'принтер: getCapabilities'
description: Получите список возможностей для принтера.
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: e82886850e577efe4cd30f1aaa1bac989aacea07
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62343973"
---
# <a name="printer-getcapabilities"></a>принтер: getCapabilities

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получите список возможностей для [принтера](../resources/printer.md).

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

Чтобы использовать службу универсальной печати, пользователь или клиент приложения должен иметь активную подписку универсальной печати в дополнение к разрешениям, перечисленным в следующей таблице. Подписанный пользователь должен быть [администратором принтера](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).

|Тип разрешения | Разрешения (в порядке повышения привилегий) |
|:---------------|:--------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)| Printer.Read.All, Printer.ReadWrite.All, Printer.FullControl.All |
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение| Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers/{id}/getCapabilities
```
## <a name="request-headers"></a>Заголовки запросов
| Имя          | Описание   |
|:--------------|:--------------|
| Авторизация | Bearer {token}. Обязательный. |

## <a name="request-body"></a>Текст запроса

## <a name="response"></a>Отклик
В случае успешного использования этот метод возвращает код `200 OK` отклика и [объект printerCapabilities](../resources/printercapabilities.md) в тексте отклика.

## <a name="example"></a>Пример
В приведенном ниже примере показано, как вызывать этот API.
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "printer-getCapabilities"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/{id}/getCapabilities
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/printer-getcapabilities-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/printer-getcapabilities-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/printer-getcapabilities-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/printer-getcapabilities-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/printer-getcapabilities-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/printer-getcapabilities-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>Отклик
Ниже приведен пример отклика.
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printerCapabilities"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

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
