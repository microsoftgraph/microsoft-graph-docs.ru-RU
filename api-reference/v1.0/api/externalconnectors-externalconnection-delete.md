---
title: Удаление externalConnection
description: Удаляет объект externalConnection.
author: mecampos
ms.localizationpriority: medium
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 89ba0cb06e9d84b6a6f83fab3f433be4dcaadfe2
ms.sourcegitcommit: dae41f5828677b993ba89f38c1d1c42d91c0ba02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2022
ms.locfileid: "65133743"
---
# <a name="delete-externalconnection"></a>Удаление externalConnection
Пространство имен: microsoft.graph.externalConnectors



Удаляет объект [externalConnection](../resources/externalconnectors-externalconnection.md) .

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированное (рабочая или учебная учетная запись)|ExternalConnection.ReadWrite.OwnedBy, ExternalConnection.ReadWrite.All|
|Делегированное (личная учетная запись Майкрософт)|Неприменимо|
|Приложение| ExternalConnection.ReadWrite.OwnedBy, ExternalConnection.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /external/connections/{connectionsId}
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос



# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_externalconnection"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/external/connections/contosohr
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-externalconnection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-externalconnection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-externalconnection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-externalconnection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/delete-externalconnection-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/delete-externalconnection-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---




### <a name="response"></a>Отклик
Ниже приведен пример отклика.

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
```

