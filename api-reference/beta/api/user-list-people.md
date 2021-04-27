---
title: Список людей
description: Получение списка объектов person, упорядоченных по их релевантности для пользователя, которая определяется его моделями общения и совместной работы, а также бизнес-отношениями.
author: dkershaw10
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: 8df99c32c43e947863c4a7713c984b99fbd4bb73
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053358"
---
# <a name="list-people"></a>Список людей

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Извлечение списка объектов [пользователя,](../resources/person.md) заказать по их релевантности для [пользователя,](../resources/user.md)который определяется шаблонами общения и совместной работы пользователя, а также деловыми отношениями.

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

Этот метод поддерживает следующие параметры запроса OData, чтобы помочь настроить ответ.

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

В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [лиц](../resources/person.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="browse"></a>Просмотр

Запросы в этом разделе получают людей, наиболее релевантных для пользователя, подписанного (), на основе связи, совместной работы `/me` и деловых отношений.

По умолчанию каждый ответ возвращает 10 записей, но изменить его можно с *помощью $top* параметра. Эти запросы требуют разрешения People.Read.

#### <a name="request"></a>Запрос

Ниже приводится пример запроса по умолчанию.

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

Ниже приведен пример ответа.
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

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

Если в первом отклике содержится неполный список релевантных людей, вы можете создать второй запрос, используя параметры *$top* и *$skip*, чтобы запросить дополнительные страницы информации. Если в предыдущем запросе есть дополнительная информация, то при последующем запросе будет получена следующая страница с людьми с сервера.

```http
GET https://graph.microsoft.com/beta/me/people/?$top=10&$skip=10
```

#### <a name="sort-the-response"></a>Сортировка в отклике

По умолчанию люди в ответе сортируются по степени соответствия запросу. Этот порядок можно изменить с помощью параметра *$orderby*. Этот запрос выбирает наиболее подходящих для вас людей, сортировать их по их имени отображения, а затем возвращает первых 10 человек в отсортировали список.

```http
GET https://graph.microsoft.com/beta/me/people/?$orderby=DisplayName
```

#### <a name="changing-the-number-of-people-returned-and-the-fields-returned"></a>Изменение количества возвращаемого и возвращаемого поля

Вы можете изменить количество людей, возвращаемых в отклике, настроив параметр *$top*.

В следующем примере запрашивается 1000 человек, наиболее подходящих для `/me` . Запрос также ограничивает объем данных, отосланных с сервера, запрашивая только отображаемую фамилию человека.

```http
GET https://graph.microsoft.com/beta/me/people/?$top=1000&$select=DisplayName
```

#### <a name="selecting-the-fields-to-return"></a>Выбор полей для возврата

Можно ограничить количество данных, возвращаемого с сервера, с помощью *параметра $select* для выбора одного или более полей. Поле *@odata.id* всегда возвращается.

В следующем примере ограничивается ответ *на displayName* и *EmailAddress* 10 наиболее релевантного пользователя.

```http
GET https://graph.microsoft.com/beta/me/people/?$select=DisplayName,EmailAddresses
```

#### <a name="using-a-filter-to-limit-the-response"></a>Использование фильтра для ограничения отклика

Вы можете использовать параметр *$filter*, чтобы ограничить количество информации в отклике и возвращать только тех людей, записи которых содержат указанные критерии.

Следующий запрос ограничивает ответ для людей с исходным кодом "Directory".

```http
GET https://graph.microsoft.com/beta/me/people/?$filter=Sources/Any (source: source/Type  eq 'Directory')
```

#### <a name="selecting-the-fields-to-return-in-a-filtered-response"></a>Выбор полей для возврата в отфильтрованный ответ

Сочетая параметры *$select* и *$filter*, вы можете создать настраиваемый список людей, релевантных для пользователя, и получать только те поля, которые необходимы вашему приложению.

В следующем примере *получается DisplayName* и *EmailAddress* людей, имя отображения которых равно указанному имени. В этом примере возвращаются только те, чье имя отображения равно "Nestor Kellum".

```http
+GET https://graph.microsoft.com/beta/me/people/?$select=DisplayName,EmailAddresses&$filter=DisplayName eq 'Nestor Kellum'
```

### <a name="search-people"></a>Поиск людей

Запросы в этом разделе также получают людей, наиболее релевантные для пользователя, заявив о подписании `/me` ( ). Запросы на поиск требуют разрешения People.Read.

#### <a name="using-search-to-select-people"></a>Использование поиска для выбора людей

Используйте параметр *$search* для выбора людей, удовлетворяющих определенному набору критериев.

В следующем поисковом запросе возвращаются люди, для которых GivenName или Surname начинается с `/me` буквы "j".

```http
GET https://graph.microsoft.com/beta/me/people/?$search=j
```

#### <a name="using-search-to-specify-a-relevant-topic"></a>Использование поиска для указания соответствующей темы

Следующий запрос возвращает людей, имя которых содержит "ma" и которые имеют связь с `/me` "планированием функций".

```http
GET https://graph.microsoft.com/beta/me/people/?$search="ma topic: feature planning"
```

#### <a name="performing-a-fuzzy-search"></a>Выполнение нечеткого поиска

Следующий запрос — поиск человека с именем "Hermaini Hall". Поскольку существует лицо с именем "Herminia Hull", соответствующее подписанной пользователю, возвращается информация для "Herminia Hull".

```http
GET https://graph.microsoft.com/beta/me/people/?$search="hermaini hall"
```

### <a name="related-people"></a>Связанные люди

Следующий запрос получает людей, наиболее релевантные другому лицу в организации пользователя. Для этого запроса требуется разрешение User.ReadBasic.All для людей.Read.All. В этом примере отображаются соответствующие люди Nestor Kellum.

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


