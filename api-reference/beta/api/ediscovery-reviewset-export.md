---
title: 'reviewSet: экспорт'
description: Инициировать экспорт из reviewSet.
author: mahage-msft
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: f4e431bf23f73d482d9fd9fa2eae929f125a3dc4
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62347708"
---
# <a name="reviewset-export"></a>reviewSet: экспорт

Пространство имен: microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Инициировать экспорт из **reviewSet**.  Подробные сведения см. [в материале Экспорт документов из набора обзоров в Advanced eDiscovery](/microsoft-365/compliance/export-documents-from-review-set).

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|eDiscovery.Read.All, eDiscovery.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/reviewsets/{reviewsetId}/export
```

## <a name="request-headers"></a>Заголовки запросов

|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса

В теле запроса поставляем представление JSON параметров.

В следующей таблице указаны параметры, которые можно использовать с этим действием.

|Параметр|Тип|Описание|
|:---|:---|:---|
|outputName|String| Имя экспорта. Обязательный. |
|description|String| Описание экспорта |
|azureBlobContainer|String| При экспорте в собственную учетную запись хранения Azure это URL-адрес контейнера. |
|azureBlobToken|String| При экспорте на собственную учетную запись хранения Azure маркер SAS для URL-адреса контейнера. |
|ExportOptions| [microsoft.graph.ediscovery.exportOptions](../resources/ediscovery-caseexportoperation.md#exportoptions-values) |Указывает параметры, которые контролируют формат экспорта. Возможные значения: `originalFiles`, `text`, `pdfReplacement`, `fileInfo`, `tags`.|
|exportStructure|[microsoft.graph.ediscovery.exportFileStructure](../resources/ediscovery-caseexportoperation.md#exportfilestructure-values)| Параметры, которые контролируют структуру файлов и упаковку экспорта. Возможные значения: `none`, `directory`, `pst`.|

## <a name="response"></a>Отклик

Если экспорт успешно запущен, это действие возвращает код `202 Accepted` ответа. В ответе также будет содержаться `Location` заглавный загот, содержащий расположение [caseExportOperation](../resources/ediscovery-caseexportoperation.md) , созданного для обработки экспорта. Проверьте состояние экспортной операции, сделав запрос GET в расположение, после успешного завершения [состояние изменится на](../resources/ediscovery-caseoperation.md#caseoperationstatus-values) `succeeded`.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reviewset_export"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/99e865fc-e29f-479a-ba83-9e58eb017103/reviewsets/e44ac2cb-f8b4-4fd8-aa1c-1391b46ba9cc/export
Content-Type: application/json

{
  "outputName": "2020-12-06 Contoso investigation export",
  "description": "Export for the Contoso investigation",
  "exportOptions": "originalFiles,fileInfo,tags",
  "exportStructure": "directory"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reviewset-export-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reviewset-export-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reviewset-export-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reviewset-export-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/reviewset-export-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/reviewset-export-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 202 Accepted
cache-control: no-cache,
client-request-id: 3ec98906-7187-927e-5203-2ed4533175c6,
location: https://graph.microsoft.com/beta/compliance/ediscovery/cases('5b840b94-f821-4c4a-8cad-3a90062bf51a')/operations('2ad2da7c7dbb404abfbbb28b7b6babd6'),
request-id: 9e6b9230-113c-49de-8f7d-ecb90d35b0de
```
