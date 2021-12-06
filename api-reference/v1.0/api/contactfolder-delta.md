---
title: 'contactFolder: delta'
description: Получение набора папок контактов, которые были добавлены в почтовый ящик пользователя или удалены из него.
ms.localizationpriority: medium
author: kevinbellinger
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: ae7895e5a8056123a744a5564eb197abc2d5249a
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "61020222"
---
# <a name="contactfolder-delta"></a>contactFolder: delta

Пространство имен: microsoft.graph

Получение набора папок контактов, которые были добавлены в почтовый ящик пользователя или удалены из него.

Вызов функции **delta** для папок контактов в почтовом ящике похож на запрос GET. С тем исключением, что можно запрашивать добавочные изменения в папках контактов, правильно применяя [маркеры состояния](/graph/delta-query-overview) при этих вызовах. Это позволяет обслуживать и синхронизировать локальное хранилище папок контактов пользователя, не загружая каждый раз все папки контактов этого почтового ящика с сервера.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).


|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Contacts.Read, Contacts.ReadWrite    |
|Делегированные (личная учетная запись Майкрософт) | Contacts.Read, Contacts.ReadWrite    |
|Для приложений | Contacts.Read, Contacts.ReadWrite |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders/delta
GET /users/{id}/contactFolders/delta
```

## <a name="query-parameters"></a>Параметры запроса

Отслеживание изменений в папках контактов представляет собой цикл из одного или нескольких вызовов функции **delta**. Если вы используете параметры запроса, отличные от `$deltatoken` и `$skiptoken`, их необходимо указать в начальном запросе **delta**. Microsoft Graph автоматически кодирует указанные параметры в токене (`skiptoken` или `$deltatoken`), входящем в состав URL-адреса `nextLink` или `deltaLink`, который включен в отклик. Параметры запроса нужно указать только один раз в первом запросе. Копируйте URL-адрес `nextLink` или `deltaLink` из предыдущего отклика и применяйте его в последующих запросах, так как он уже содержит необходимые закодированные параметры.

| Параметр запроса      | Тип   |Описание|
|:---------------|:--------|:----------|
| $deltatoken | string | Этот [маркер состояния](/graph/delta-query-overview) возвращается в URL-адресе `deltaLink` при предыдущем вызове функции **delta** для той же коллекции папок контактов и указывает на завершение этого цикла отслеживания изменений. Сохраните URL-адрес `deltaLink` с этим токеном и примените его в первом запросе следующего цикла отслеживания изменений для этой коллекции.|
| $skiptoken | string | Этот [маркер состояния](/graph/delta-query-overview) возвращается в URL-адресе `nextLink` при предыдущем вызове функции **delta** и указывает, что из коллекции папок контактов получены не все изменения. |

### <a name="odata-query-parameters"></a>Параметры запросов OData

Вы можете использовать параметр запроса `$select` так же, как в любом другом запросе GET, чтобы задать только те свойства, которые необходимы для эффективной работы. Свойство _id_ возвращается всегда. 

## <a name="request-headers"></a>Заголовки запросов
| Имя       | Тип | Описание |
|:---------------|:----------|:----------|
| Authorization  | string  | Bearer {token}. Обязательный. |
| Content-Type  | string  | application/json. Обязательный. |
| Prefer | string  | odata.maxpagesize={x}. Необязательный параметр. |

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект коллекции [contactFolder](../resources/contactfolder.md) в теле отклика.

## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
В следующем примере показано, как выполнить один вызов функции **delta** и ограничить максимальное количество папок контактов в теле отклика двумя.

Чтобы отследить изменения в папках контактов почтового ящика, выполните один или несколько вызовов функции **delta** с правильными маркерами состояния, чтобы получить набор добавочных изменений с момента последнего разностного запроса. 

Пример, в котором показано, как использовать маркеры состояния для отслеживания изменений сообщений в почтовой папке: [Получение добавочных изменений сообщений в папке](/graph/delta-query-messages). Отслеживания папок контактов и отслеживания сообщений в папках отличаются, прежде всего, URL-адресами разностных запросов и возвращаемыми в откликах коллекциями (**contactFolder** и **message** соответственно).


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "contactfolder_delta"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/contactFolders/delta
Prefer: odata.maxpagesize=2
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/contactfolder-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/contactfolder-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/contactfolder-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/contactfolder-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/contactfolder-delta-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>Отклик

В случае успешного выполнения запроса отклик будет содержать маркер состояния — _skipToken_  
или _deltaToken_. Первый включен в заголовок отклика _@odata.nextLink_, второй — в заголовок отклика _@odata.deltaLink_. Первый указывает на необходимость продолжать цикл, второй — на наличие всех изменений для определенного цикла.

Ниже показан отклик с маркером состояния _skipToken_ в заголовке отклика _@odata.nextLink_.

Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactFolder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/me/contactfolders/delta?$skiptoken={_skipToken_}",
  "value": [
    {
     "parentFolderId": "parentFolderId-value",
      "displayName": "displayName-value",
      "id": "id-value"
    }
  ]
}
```

### <a name="see-also"></a>См. также

- [Отслеживание изменений данных Microsoft Graph с помощью запроса изменений](/graph/delta-query-overview)
- [Получение добавочных изменений сообщений в папке](/graph/delta-query-messages)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "contactFolder: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

