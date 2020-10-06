---
title: 'Тодотаск: Delta'
description: Получение набора ресурсов Тодотаск, добавленных, удаленных или обновленных в указанном Тодотасклист.
localization_priority: Normal
author: avijityadav
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 7433748c04b5ee79e6c8795661cec2e71eae9d41
ms.sourcegitcommit: 39e48ed2d95b142ccf3f40ecc52441458f2745bf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/06/2020
ms.locfileid: "48364385"
---
# <a name="todotask-delta"></a>Тодотаск: Delta

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение набора ресурсов [тодотаск](../resources/todotask.md) , добавленных, удаленных или обновленных в указанном [тодотасклист](../resources/todotasklist.md).

Вызов функции **Delta** для ресурсов **тодотаск** в **тодотасклист** аналогичен запросу Get, за исключением того, что при соответствующем применении [маркеров состояния](/graph/delta-query-overview) в одном или нескольких вызовах Вы можете запросить добавочные изменения в **тодотаск** в этом **тодотасклист**. Это позволяет поддерживать и синхронизировать локальное хранилище ресурсов **тодотаск** пользователя без необходимости каждый раз получать весь набор с сервера.  

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

Отслеживание изменений в коллекции **тодотаск** приводит к округлению одного или нескольких вызовов функции **Delta** . Если вы используете параметры запроса, отличные от `$deltatoken` и `$skiptoken`, их необходимо указать в начальном запросе **delta**. Microsoft Graph автоматически кодирует указанные параметры в маркере, входящем в состав URL-адреса `nextLink` или `deltaLink`, включенного в отклик. Параметры запроса нужно указать только один раз в первом запросе. При последующих запросах просто скопируйте и примените `nextLink` `deltaLink` URL-адрес из предыдущего ответа, так как этот URL-адрес уже включает закодированные, нужные параметры.

| Параметр запроса      | Тип   |Описание|
|:---------------|:--------|:----------|
| $deltatoken | string | [Токен состояния](/graph/delta-query-overview) возвращается в `deltaLink` URL-адресе предыдущего вызова функции **Delta** для той же коллекции тодотаск, что указывает на завершение этого круга отслеживания изменений. Сохраните URL-адрес `deltaLink` с этим токеном и примените его в первом запросе следующего цикла отслеживания изменений для этой коллекции.|
| $skiptoken | string | [Маркер состояния](/graph/delta-query-overview) возвращается в `nextLink` URL-адресе предыдущего вызова функции **Delta** , указывая, что в одной коллекции тодотаск есть изменения, которые необходимо отслеживать. |

### <a name="odata-query-parameters"></a>Параметры запросов OData

- Вы можете использовать параметр запроса `$select` так же, как в любом другом запросе GET, чтобы задать только те свойства, которые необходимы для эффективной работы. Свойство _id_ возвращается всегда. 
- Поддержка запросов Delta `$select` , `$top` и `$expand` для тодотаск. 
- Имеется ограниченная поддержка параметров `$filter` и `$orderby`:
  * Для параметра `$filter` поддерживаются только выражения `$filter=receivedDateTime+ge+{value}` и `$filter=receivedDateTime+gt+{value}`.
  * Для параметра `$orderby` поддерживается только выражение `$orderby=receivedDateTime+desc`. Если выражение `$orderby` не указано, результаты будут возвращаться в непредсказуемом порядке. 
- Параметр `$search` не поддерживается.

## <a name="request-headers"></a>Заголовки запросов
| Имя       | Тип | Описание |
|:---------------|:----------|:----------|
| Authorization  | string  | Bearer {токен}. Обязательный. |
| Content-Type  | string  | application/json. Обязательный. |
| Prefer | string  | odata.maxpagesize={x}. Необязательный параметр. |

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект коллекции [тодотаск](../resources/todotask.md) в тексте отклика.

## <a name="example"></a>Пример
### <a name="request"></a>Запрос
В приведенном ниже примере показано, как выполнить один вызов функции **Delta** и ограничить максимальное число **тодотаск** в тексте отклика до 2.

Чтобы отслеживать изменения в ресурсах **тодотаск** в **тодотасклист**, необходимо выполнить один или несколько вызовов функции **Delta** для получения набора добавочных изменений с момента последнего разностного запроса. 
 

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

Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 337

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

