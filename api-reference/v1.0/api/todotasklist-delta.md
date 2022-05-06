---
title: 'todoTaskList: delta'
description: Получение набора ресурсов todoTaskList, которые были добавлены, удалены или удалены в Список дел Microsoft.
ms.localizationpriority: medium
author: avijityadav
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 0259b84ba88ce6536c9eb8a5828010ff4b947351
ms.sourcegitcommit: 972d83ea471d1e6167fa72a63ad0951095b60cb0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2022
ms.locfileid: "65247289"
---
# <a name="todotasklist-delta"></a>todoTaskList: delta

Пространство имен: microsoft.graph

Получение набора ресурсов [todoTaskList](../resources/todotasklist.md), которые были добавлены, удалены или удалены в Список дел Microsoft.

Вызов **разностной** функции **для todoTaskList** аналогичен запросу GET, за исключением того, [](/graph/delta-query-overview) что путем соответствующего применения маркеров состояния в одном или нескольких из этих вызовов можно запросить добавочные изменения в **todoTaskList**. Это позволяет поддерживать и синхронизировать локальное хранилище **todoTaskList** пользователя без необходимости каждый раз получать все **todoTaskList** с сервера.

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

Отслеживание изменений в **ресурсах todoTaskList** вызывает один или несколько вызовов **разностных** функций. Если вы используете параметры запроса, отличные от `$deltatoken` и `$skiptoken`, их необходимо указать в начальном запросе **delta**. Microsoft Graph автоматически кодирует указанные параметры в маркере, входящем в состав URL-адреса `@odata.nextLink` или `@odata.deltaLink`, включенного в отклик. Параметры запроса нужно указать только один раз в первом запросе. В последующих запросах `@odata.nextLink` `@odata.deltaLink` просто скопируйте и примените URL-адрес из предыдущего ответа, так как этот URL-адрес уже содержит закодированные требуемые параметры.

| Параметр запроса      | Тип   |Описание|
|:---------------|:--------|:----------|
| $deltatoken | string | Маркер [состояния,](/graph/delta-query-overview) возвращенный `@odata.deltaLink` в URL-адресе предыдущего вызова разностной функции для той же коллекции **todoTaskList**, указывающий на завершение этого цикла отслеживания изменений. Сохраните URL-адрес `@odata.deltaLink` с этим токеном и примените его в первом запросе следующего цикла отслеживания изменений для этой коллекции.|
| $skiptoken | string | Маркер [состояния,](/graph/delta-query-overview) возвращенный `@odata.nextLink` в URL-адресе предыдущего вызова функции delta, указывающий на то, что в той же коллекции **todoTaskList** будут отслеживаться дальнейшие изменения. |

### <a name="odata-query-parameters"></a>Параметры запросов OData

Вы можете использовать параметр запроса `$select` так же, как в любом другом запросе GET, чтобы задать только те свойства, которые необходимы для эффективной работы. Свойство _id_ возвращается всегда. 

## <a name="request-headers"></a>Заголовки запросов
| Имя       | Тип | Описание |
|:---------------|:----------|:----------|
| Authorization  | string  | Bearer {token}. Обязательный. |
| Content-Type  | string  | application/json. Обязательный. |
| Prefer | string  | odata.maxpagesize={x}. Необязательный параметр. |

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код `200 OK` отклика и объект коллекции [todoTaskList](../resources/todotasklist.md) в тексте отклика.

## <a name="example"></a>Пример
### <a name="request"></a>Запрос
В следующем примере показано, как выполнить  начальный вызов функции delta и ограничить максимальное число **todoTaskList** в тексте ответа 2.

Чтобы отслеживать изменения в **todoTaskList**, необходимо выполнить один или несколько вызовов  разностных функций с соответствующими маркерами состояния, чтобы получить набор добавочных изменений с момента последнего разностного запроса. 

Основные различия между отслеживанием **todoTaskList** и ресурсами **отслеживания todoTask** в списке находятся в URL-адресах разностных запросов и ответах запросов, возвращаемых **todoTaskList** , а не **коллекциях todoTask** .

<!-- { "blockType": "ignored" } -->
``` http
GET https://graph.microsoft.com/v1.0/me/todo/lists/delta
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
  "@odata.deltaLink":"https://graph.microsoft.com/v1.0/me/todo/lists/delta?$skiptoken=ldfdgdgfoT5csv4k99nvQqyku0jaGqMhc6XyFff5qQTQ7RJOr",
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

