---
title: 'todoTaskList: delta'
description: Получение набора ресурсов todoTaskList, которые были добавлены, удалены или удалены в Microsoft To Do.
localization_priority: Normal
author: avijityadav
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: b5d3acdc5b4b052744c26e95564c0e5abe1660ca
ms.sourcegitcommit: 1f8dc8750a50fb624a33e1d6360d29af38fa9514
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/21/2020
ms.locfileid: "46850059"
---
# <a name="todotasklist-delta"></a>todoTaskList: delta

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение набора ресурсов [todoTaskList,](../resources/todotasklist.md) которые были добавлены, удалены или удалены в Microsoft To Do.

Вызов **функции delta** **для todoTaskList** аналогичен запросу GET, за исключением того, что правильно применяя [маркеры состояния](/graph/delta-query-overview) в одном или нескольких из этих вызовов, вы можете запросить добавочные изменения в **todoTaskList.** Это позволяет поддерживать и синхронизировать локальное **хранилище списка todoTaskList пользователя,** при этом при этом не требуется каждый раз извлечь с сервера весь список **todoTaskList.**

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

Отслеживание изменений в **ресурсах todoTaskList** указывает на цикл из одного или **нескольких вызовов функции дельтирования.** Если вы используете параметры запроса, отличные от `$deltatoken` и `$skiptoken`, их необходимо указать в начальном запросе **delta**. Microsoft Graph автоматически кодирует указанные параметры в маркере, входящем в состав URL-адреса `nextLink` или `deltaLink`, включенного в отклик. Параметры запроса нужно указать только один раз в первом запросе. В последующих запросах просто скопируйте и примените `nextLink` `deltaLink` или введите URL-адрес из предыдущего ответа, так как в нем уже содержатся закодированные параметры.

| Параметр запроса      | Тип   |Описание|
|:---------------|:--------|:----------|
| $deltatoken | string | Маркер [состояния, возвращенный](/graph/delta-query-overview) в `deltaLink` URL-адресе предыдущего **вызова функции delta** для **той же коллекции todoTaskList** и указывает на завершение этого цикла отслеживания изменений. Сохраните URL-адрес `deltaLink` с этим токеном и примените его в первом запросе следующего цикла отслеживания изменений для этой коллекции.|
| $skiptoken | строка | Маркер [состояния, возвращаемый](/graph/delta-query-overview) в `nextLink` URL-адресе предыдущего **вызова функции delta** и указывающий, что в той же **коллекции todoTaskList остаются не** все изменения. |

### <a name="odata-query-parameters"></a>Параметры запросов OData

Вы можете использовать параметр запроса `$select` так же, как в любом другом запросе GET, чтобы задать только те свойства, которые необходимы для эффективной работы. Свойство _id_ возвращается всегда. 

## <a name="request-headers"></a>Заголовки запросов
| Имя       | Тип | Описание |
|:---------------|:----------|:----------|
| Authorization  | string  | Bearer {токен}. Обязательный. |
| Content-Type  | string  | application/json. Обязательный. |
| Prefer | string  | odata.maxpagesize={x}. Необязательный параметр. |

## <a name="response"></a>Отклик

При успешном выполнении этот метод возвращает `200 OK` код ответа [и объект коллекции todoTaskList](../resources/todotasklist.md) в тексте отклика.

## <a name="example"></a>Пример
### <a name="request"></a>Запрос
В следующем примере показано, как выполнить один **вызов функции delta** и ограничить максимальное количество **объектов todoTaskList** в теле отклика до 2.

Чтобы отследить изменения **в todoTaskList,** выполните один или несколько **разностных** вызовов функции с соответствующими маркерами состояния, чтобы получить набор добавочных изменений с момента последнего разностного запроса. 

Основные различия между **отслеживанием ресурса todoTaskList** и **ресурсами todoTask** в списке представлены в URL-адресах запроса изменений, а ответы возвращают **объект ы todoTaskList,** а не **коллекции todoTask.**

### <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
``` http
GET https://graph.microsoft.com/beta/me/todo/lists/delta?$skiptoken=l7WI41swwioT5csv4k99nvQqyku0jaGqMhc6XyFff5qQTQ7RJOr
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
Content-length: 254

{
  "@odata.deltaLink":"https://graph.microsoft.com/beta/me/todo/lists/delta?$skiptoken=ldfdgdgfoT5csv4k99nvQqyku0jaGqMhc6XyFff5qQTQ7RJOr",
  "value": [
    {
      "@odata.etag":"W/\"4rfRVIPi9EqXgDbc8U7HGwADLLQ93w==\"",
         "displayName":"List1",
         "isOwner":true,
         "isShared":false,
         "wellknownListName":"none",
         "id":"AQMkADMwNTcyZjQzLTdkMGItNDdjMy04ZTYwLTJhYmUzNGI5ZD
    }
  ]
}
```

## <a name="see-also"></a>См. также

- [Запрос изменений Microsoft Graph](/graph/delta-query-overview)