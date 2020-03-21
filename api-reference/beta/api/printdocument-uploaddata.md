---
title: 'printDocument: Уплоаддата'
description: Отправьте один двоичный сегмент printDocument.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 7592de07f74aa6fb715a90b2becad57a0e14b194
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/21/2020
ms.locfileid: "42896302"
---
# <a name="printdocument-uploaddata"></a>printDocument: Уплоаддата

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Отправьте один двоичный сегмент **printDocument**.

Вы можете отправить файл целиком или разбить его на несколько диапазонов байтов, если число запросов не превышает 1 МБ.

Сегменты файла можно отправить в любом порядке и можно отправить параллельно, используя до четырех одновременных запросов. После отправки всех двоичных сегментов документа двоичный файл связывается с **методом printJob**.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

В дополнение к следующим разрешениям клиент пользователя должен иметь активную универсальную подписку на печать.

|Тип разрешения | Разрешения (в порядке повышения привилегий) |
|:---------------|:--------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)| Users. Read. ALL |
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложения|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/{id}/jobs/{id}/documents/{id}/uploadData
```
## <a name="request-headers"></a>Заголовки запросов
| Имя          | Описание   |
|:--------------|:--------------|
| Авторизация | Bearer {токен}. Обязательный. |
| Диапазон | байт = {Стартбитеиндекс} — {Ендбитеиндекс}  |
| Content-Length | ContentLength  |
| Content-Type  | application/json. Обязательный.|

## <a name="request-body"></a>Основной текст запроса
Текст запроса представляет собой двоичный объект BLOB, содержащий байты документа, которые задаются в `Range` заголовке как инклюзивный диапазон байтов. 

## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает один из следующих ответов. В тексте отклика не возвращается никаких данных.

| Условие     | Код ответа |
|:--------------|:--------------|
| Один или несколько двоичных сегментов по-прежнему необходимо отправить | `202 Accepted` |
| Все двоичные сегменты успешно отправлены | `201 Created` |

## <a name="example"></a>Пример
В приведенном ниже примере показано, как вызвать этот API, чтобы отправить первые 72797 байтов документа.
##### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "printdocument-uploaddata"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/{id}/jobs/{id}/documents/{id}/uploadData
Range: bytes=0-72796
Content-Length: 72797
```
##### <a name="response"></a>Отклик

Отсутствует один или несколько сегментов:
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printDocument"
} -->
```http
HTTP/1.1 202 Accepted
```

Все принимаемые сегменты:
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printDocument"
} -->
```http
HTTP/1.1 201 Created
```