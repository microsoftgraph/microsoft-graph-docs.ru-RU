---
title: Загрузка двоичного файла printDocument
description: Скачайте двоичный файл, связанный с документом.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: a7e7de914d8549472e08c23f65af25ca99542a58
ms.sourcegitcommit: 3c0fa2d13ede0fdfa66d966d4ec32cb468c3befa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/25/2020
ms.locfileid: "48273660"
---
# <a name="download-printdocument-binary-file"></a>Загрузка двоичного файла printDocument

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Скачайте двоичный файл, связанный с [printDocument](../resources/printdocument.md). При вызове этого метода выдается ответ перенаправления с URL-адресом, предварительно прошедший проверку подлинности, который можно использовать для загрузки полезных данных.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

В дополнение к следующим разрешениям пользователь или клиент приложения должен иметь активную универсальную подписку на печать и иметь разрешение на получение доступа к [принтеру](printer-get.md) .

| Тип разрешения                        | Разрешения (в порядке повышения привилегий)                  |
| :------------------------------------- | :----------------------------------------------------------- |
| Делегированные (рабочая или учебная учетная запись)     | PrintJob. Read, PrintJob. Read. ALL, PrintJob. ReadWrite, PrintJob. ReadWrite. ALL |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается.                                               |
| Приложение                            | PrintJob. Read. ALL, PrintJob. ReadWrite. ALL                    |

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
В случае успешного выполнения этот метод возвращает `302 Found` URL-адрес скачивания, предварительно прошедший проверку подлинности, в заголовке Location.

## <a name="examples"></a>Примеры
В приведенном ниже примере показано, как вызвать этот API, чтобы получить URL-адрес для скачивания, прошедший проверку подлинности. Чтобы начать загрузку, следуйте указаниям URL-адреса перенаправления в ответе.

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "get_document_value"
}-->
```http
GET https://graph.microsoft.com/beta/print/printers/fcb0bc53-a446-41d0-bfc3-5c56cdbb0f2a/jobs/46140/documents/bd260b1a-044e-4ca6-afa9-17d9a587d254/$value
```

### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 302 Accepted
Location: https://print.print.microsoft.com/downloads/bd260b1a-044e-4ca6-afa9-17d9a587d254?tempauthtoken={accesstoken}
```
