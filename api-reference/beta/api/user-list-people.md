---
title: Список людей
description: Получение списка объектов person, упорядоченные по их важности для пользователя, который определяет, какие связи и совместной работы шаблоны и устанавливать деловые контакты пользователя.
author: simonhult
ms.openlocfilehash: 64d24111f295fd076024a889d050c8c48c104295
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27347658"
---
# <a name="list-people"></a>Список людей

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Получение списка объектов [person](../resources/person.md) , упорядоченные по их важности для [пользователя](../resources/user.md), который определяет, какие связи и совместной работы шаблоны и устанавливать деловые контакты пользователя.

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
|$search|string|Поиск пользователей по имени или псевдониму. Поддерживается нечеткое соответствие. Параметр работает только при поиске людей соответствующий пользователь выполнил вход, не для поиска людей, предназначенных для других пользователей. Также поддерживает `topic` ключевое слово для поиска людей на основании разделы, извлеченные из сообщений электронной почты с этим контактом. В разделе *Perform Нечеткое поиска* в [получить информацию о пользователях](/graph/people-example#perform-a-fuzzy-search) сведения и примеры.|
|$select|string|Список разделенных запятыми свойств, которые необходимо включить в отклик. Для оптимизации производительности выбирайте только необходимые свойства.|
|$skip|целое|Пропуск первых n результатов; эту функцию удобно использовать при разбиении результатов на страницы. Эта возможность не поддерживается при использовании параметра *$search*.|
|$top|целое|Количество возвращаемых результатов.|

## <a name="request-headers"></a>Заголовки запроса

| Имя      |Описание|
|:----------|:----------|
| Авторизация  | Bearer {токен}. Обязательный. |
| Accept | application/json |

## <a name="request-body"></a>Текст запроса

Не указывайте тело запроса для этого метода.

## <a name="response"></a>Ответ

Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [человека](../resources/person.md) в теле ответа.

## <a name="examples"></a>Примеры

### <a name="browse"></a>Обзор

Запросы в этом разделе получить наиболее важные, чтобы пользователь выполнил вход пользователей (`/me`), в зависимости от связи, совместной работы и деловыми отношениями.

По умолчанию каждый отклик возвращает 10 записей, но его можно изменить с помощью параметра *$top* . Эти запросы требуется разрешение People.Read.

#### <a name="request"></a>Запрос

Ниже приведен пример запроса по умолчанию.
<!-- {
  "blockType": "request",
  "name": "get_person_collection_beta"
}-->

```http
GET https://graph.microsoft.com/beta/me/people
```

#### <a name="response"></a>Ответ

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

#### <a name="requesting-a-subsequent-page-of-people"></a>Разрешения на запрос следующей странице людей

Если в первом отклике содержится неполный список релевантных людей, вы можете создать второй запрос, используя параметры *$top* и *$skip*, чтобы запросить дополнительные страницы информации. Если в предыдущем запросе есть дополнительная информация, то при последующем запросе будет получена следующая страница с людьми с сервера.

```http
GET https://graph.microsoft.com/beta/me/people/?$top=10&$skip=10
```

#### <a name="sort-the-response"></a>Сортировка в отклике

По умолчанию люди в ответе сортируются по степени соответствия запросу. Этот порядок можно изменить с помощью параметра *$orderby*. Этот запрос выбирает наиболее важные для вас людей, их сортировка по их отображаемое имя и затем возвращаются первые 10 пользователей на отсортированный список.

```http
GET https://graph.microsoft.com/beta/me/people/?$orderby=DisplayName
```

#### <a name="changing-the-number-of-people-returned-and-the-fields-returned"></a>Изменение числа возвращаемых людей и поля

Вы можете изменить количество людей, возвращаемых в отклике, настроив параметр *$top*.

Следующий пример запрашивает 1 000 пользователей, наиболее подходящих для `/me`. Запрос также ограничивает объем данных, отправленных с сервера, запрашивая только отображаемое имя пользователя.

```http
GET https://graph.microsoft.com/beta/me/people/?$top=1000&$select=DisplayName
```

#### <a name="selecting-the-fields-to-return"></a>Выбор полей для возврата

Можно ограничить объем данных, возвращаемых с сервера с помощью параметра *$select* выбрать одно или несколько полей. В поле *@odata.id* всегда возвращается.

В следующем примере ограничиваются ответ на *DisplayName* и *EmailAddress* 10 наиболее подходящих людей.

```http
GET https://graph.microsoft.com/beta/me/people/?$select=DisplayName,EmailAddresses
```

#### <a name="using-a-filter-to-limit-the-response"></a>С помощью фильтра для ограничения ответа

Вы можете использовать параметр *$filter*, чтобы ограничить количество информации в отклике и возвращать только тех людей, записи которых содержат указанные критерии.

Следующий запрос ограничивает ответа для людей с источником «Каталог».

```http
GET https://graph.microsoft.com/beta/me/people/?$filter=Sources/Any (source: source/Type  eq 'Directory')
```

#### <a name="selecting-the-fields-to-return-in-a-filtered-response"></a>Выбор полей для возврата в отфильтрованные ответа

Сочетая параметры *$select* и *$filter*, вы можете создать настраиваемый список людей, релевантных для пользователя, и получать только те поля, которые необходимы вашему приложению.

В следующем примере получается *DisplayName* и *EmailAddress* людей, отображаемое имя равно указанному имени. В этом примере возвращаются только тех, отображаемое имя равно «Nestor Kellum».

```http
+GET https://graph.microsoft.com/beta/me/people/?$select=DisplayName,EmailAddresses&$filter=DisplayName eq 'Nestor Kellum'
```

### <a name="search-people"></a>Поиск людей

Запросы в этом разделе также получить людей самые точные, чтобы пользователь выполнил вход (`/me`). Запросы поиска требуется разрешение People.Read.

#### <a name="using-search-to-select-people"></a>Использование поиска для выбора людей

Используйте параметр *$search* для выбора людей, удовлетворяющих определенному набору критериев.

Следующий запрос поиска возвращает людей, относящиеся к `/me` , GivenName или фамилию начинается с буквы «j».

```http
GET https://graph.microsoft.com/beta/me/people/?$search=j
```

#### <a name="using-search-to-specify-a-relevant-topic"></a>Использование поиска для указания соответствующей темы

Следующий запрос возвращает людей, относящиеся к `/me` , имя которого содержит «ma» и пользователей, которые имеют связь с «планирование компонентов».

```http
GET https://graph.microsoft.com/beta/me/people/?$search="ma topic: feature planning"
```

#### <a name="performing-a-fuzzy-search"></a>Для выполнения Нечеткое поиска

Следующий запрос поиска для пользователя с именем «Зал Hermaini». Так как пользователь с именем «Herminia оболочка» относится к пользователь выполнил вход, возвращается информация для «Herminia оболочка».

```http
GET https://graph.microsoft.com/beta/me/people/?$search="hermaini hall"
```

### <a name="related-people"></a>Связанные людей

Следующий запрос получает наиболее подходящих другому пользователю людей в организации пользователя. Этот запрос требует User.ReadBasic.All People.Read.All разрешения. В этом примере отображаются Nestor Kellum соответствующих пользователей.

```http
GET https://graph.microsoft.com/beta/users('nestork@contoso.com')/people/
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List people",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
