---
title: 'todoTaskList: delta'
description: Получите набор ресурсов todoTaskList, которые были добавлены, удалены или удалены в Microsoft To Do.
ms.localizationpriority: medium
author: avijityadav
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: ca81f053936e93fd5cecc31c285a739d5109a170
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/12/2021
ms.locfileid: "60943061"
---
# <a name="todotasklist-delta"></a>todoTaskList: delta

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получите набор ресурсов [todoTaskList,](../resources/todotasklist.md) которые были добавлены, удалены или удалены в Microsoft To Do.

Вызов  функции дельты **для todoTaskList** похож на запрос GET, [](/graph/delta-query-overview) за исключением того, что при надлежащем применении маркеров состояния в одном или более из этих вызовов можно запрашивать дополнительные изменения в **todoTaskList**. Это позволяет поддерживать и синхронизировать локальный магазин **todoTaskList** пользователя без необходимости получать все **todoTaskList** с сервера каждый раз.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).


|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Tasks.ReadWrite    |
|Делегированные (личная учетная запись Майкрософт) | Tasks.ReadWrite    |
|Для приложений | Не поддерживается |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
GET /me/todo/lists/delta
GET /users/{id|userPrincipalName}/todo/lists/delta
```

## <a name="query-parameters"></a>Параметры запроса

Отслеживание изменений **в ресурсах todoTaskList** вызывает один или несколько вызовов функций **дельты.** Если вы используете параметры запроса, отличные от `$deltatoken` и `$skiptoken`, их необходимо указать в начальном запросе **delta**. Microsoft Graph автоматически кодирует указанные параметры в маркере, входящем в состав URL-адреса `nextLink` или `deltaLink`, включенного в отклик. Параметры запроса нужно указать только один раз в первом запросе. В последующих запросах просто скопируйте и примените URL-адрес из предыдущего ответа, так как этот URL-адрес уже содержит закодированные `nextLink` `deltaLink` и нужные параметры.

| Параметр запроса      | Тип   |Описание|
|:---------------|:--------|:----------|
| $deltatoken | string | Маркер [состояния,](/graph/delta-query-overview) возвращенный в URL-адрес предыдущей функции дельты, должен вызывать ту же коллекцию `deltaLink` **todoTaskList,** что указывает на завершение этого раунда отслеживания изменений.  Сохраните URL-адрес `deltaLink` с этим токеном и примените его в первом запросе следующего цикла отслеживания изменений для этой коллекции.|
| $skiptoken | string | Маркер [состояния,](/graph/delta-query-overview) возвращенный в URL-адрес предыдущего вызова функции дельты, указывает на то, что в том же `nextLink` **собрании todoTaskList** необходимо отслеживать дальнейшие изменения.  |

### <a name="odata-query-parameters"></a>Параметры запросов OData

Вы можете использовать параметр запроса `$select` так же, как в любом другом запросе GET, чтобы задать только те свойства, которые необходимы для эффективной работы. Свойство _id_ возвращается всегда. 

## <a name="request-headers"></a>Заголовки запросов
| Имя       | Тип | Описание |
|:---------------|:----------|:----------|
| Authorization  | string  | Bearer {token}. Обязательный. |
| Content-Type  | string  | application/json. Обязательный. |
| Prefer | string  | odata.maxpagesize={x}. Необязательный параметр. |

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код ответа и объект `200 OK` [коллекции todoTaskList](../resources/todotasklist.md) в тексте ответа.

## <a name="example"></a>Пример
### <a name="request"></a>Запрос
В следующем примере показано, как сделать начальный вызов функции дельты и ограничить максимальное число **todoTaskList** в теле ответа 2. 

Чтобы отслеживать изменения **в todoTaskList,** необходимо  сделать один или несколько вызовов функции дельты с соответствующими маркерами состояния, чтобы получить набор дополнительных изменений после последнего запроса дельты. 

Основные различия между отслеживанием **todoTaskList** и отслеживанием ресурсов **todoTask** в списке находятся в URL-адресах запроса запроса дельты и ответов на запросы, возвращающие **коллекции todoTaskList,** а не **todoTask.**

<!-- { "blockType": "ignored" } -->
``` http
GET https://graph.microsoft.com/beta/me/todo/lists/delta
Prefer: odata.maxpagesize=2
```
### <a name="response"></a>Отклик

В случае успешного выполнения запроса отклик будет содержать маркер состояния — _skipToken_  
или _deltaToken_. Первый включен в заголовок отклика _@odata.nextLink_, второй — в заголовок отклика _@odata.deltaLink_. Первый указывает на необходимость продолжать цикл, второй — на наличие всех изменений для определенного цикла.

Ниже показан отклик с маркером состояния _skipToken_ в заголовке отклика _@odata.nextLink_.

Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.deltaLink":"https://graph.microsoft.com/beta/me/todo/lists/delta?$skiptoken=ldfdgdgfoT5csv4k99nvQqyku0jaGqMhc6XyFff5qQTQ7RJOr",
  "value": [
    {
      "@odata.etag":"W/\"4rfRVIPi9EqXgDbc8U7HGwADLLQ93w==\"",
         "displayName":"List1",
         "isOwner":true,
         "isShared":false,
         "wellknownListName":"none",
         "id":"AQMkADMwNTcyZjQzLTdkMGItNDdjMy04ZTYwLTJhYmUzNGI5ZD"
    }
  ]
}
```

## <a name="see-also"></a>См. также

- [Запрос изменений Microsoft Graph](/graph/delta-query-overview)

