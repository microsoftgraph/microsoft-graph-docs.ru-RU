---
title: 'subjectRightsRequest: getFinalReport'
description: Получите окончательный отчет для запроса на права субъекта.
author: skadam-msft
ms.localizationpriority: medium
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 77c517c1ef6742dc173562aca9e6188c75b085e5
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62131941"
---
# <a name="subjectrightsrequest-getfinalreport"></a>subjectRightsRequest: getFinalReport
Пространство имен: microsoft.graph

Получите окончательный отчет для запроса на права субъекта. Отчет — это текстовый файл, содержащий сведения о файлах, включенных администратором конфиденциальности.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|SubjectRightsRequest.Read.All, SubjectRightsRequest.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|Не поддерживается|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /privacy/subjectRightsRequests{subjectRightsRequestId}/getFinalReport
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Тело запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы эта функция возвращает код отклика и `200 OK` поток в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "subjectRightsRequest_getfinalreport"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/privacy/subjectRightsRequests/{subjectRightsRequestId}/getFinalReport
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/subjectrightsrequest-getfinalreport-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/subjectrightsrequest-getfinalreport-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/subjectrightsrequest-getfinalreport-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/subjectrightsrequest-getfinalreport-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/subjectrightsrequest-getfinalreport-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Edm.Stream"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Id, Workload, Size, ImmutableId, FileName, FilePath, ItemUrl
```

