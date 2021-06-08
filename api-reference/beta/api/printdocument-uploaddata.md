---
title: 'printDocument: uploadData'
description: Upload двоичный сегмент printDocument.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 6435a36e7713435dce3f38145d48083bdabcc532
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787599"
---
# <a name="printdocument-uploaddata"></a>printDocument: uploadData

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Upload двоичный сегмент **printDocument**.

Вы можете загрузить весь файл или разделить его на несколько диапазонов byte, если размер запроса не превышает 1 МБ.

Сегменты файла можно отправлять в любом порядке, в том числе параллельно (до четырех параллельных запросов). При загрузке всех двоичных сегментов документа двоичный файл связан с **printJob.**

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).

Помимо следующих разрешений, пользователь или клиент приложения должен иметь активную подписку на универсальную печать и иметь разрешение, которое предоставляет [доступ к принтеру Get.](printer-get.md)

|Тип разрешения | Разрешения (в порядке повышения привилегий) |
|:---------------|:--------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)| PrintJob.ReadWrite, PrintJob.ReadWrite.All |
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение| Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/{id}/jobs/{id}/documents/{id}/uploadData
```
## <a name="request-headers"></a>Заголовки запросов
| Имя          | Описание   |
|:--------------|:--------------|
| Авторизация | Bearer {токен}. Обязательный. |
| Range | bytes={startByteIndex}-{endByteIndex}  |
| Content-Length | {contentLength}  |
| Content-Type  | application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
Текст запроса — это большой двоичный объект, содержащий байты документа, указанные как инклюзивный диапазон байтов, в заголовке `Range`. 

## <a name="response"></a>Отклик
В случае успешной работы этот метод возвращает один из следующих ответов. Метод не возвращает данные в теле отклика.

| Условие     | Код ответа |
|:--------------|:--------------|
| Один или несколько двоичных сегментов по-прежнему необходимо загрузить | `202 Accepted` |
| Все двоичные сегменты успешно загружены | `201 Created` |

## <a name="example"></a>Пример
В следующем примере показано, как вызвать этот API, чтобы загрузить первые 72797 bytes документа.
##### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "printdocument-uploaddata"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/{id}/jobs/{id}/documents/{id}/uploadData
Range: bytes=0-72796
Content-Length: 72797
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/printdocument-uploaddata-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/printdocument-uploaddata-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/printdocument-uploaddata-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/printdocument-uploaddata-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a>Отклик

Отсутствуют один или несколько сегментов:
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 202 Accepted
```

Все полученные сегменты:
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printDocument"
} -->
```http
HTTP/1.1 201 Created
```


