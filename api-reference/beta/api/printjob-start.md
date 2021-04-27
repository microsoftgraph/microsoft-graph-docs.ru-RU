---
title: 'printJob: начните'
description: Отправка задания печати на связанный принтер или принтерShare. Она будет напечатана после завершения, отмены или отмены существующих ожидающих заданий.
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 288e3b8cfcd1458f7d71c8fb43ae57ac97237e56
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049879"
---
# <a name="printjob-start"></a>printJob: начните

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Отправка задания печати на [связанный](../resources/printer.md) принтер или [принтерShare](../resources/printershare.md). Он будет напечатан после завершения, отмены или отмены существующих ожидающих заданий. 

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

Помимо следующих разрешений, клиент пользователя или приложения должен иметь активную подписку на универсальную печать и иметь разрешение, которое предоставляет [get printer](printer-get.md) или Get printerShare в зависимости от того, используется принтер или [принтерShare.](printershare-get.md)

|Тип разрешения | Разрешения (в порядке повышения привилегий) |
|:---------------|:--------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)| PrintJob.Create, PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All |
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение| Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос
```http
POST /print/shares/{id}/jobs/{id}/start
```
## <a name="request-headers"></a>Заголовки запросов
| Имя          | Описание   |
|:--------------|:--------------|
| Авторизация | Bearer {токен}. Обязательный. |

## <a name="request-body"></a>Текст запроса

Не отправлять тело запроса для этого метода. 

## <a name="response"></a>Отклик
В случае успешной работы этот метод возвращает код отклика и `200 OK` объект [printJobStatus](../resources/printjobstatus.md) в теле.

## <a name="example"></a>Пример
В приведенном ниже примере показано, как вызывать этот API.
##### <a name="request"></a>Запрос

```http
POST https://graph.microsoft.com/beta/print/shares/{id}/jobs/{id}/start
```

##### <a name="response"></a>Отклик
Ниже приведен пример ответа. 
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

```http
HTTP/1.1 200 OK

{
    "state": "processing",
    "description": "The print job is currently being processed.",
    "isAcquiredByPrinter": false,
    "details": ["interpreting"]
}
```


