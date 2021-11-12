---
title: 'todoTask: дельта'
description: Получите набор ресурсов todoTask, которые были добавлены, удалены или обновлены в указанном todoTaskList.
ms.localizationpriority: medium
author: avijityadav
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 6917a732189ce505da75baaf716a0a2ed583b007
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/12/2021
ms.locfileid: "60947058"
---
# <a name="todotask-delta"></a>todoTask: дельта

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получите набор ресурсов [todoTask,](../resources/todotask.md) которые были добавлены, удалены или обновлены в указанном [todoTaskList.](../resources/todotasklist.md)

Вызов  функции delta для ресурсов **todoTask** в **todoTaskList** похож на запрос GET, за исключением того, что при надлежащем применении маркеров состояния в одном или более из этих вызовов можно запрашивать дополнительные изменения в **todoTask** в том **todoTaskList**. [](/graph/delta-query-overview) Это позволяет поддерживать и синхронизировать локальный магазин ресурсов **todoTask** пользователя без необходимости каждый раз получать весь набор с сервера.  

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

Отслеживание изменений в **коллекции todoTask** вызывает один или несколько вызовов функций **дельты.** Если вы используете параметры запроса, отличные от `$deltatoken` и `$skiptoken`, их необходимо указать в начальном запросе **delta**. Microsoft Graph автоматически кодирует указанные параметры в маркере, входящем в состав URL-адреса `nextLink` или `deltaLink`, включенного в отклик. Параметры запроса нужно указать только один раз в первом запросе. В последующих запросах просто скопируйте и примените URL-адрес из предыдущего ответа, так как этот URL-адрес уже содержит закодированные `nextLink` `deltaLink` и нужные параметры.

| Параметр запроса      | Тип   |Описание|
|:---------------|:--------|:----------|
| $deltatoken | string | В [URL-адрес](/graph/delta-query-overview) предыдущей функции дельты возвращается маркер состояния для той же коллекции `deltaLink`  todoTask, что указывает на завершение этого раунда отслеживания изменений. Сохраните URL-адрес `deltaLink` с этим токеном и примените его в первом запросе следующего цикла отслеживания изменений для этой коллекции.|
| $skiptoken | string | Маркер [состояния,](/graph/delta-query-overview) возвращенный в URL-адрес предыдущего вызова функции дельты, указывает на то, что в той же `nextLink` коллекции  todoTask необходимо отслеживать дальнейшие изменения. |

### <a name="odata-query-parameters"></a>Параметры запросов OData

- Вы можете использовать параметр запроса `$select` так же, как в любом другом запросе GET, чтобы задать только те свойства, которые необходимы для эффективной работы. Свойство _id_ возвращается всегда. 
- Поддержка запросов Delta `$select` `$top` и `$expand` todoTask. 
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

В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект коллекции todoTask](../resources/todotask.md) в тексте ответа.

## <a name="example"></a>Пример
### <a name="request"></a>Запрос
Чтобы отслеживать изменения ресурсов **todoTask** в **todoTaskList** после последнего раунда отслеживания  изменений, необходимо сделать один или несколько вызовов функции дельты, чтобы получить набор дополнительных изменений. В следующем примере показано, как начать следующий раунд отслеживания изменений с использованием URL-адреса в последнем вызове функции дельты последнего раунда, который `deltaLink` содержит  `deltaToken` . Этот **вызов** функции дельты ограничивает максимальное число **todoTask** в теле ответа до 2.
 

### <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
``` http
GET https://graph.microsoft.com/beta/me/todo/lists/gDbc8U7HGwADDZocJgAAAA==/tasks/delta?$deltatoken=w0vf2jHg2mBXU-I2AK0FSWl0dopNtG8u5YoM
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
   "@odata.deltaLink":"https://graph.microsoft.com/beta/me/todo/lists/gDbc8U7HGwADDZocJgAAAA==/tasks/delta?$deltatoken=MoVMZ_DzHG4AhT3WE8VioVS1IXZJ-ArqK5fknOjnKFY",
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

