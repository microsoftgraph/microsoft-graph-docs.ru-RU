---
title: Список людей
description: Получение списка объектов person, упорядоченных по их релевантности для пользователя, которая определяется его моделями общения и совместной работы, а также бизнес-отношениями.
author: dkershaw10
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: 6212446f136d87b9331793c9846be8f2edd8a499
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48968869"
---
# <a name="list-people"></a>Список людей

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение списка объектов [Person](../resources/person.md) , упорядоченных по релевантности для [пользователя](../resources/user.md), которые определяются шаблонами общения и совместной работы пользователя, а также бизнес-отношениями.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | People.Read    |
|Делегированные (личная учетная запись Майкрософт) | People.Read    |
|Для приложений | Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
GET /me/people
GET /users/{id | userPrincipalName}/people
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод поддерживает следующие параметры запроса OData для настройки ответа.

|Имя|Значение|Описание|
|:---------------|:--------|:-------|
|$filter|string|Позволяет возвращать в отклике только тех людей, чьи записи содержат указанные критерии.|
|$orderby|строка|По умолчанию люди в ответе сортируются по степени соответствия запросу. Этот порядок можно изменить с помощью параметра *$orderby*.|
|$search|string|Поиск пользователей по имени или псевдониму. Поддерживается нечеткое соответствие. Параметр применяется только для поиска людей, относящихся к вошедшему пользователю, а не для поиска людей, относящихся к другим пользователям. Также поддерживает ключевое слово `topic` для поиска людей с учетом тем, извлеченных из бесед электронной почты с определенным человеком. Сведения и примеры см. в разделе *Нечеткий поиск* статьи [Получение релевантных сведений о людях](/graph/people-example#perform-a-fuzzy-search).|
|$select|string|Список разделенных запятыми свойств, которые необходимо включить в отклик. Для оптимизации производительности выбирайте только необходимые свойства.|
|$skip|int|Пропуск первых n результатов; эту функцию удобно использовать при разбиении результатов на страницы. Эта возможность не поддерживается при использовании параметра *$search*.|
|$top|int|Количество возвращаемых результатов.|

## <a name="request-headers"></a>Заголовки запроса

| Имя      |Описание|
|:----------|:----------|
| Авторизация  | Bearer {токен}. Обязательный. |
| Accept | application/json |

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [Person](../resources/person.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="browse"></a>Обратитесь

Запросы в этом разделе позволяют получить людей, наиболее релевантных для вошедшего пользователя ( `/me` ), на основе взаимодействия, совместной работы и бизнес-связей.

По умолчанию каждый ответ возвращает 10 записей, но вы можете изменить его с помощью параметра *$Top* . Для этих запросов требуется разрешение "люди. чтение".

#### <a name="request"></a>Запрос

Ниже приведен пример запроса по умолчанию.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_person_collection_beta"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/people
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-person-collection-beta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-person-collection-beta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-person-collection-beta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-person-collection-beta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик

Ниже приведен пример отклика.
>**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.

<!-- {
  "blockType": "response",
  "name": "get_person_collection_beta",
  "truncated": true,
  "@odata.type": "microsoft.graph.person",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1326

{
    "value": [
        {
            "id": "33b43a5b-87d6-41ec-91f8-a2610048105f",
            "displayName": "Marketing",
            "givenName": null,
            "surname": null,
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "title": null,
            "companyName": null,
            "yomiCompany": "",
            "department": null,
            "officeLocation": null,
            "profession": "",
            "mailboxType": "GroupMailbox",
            "personType": "ModernGroup",
            "userPrincipalName": "",
            "emailAddresses": [
                {
                    "address": "Marketing@contoso.com",
                    "rank": 30
                }
            ],
            "phones": [],
            "postalAddresses": [],
            "websites": [],
            "sources": [
                {
                    "type": "Directory"
                }
            ]
        },
        {
            "id": "e3d0513b-449e-4198-ba6f-bd97ae7cae85",
            "displayName": "Isaiah Langer",
            "givenName": "Isaiah",
            "surname": "Langer",
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "title": "Web Marketing Manager",
            "companyName": null,
            "yomiCompany": "",
            "department": "Sales & Marketing",
            "officeLocation": "20/1101",
            "profession": "",
            "mailboxType": "Mailbox",
            "personType": "Person",
            "userPrincipalName": "IsaiahL@contoso.com",
            "emailAddresses": [
                {
                    "address": "IsaiahL@contoso.com",
                    "rank": 20
                }
            ],
            "phones": [
                {
                    "type": "business",
                    "number": "+1 918 555 0101"
                }
            ],
            "postalAddresses": [],
            "websites": [],
            "sources": [
                {
                    "type": "Directory"
                }
            ]
        }
    ]
}
```

#### <a name="requesting-a-subsequent-page-of-people"></a>Запрос последующей страницы людей

Если в первом отклике содержится неполный список релевантных людей, вы можете создать второй запрос, используя параметры *$top* и *$skip* , чтобы запросить дополнительные страницы информации. Если в предыдущем запросе есть дополнительная информация, то при последующем запросе будет получена следующая страница с людьми с сервера.

```http
GET https://graph.microsoft.com/beta/me/people/?$top=10&$skip=10
```

#### <a name="sort-the-response"></a>Сортировка в отклике

По умолчанию люди в ответе сортируются по степени соответствия запросу. Этот порядок можно изменить с помощью параметра *$orderby*. Этот запрос выбирает наиболее релевантных для вас сотрудников, сортирует их по отображаемому имени, а затем возвращает первые 10 пользователей из отсортированного списка.

```http
GET https://graph.microsoft.com/beta/me/people/?$orderby=DisplayName
```

#### <a name="changing-the-number-of-people-returned-and-the-fields-returned"></a>Изменение количества возвращаемых людей и возвращаемых полей

Вы можете изменить количество людей, возвращаемых в отклике, настроив параметр *$top*.

В следующем примере запрашивается 1 000 пользователей, наиболее релевантных для `/me` . Запрос также ограничит количество данных, отправляемых с сервера, запросив только отображаемое имя пользователя.

```http
GET https://graph.microsoft.com/beta/me/people/?$top=1000&$select=DisplayName
```

#### <a name="selecting-the-fields-to-return"></a>Выбор полей для возврата

Можно ограничить объем данных, возвращаемых с сервера, с помощью параметра *$SELECT* , чтобы выбрать одно или несколько полей. Поле *@odata. ID* всегда возвращается.

В следующем примере показано, как ограничить выданный ответ на *DisplayName* и *EmailAddress* 10 самых релевантных людей.

```http
GET https://graph.microsoft.com/beta/me/people/?$select=DisplayName,EmailAddresses
```

#### <a name="using-a-filter-to-limit-the-response"></a>Использование фильтра для ограничения ответа

Вы можете использовать параметр *$filter* , чтобы ограничить количество информации в отклике и возвращать только тех людей, записи которых содержат указанные критерии.

Следующий запрос ограничит отклик для людей с исходным каталогом.

```http
GET https://graph.microsoft.com/beta/me/people/?$filter=Sources/Any (source: source/Type  eq 'Directory')
```

#### <a name="selecting-the-fields-to-return-in-a-filtered-response"></a>Выбор полей, возвращаемых в отфильтрованном ответе

Сочетая параметры *$select* и *$filter* , вы можете создать настраиваемый список людей, релевантных для пользователя, и получать только те поля, которые необходимы вашему приложению.

В следующем примере показано, как получить *DisplayName* и *EmailAddress* людей, отображаемое имя которых соответствует заданному имени. В этом примере возвращаются только те пользователи, отображаемое имя которых равно "пользователя Nestor Келлум".

```http
+GET https://graph.microsoft.com/beta/me/people/?$select=DisplayName,EmailAddresses&$filter=DisplayName eq 'Nestor Kellum'
```

### <a name="search-people"></a>Поиск людей

Запросы в этом разделе также получают людей, наиболее релевантных для вошедшего пользователя ( `/me` ). Для запросов поиска требуются разрешения "люди. чтение".

#### <a name="using-search-to-select-people"></a>Использование поиска для выбора людей

Используйте параметр *$search* для выбора людей, удовлетворяющих определенному набору критериев.

Следующий поисковый запрос возвращает пользователей, имеющих отношение к `/me` givenName или фамилии, начинающиеся с буквы j.

```http
GET https://graph.microsoft.com/beta/me/people/?$search=j
```

#### <a name="using-search-to-specify-a-relevant-topic"></a>Использование поиска для указания соответствующего раздела

Следующий запрос возвращает пользователей, имеющих отношение к имени, которое `/me` содержит "MA" и у которого есть связь с "планированием компонентов".

```http
GET https://graph.microsoft.com/beta/me/people/?$search="ma topic: feature planning"
```

#### <a name="performing-a-fuzzy-search"></a>Выполнение нечеткого поиска

Следующий запрос выполняет поиск пользователя с именем "Хермаини зал". Так как существует пользователь "Херминиа Хулл", относящийся к пользователю, вошедшего в систему, возвращаются сведения о "Херминиа Хулл".

```http
GET https://graph.microsoft.com/beta/me/people/?$search="hermaini hall"
```

### <a name="related-people"></a>Связанные люди

Следующий запрос получает людей, наиболее релевантных для другого пользователя в Организации. Для этого запроса требуется разрешение User. ReadBasic. ALL для People. Read. ALL. В этом примере отображаются важные люди пользователя Nestor Келлум.

```http
GET https://graph.microsoft.com/beta/users('nestork@contoso.com')/people/
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List people",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


