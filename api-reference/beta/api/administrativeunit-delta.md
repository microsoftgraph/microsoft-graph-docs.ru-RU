---
title: 'administrativeUnit: delta'
description: Получите вновь созданные, обновленные или удаленные административные единицы без выполнения полного чтения всей коллекции ресурсов.
ms.localizationpriority: medium
author: DougKirschner
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: ac39c1db1a6bcf2a433671526ef546f19599e6b7
ms.sourcegitcommit: 0e7927f34b7e55d323acbf281e11560cb40a89ed
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2022
ms.locfileid: "63669482"
---
# <a name="administrativeunit-delta"></a>administrativeUnit: delta

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создайте заново созданные, обновленные или удаленные **административные** подразделения, не выполняя полное чтение всей коллекции ресурсов. Подробные сведения см. в [материале Использование delta-запроса](/graph/delta-query-overview).

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).


|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|administrativeunit | AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

Чтобы начать отслеживать изменения, необходимо сделать запрос, который включает функцию дельты на **ресурсе administrativeUnit** .

<!-- { "blockType": "ignored" } -->
```http
GET /administrativeUnits/delta
```

## <a name="query-parameters"></a>Параметры запроса

Отслеживание изменений вызывает один или несколько вызовов функции **дельты** . Если вы используете параметры запроса, отличные от `$deltatoken` и `$skiptoken`, их необходимо указать в начальном запросе **delta**. Microsoft Graph автоматически кодирует указанные параметры в маркере, входящем в состав URL-адреса `nextLink` или `deltaLink`, включенного в отклик. Необходимо указать параметры запроса только один раз. В последующих запросах скопируйте и примените `nextLink` URL-адрес `deltaLink` из предыдущего ответа. Этот URL-адрес уже содержит закодированные параметры.

| Параметр запроса      | Тип   |Описание|
|:---------------|:--------|:----------|
| $deltatoken | string | Маркер [состояния,](/graph/delta-query-overview) возвращенный в `deltaLink` URL-адрес предыдущей  функции дельты, вызываем для того же собрания ресурсов, что указывает на завершение этого раунда отслеживания изменений. Сохраните URL-адрес `deltaLink` с этим токеном и примените его в первом запросе следующего цикла отслеживания изменений для этой коллекции.|
| $skiptoken | string | Маркер [состояния,](/graph/delta-query-overview) возвращенный в URL-адрес `nextLink` предыдущего  вызова функции дельты, указывает на то, что в том же собрании ресурсов необходимо отслеживать дальнейшие изменения. |

### <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод поддерживает указанные ниже параметры запросов OData для настройки отклика.

- Вы можете использовать параметр запроса `$select` так же, как в любом другом запросе GET, чтобы задать только те свойства, которые необходимы для эффективной работы. Свойство **id** возвращается всегда. 

- Имеется ограниченная поддержка параметра `$filter`:
  * Единственным поддерживаемым `$filter` выражением является отслеживание изменений для определенных ресурсов по их ID:  `$filter=id+eq+{value}` или `$filter=id+eq+{value1}+or+id+eq+{value2}`. Количество url-адресов, которые можно указать, ограничено максимальной длиной URL-адреса.


## <a name="request-headers"></a>Заголовки запросов
| Имя       | Описание|
|:---------------|:----------|
| Авторизация  | Носитель &lt;токен&gt;. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы этот `200 OK` метод возвращает код ответа и объект [коллекции administrativeUnit](../resources/administrativeunit.md) в тексте ответа. Отклик также содержит URL-адрес `nextLink` или `deltaLink`. 

- Если возвращается URL-адрес `nextLink`, это означает, что во время сеанса получены не все страницы данных. Администратор **продолжает делать** запросы с помощью `nextLink` URL-адреса `deltaLink` до тех пор, пока URL-адрес не будет включен в ответ.

- Если возвращается URL-адрес `deltaLink`, это означает, что больше нет данных о текущем состоянии ресурса. Сохраните и используйте URL-адрес `deltaLink` , чтобы узнать об изменениях в ресурсе в будущем.

Дополнительные сведения и пример см. в примере [Using delta query](/graph/delta-query-overview) and [Get incremental changes for users](/graph/delta-query-users).

## <a name="example"></a>Пример
### <a name="request"></a>Запрос


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "administrativeunit_delta"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/administrativeUnits/delta
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/administrativeunit-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/administrativeunit-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/administrativeunit-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/administrativeunit-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/administrativeunit-delta-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/administrativeunit-delta-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- { 
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.administrativeUnit",
  "isCollection": true 
} --> 
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#administrativeunits",
  "@odata.nextLink":"https://graph.microsoft.com/beta/administrativeunits/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "displayName": "Management Fast Track",
      "visibility": null,
      "extension_fe2174665583431c953114ff7268b7b3_Education_ObjectType": "School",
      "extension_fe2174665583431c953114ff7268b7b3_Education_StateId": "WA",
      "extension_fe2174665583431c953114ff7268b7b3_Education_Address": "2 Microsoft Way",
      "extension_fe2174665583431c953114ff7268b7b3_Education_City": "Redmond",
      "extension_fe2174665583431c953114ff7268b7b3_Education_State": "WA",
      "extension_fe2174665583431c953114ff7268b7b3_Education_Country": "US",
      "extension_fe2174665583431c953114ff7268b7b3_Education_Zip": "98052",
      "extension_fe2174665583431c953114ff7268b7b3_Education_Phone": "555-123-4567",
      "extension_fe2174665583431c953114ff7268b7b3_Education_SyncSource": "SIS",
      "extension_fe2174665583431c953114ff7268b7b3_Education_SyncSource_SchoolId": "10002",
      "extension_fe2174665583431c953114ff7268b7b3_Education_SchoolPrincipalSyncSourceId": "14008",
      "extension_fe2174665583431c953114ff7268b7b3_Education_SchoolPrincipalName": "Amy Roebuck",
      "extension_fe2174665583431c953114ff7268b7b3_Education_SchoolPrincipalEmail": "aroebuck@principal.edu",
      "extension_fe2174665583431c953114ff7268b7b3_Education_SchoolZone": "1",
      "id": "8a07f5a8-edc9-4847-bbf2-dde106594bf4",
      "members@delta": [
        {
            "@odata.type": "#microsoft.graph.user",
            "id": "b66ecf79-a093-4d51-86e0-efcc4531f37a"
        },
        {
            "@odata.type": "#microsoft.graph.user",
            "id": "5bde3e51-d13b-4db1-9948-fe4b109d11a7"
        },
        {
            "@odata.type": "#microsoft.graph.group",
            "id": "801f2093-de7e-4883-a786-8a5f30874ff4"
        },
        {
            "@odata.type": "#microsoft.graph.group",
            "id": "7e4ec76c-8276-43ef-ba10-9aaa197cb212"
        },
        {
            "@odata.type": "#microsoft.graph.user",
            "id": "f5289423-7233-4d60-831a-fe107a8551cc"
        },
        {
            "@odata.type": "#microsoft.graph.user",
            "id": "48d31887-5fad-4d73-a9f5-3c356e68a038"
        },
        {
            "@odata.type": "#microsoft.graph.user",
            "id": "87d349ed-44d7-43e1-9a83-5f2406dee5bd"
        },
        {
            "@odata.type": "#microsoft.graph.user",
            "id": "c03e6eaa-b6ab-46d7-905b-73ec7ea1f755"
        }
      ]
  }
  ]
}
```

<!-- uuid: 69848a18-6b48-44fd-a398-4521803a0a00
2020-04-09 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "administrativeunit: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


