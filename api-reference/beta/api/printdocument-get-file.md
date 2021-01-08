---
title: Скачивание двоичного файла printDocument
description: Скачайте двоичный файл, связанный с документом.
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: c56d1012e4b375be318f48f91cfb7e9f863b5704
ms.sourcegitcommit: a0a5690ad9c109149e0b8c8baba164648ff5c226
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/08/2021
ms.locfileid: "49784873"
---
# <a name="download-printdocument-binary-file"></a>Скачивание двоичного файла printDocument

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Скачайте двоичный файл, связанный с [printDocument.](../resources/printdocument.md) Вызов этого метода дает отклик перенаправления с URL-адресом с предварительной проверкой подлинности, который можно использовать для скачивания полезной нагрузки.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

Помимо следующих разрешений, у пользователя или клиента приложения должна быть активная подписка [](printer-get.md) универсальной печати и разрешение, которое предоставляет доступ к принтеру в случае маркеров доступа пользователя и разрешения printer.Read.All или Printer.ReadWrite.All приложения в случае маркеров доступа только для приложений. 

| Тип разрешения                        | Разрешения (в порядке повышения привилегий)                  |
| :------------------------------------- | :----------------------------------------------------------- |
| Делегированные (рабочая или учебная учетная запись)     | PrintJob.Read, PrintJob.Read.All, PrintJob.ReadWrite, PrintJob.ReadWrite.All |
| Делегированное (личная учетная запись Майкрософт) | Не поддерживается.                                               |
| Приложение                            | PrintJob.Read.All, PrintJob.ReadWrite.All                    |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers/{id}/jobs/{id}/documents/{id}/$value
```
## <a name="request-headers"></a>Заголовки запросов
| Имя          | Описание               |
| :------------ | :------------------------ |
| Авторизация | Bearer {токен}. Обязательный. |

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик
В случае успеха этот метод возвращает URL-адрес скачивания с предварительной проверкой подлинности `302 Found` в заголке Location.

## <a name="examples"></a>Примеры
В следующем примере показано, как вызвать этот API для получения URL-адреса скачивания с предварительной проверкой подлинности. Чтобы начать скачивание, следуйте URL-адресу перенаправления в ответе.

### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_document_value"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/fcb0bc53-a446-41d0-bfc3-5c56cdbb0f2a/jobs/46140/documents/bd260b1a-044e-4ca6-afa9-17d9a587d254/$value
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-document-value-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-document-value-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-document-value-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-document-value-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 302 Accepted
Location: https://print.print.microsoft.com/downloads/bd260b1a-044e-4ca6-afa9-17d9a587d254?tempauthtoken={accesstoken}
```
