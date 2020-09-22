---
title: Создание сеанса
description: 'Создайте новый сеанс книги. '
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 68d69c8dde26a0634604c60a01e3c30d9421a8ca
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47999036"
---
# <a name="create-session"></a>Создание сеанса

Пространство имен: microsoft.graph

Создайте новый сеанс книги. 

Интерфейсы API Excel можно вызвать в одном из двух режимов. 

1. Постоянный сеанс — все изменения, внесенные в книгу, сохраняются (сохраненные). Это обычный режим работы. 
2. Временный сеанс — изменения, внесенные интерфейсом API, не сохраняются в исходном расположении. Вместо этого внутренний сервер Excel сохраняет временную копию файла, в которой отражены изменения, внесенные во время конкретного сеанса API. Когда истечет срок действия сеанса Excel, изменения будут потеряны. Этот режим удобен для приложений, которым нужно выполнять анализ или получать результаты вычислений или изображение диаграммы, не изменяя состояние документа.   

Чтобы представить сеанс в API, используйте заголовок `workbook-session-id: {session-id}`. 

>**Примечание.** Заголовок сеанса не является обязательным для работы API Excel. Тем не менее мы рекомендуем использовать заголовок сеанса для повышения производительности. Если вы не используете заголовок сеанса, изменения, внесенные во время вызова API _сохраняются_ в файл.  

В некоторых случаях для создания нового сеанса требуется неопределенное время. Microsoft Graph также предоставляет шаблон операций длительного выполнения. Этот шаблон предоставляет способ опроса обновлений состояния создания, не дожидаясь завершения создания. Ниже описаны действия, которые следует выполнить.

1. В `Prefer: respond-async` запрос добавляется заголовок, указывающий на выполнение длительной операции.
2. В ответе возвращается `Location` заголовок, указывающий URL-адрес для опроса состояния операции создания. Вы можете получить состояние операции, обратившись к указанному URL-адресу. Состояние будет одним из следующих: `notStarted` ,, `running` `succeeded` , или `failed` .
3. После завершения операции можно запросить состояние повторно, а в ответе будет отображаться либо `succeeded` `failed` .

### <a name="error-handling"></a>Обработка ошибок

Иногда при выполнении этого запроса может отображаться сообщение об ошибке 504 HTTP. В этом случае нужно повторить запрос.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Files.ReadWrite    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/createSession
```
## <a name="request-headers"></a>Заголовки запросов
| Имя       | Описание|
|:---------------|:----------|
| Авторизация  | Bearer {токен}. Обязательный. |

## <a name="request-body"></a>Тело запроса
В теле запроса укажите представление JSON объекта [WorkbookSessionInfo](../resources/workbooksessioninfo.md).

## <a name="response"></a>Ответ

В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [workbookSessionInfo](../resources/workbooksessioninfo.md) в тексте отклика. Для длительной операции она возвращает `202 Accepted ` код отклика и `Location` заголовок с пустым текстом в ответе.

## <a name="examples"></a>Примеры

### <a name="example-1-basic-session-creation"></a>Пример 1: создание базового сеанса
#### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_excel_session"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/createSession
Content-type: application/json
Content-length: 52

{
  "persistChanges": true
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-excel-session-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-excel-session-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-excel-session-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>Отклик

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости. 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookSessionInfo"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "persistChanges": true
}
```
### <a name="example-2-session-creation-with-long-running-operation-pattern"></a>Пример 2: Создание сеанса с длительным шаблоном операции

#### <a name="request"></a>Запрос

```http
POST https://graph.microsoft.com/beta/me/drive/items/{drive-item-id}/workbook/worksheets({id})/createSession
Prefer: respond-async
Content-type: application/json
{
    "persistChanges": true
}
```

#### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости. 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookSessionInfo"
} -->
```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/v1.0/me/drive/items/{drive-item-id}/workbook/operations/{operation-id}
Content-type: application/json
{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


