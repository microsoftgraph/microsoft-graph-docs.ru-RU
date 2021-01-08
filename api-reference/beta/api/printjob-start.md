---
title: 'printJob: start'
description: Отправка задания печати на связанный принтер или printerShare. Он будет печататься после завершения всех ожидающих заданий, отмены или отмены.
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: d2cb4a5413d592d170e31a882be93d900deca8c1
ms.sourcegitcommit: a0a5690ad9c109149e0b8c8baba164648ff5c226
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/08/2021
ms.locfileid: "49784802"
---
# <a name="printjob-start"></a>printJob: start

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Отправка задания печати на связанный [принтер](../resources/printer.md) или [printerShare.](../resources/printershare.md) Он будет печататься после  завершения, отмены или отмены всех ожидающих заданий.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

Помимо следующих разрешений, у пользователя или клиента приложения должна быть активная подписка [](printer-get.md) универсальной печати и разрешение на получение принтера или [get printerShare](printershare-get.md) в зависимости от того, используется ли принтер или printerShare.

|Тип разрешения | Разрешения (в порядке повышения привилегий) |
|:---------------|:--------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)| PrintJob.Create, PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All |
|Делегированное (личная учетная запись Майкрософт)|Не поддерживается.|
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
В случае успеха этот метод возвращает код отклика и объект `200 OK` [printJobStatus](../resources/printjobstatus.md) в теле.

## <a name="example"></a>Пример
В приведенном ниже примере показано, как вызывать этот API.
##### <a name="request"></a>Запрос

```http
POST https://graph.microsoft.com/beta/print/shares/{id}/jobs/{id}/start
```

##### <a name="response"></a>Отклик
Ниже приведен пример отклика. 
>**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.

```http
HTTP/1.1 200 OK

{
    "state": "processing",
    "description": "The print job is currently being processed.",
    "isAcquiredByPrinter": false,
    "details": ["interpreting"]
}
```


