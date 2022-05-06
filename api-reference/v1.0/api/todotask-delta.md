---
title: 'todoTask: delta'
description: Получение набора ресурсов todoTask, которые были добавлены, удалены или обновлены в указанном todoTaskList.
ms.localizationpriority: medium
author: avijityadav
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: f7e789de85a19fbbb41308e68f7a4d71a03f6919
ms.sourcegitcommit: 972d83ea471d1e6167fa72a63ad0951095b60cb0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2022
ms.locfileid: "65246939"
---
# <a name="todotask-delta"></a>todoTask: delta

Пространство имен: microsoft.graph

Получение набора ресурсов [todoTask](../resources/todotask.md) , которые были добавлены, удалены или обновлены в указанном [todoTaskList](../resources/todotasklist.md).

Вызов  разностной функции для ресурсов **todoTask** в **todoTaskList** аналогичен запросу GET, за исключением того, что [](/graph/delta-query-overview) путем соответствующего применения маркеров состояния в одном или нескольких из этих вызовов можно запросить добавочные изменения в **todoTask** в **этом todoTaskList**. Это позволяет поддерживать и синхронизировать локальное хранилище ресурсов **todoTask** пользователя, не извлекая весь набор данных с сервера каждый раз.  

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
GET /me/todo/lists/{id}/tasks/delta
GET /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/delta
```

## <a name="query-parameters"></a>Параметры запроса

Отслеживание изменений в **коллекции todoTask** вызывает цикл из одного или нескольких вызовов **разностных** функций. Если вы используете параметры запроса, отличные от `$deltatoken` и `$skiptoken`, их необходимо указать в начальном запросе **delta**. Microsoft Graph автоматически кодирует указанные параметры в маркере, входящем в состав URL-адреса `@odata.nextLink` или `@odata.deltaLink`, включенного в отклик. Параметры запроса нужно указать только один раз в первом запросе. В последующих запросах `@odata.nextLink` `@odata.deltaLink` просто скопируйте и примените URL-адрес из предыдущего ответа, так как этот URL-адрес уже содержит закодированные требуемые параметры.

| Параметр запроса      | Тип   |Описание|
|:---------------|:--------|:----------|
| $deltatoken | string | Маркер [состояния,](/graph/delta-query-overview) возвращенный `@odata.deltaLink` в URL-адресе предыдущего вызова разностной функции для той же коллекции todoTask, указывающий на завершение этого цикла отслеживания изменений. Сохраните URL-адрес `@odata.deltaLink` с этим токеном и примените его в первом запросе следующего цикла отслеживания изменений для этой коллекции.|
| $skiptoken | string | Маркер [состояния,](/graph/delta-query-overview) возвращенный `@odata.nextLink` в URL-адресе предыдущего вызова функции delta, указывающий на то, что в той же коллекции todoTask будут отслеживаться дальнейшие изменения. |

### <a name="odata-query-parameters"></a>Параметры запросов OData

- Вы можете использовать параметр запроса `$select` так же, как в любом другом запросе GET, чтобы задать только те свойства, которые необходимы для эффективной работы. Свойство _id_ возвращается всегда. 
- Поддержка разностных `$select`запросов `$top`и `$expand` todoTask. 
- Имеется ограниченная поддержка параметров `$filter` и `$orderby`:
  * Для параметра `$filter` поддерживаются только выражения `$filter=receivedDateTime+ge+{value}` и `$filter=receivedDateTime+gt+{value}`.
  * Для параметра `$orderby` поддерживается только выражение `$orderby=receivedDateTime+desc`. Если выражение `$orderby` не указано, результаты будут возвращаться в непредсказуемом порядке. 
- Параметр `$search` не поддерживается.

## <a name="request-headers"></a>Заголовки запросов
| Имя       | Тип | Описание |
|:---------------|:----------|:----------|
| Authorization  | string  | Bearer {token}. Обязательный. |
| Content-Type  | string  | application/json. Обязательный. |
| Prefer | string  | odata.maxpagesize={x}. Необязательный параметр. |

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код `200 OK` отклика и объект [коллекции todoTask](../resources/todotask.md) в тексте отклика.

## <a name="example"></a>Пример
### <a name="request"></a>Запрос
Чтобы отслеживать изменения в ресурсах **todoTask** в **todoTaskList** с момента последнего цикла отслеживания изменений, необходимо выполнить один или несколько вызовов разностных функций, чтобы получить набор добавочных изменений. В следующем примере показано, как начать следующий цикл отслеживания изменений, используя URL-адрес`@odata.deltaLink`, возвращенный из последнего вызова функции разностной функции последнего цикла, который содержит . `deltaToken` Этот **вызов разностной** функции ограничивает максимальное число **todoTask** в тексте ответа 2.
 

### <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
``` http
GET https://graph.microsoft.com/v1.0/me/todo/lists/gDbc8U7HGwADDZocJgAAAA==/tasks/delta?$deltatoken=w0vf2jHg2mBXU-I2AK0FSWl0dopNtG8u5YoM
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
   "@odata.deltaLink":"https://graph.microsoft.com/v1.0/me/todo/lists/gDbc8U7HGwADDZocJgAAAA==/tasks/delta?$deltatoken=MoVMZ_DzHG4AhT3WE8VioVS1IXZJ-ArqK5fknOjnKFY",
   "value":[
      {
         "@odata.etag":"W/\"4rfRVIPi9EqXgDbc8U7HGwADLLQ9xQ==\"",
         "importance":"normal",
         "isReminderOn":false,
         "status":"notStarted",
         "title":"empty task3",
         "createdDateTime":"2020-08-12T04:54:29.1925206Z",
         "lastModifiedDateTime":"2020-08-12T04:54:29.4903939Z",
         "id":"AAMkADMwNTcyZjQzLTdkMGItNDdjMy04ZTYwLTJhYmUzNGI5ZDEwMwBGAAAAAAB5M0K0qlJySLOAgV22zPnuBwDit9FUg_L0SpeANtzxTscbAAMNmhwmAADit9FUg_L0SpeANtzxTscbAAMxlnrYAAA=",
         "body":{
            "content":"",
            "contentType":"text"
         }
      }
   ]
}
```

## <a name="see-also"></a>См. также

- [Запрос изменений Microsoft Graph](/graph/delta-query-overview)

