---
title: 'printDocument: Уплоаддата'
description: Отправьте один двоичный сегмент printDocument.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 10bf87d66126d85bdc52c69659647c7728084ac5
ms.sourcegitcommit: 9edfcf99706c8490cd5832a1c706a88a89e24db1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/07/2020
ms.locfileid: "42948102"
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
|Для приложений|Не поддерживается.|

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

## <a name="response"></a>Ответ
В случае успешного выполнения этот метод возвращает один из следующих ответов. В тексте отклика не возвращается никаких данных.

| Условие     | Код ответа |
|:--------------|:--------------|
| Один или несколько двоичных сегментов по-прежнему необходимо отправить | `202 Accepted` |
| Все двоичные сегменты успешно отправлены | `201 Created` |

## <a name="example"></a>Пример
В приведенном ниже примере показано, как вызвать этот API, чтобы отправить первые 72797 байтов документа.
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

---

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
