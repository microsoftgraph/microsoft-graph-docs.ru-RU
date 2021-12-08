---
title: Запросить различия между Azure AD Graph Microsoft Graph
description: Описывает, как Graph Microsoft отличаются от Azure Active Directory (Azure AD) Graph, что помогает перенести приложения в более новую службу..
author: dkershaw10
ms.localizationpriority: medium
ms.prod: applications
ms.openlocfilehash: dc11e79faf3d2e1e0cc614fe9044eea7e41bb9a5
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2021
ms.locfileid: "61344451"
---
# <a name="request-differences-between-azure-ad-graph-and-microsoft-graph"></a>Запросить различия между Azure AD Graph Microsoft Graph

Эта статья является *частью шага 1: просмотрите различия API* процесса переноса [приложений.](migrate-azure-ad-graph-planning-checklist.md)

Microsoft Graph и Azure Active Directory (Azure AD) Graph API являются API REST, и каждый из них поддерживает соглашения OData для параметров запросов. Однако синтаксис различается между этими двумя API.

Используйте [Graph Explorer,](https://aka.ms/ge) чтобы попробовать эти шаблоны запросов в отношении собственных данных, так как это отличный способ узнать о различиях запросов и ответов.

## <a name="basic-requests"></a>Основные запросы

В следующей таблице выделяются основные различия запросов между двумя API:

|Сведения о запросе| Azure AD Graph | Microsoft Graph |
|---|---|---|
|Запрос синтаксиса| `https://graph.windows.net/{tenant_id}/` <br> `{resource}?{version}&query-parameters` | `https://graph.microsoft.com/`<br>`{version}/{resource}?query-parameters`|
|Конечные &nbsp; точки службы:||
|-&nbsp;Глобальный|`https://graph.windows.net`|`https://graph.microsoft.com`|
|-&nbsp;США &nbsp; Gov &nbsp; L4|`https://graph.microsoftazure.us`|`https://graph.microsoft.us`|
|-&nbsp;США &nbsp; Gov &nbsp; L5 &nbsp; (DOD)|`https://graph.microsoftazure.us`|`https://dod-graph.microsoft.us`|
|-&nbsp;Германия|`https://graph.cloudapi.de`|`https://graph.microsoft.de`|
|-&nbsp;Китай &nbsp; (21Vianet)| `https://graph.chinacloudapi.cn`|`https://microsoftgraph.chinacloudapi.cn`|
|{tenant_id}|Укажите в запросе ID клиента.|Необязательно указывать в запросе ИД клиента, так как он высвечен из маркера доступа.<br><br>Если указать ID клиента, он переходит между URL-адресом запроса `{version}` `{resource}` и url-адресом запроса.|
|{version}|Укажите версию выпуска Azure AD Graph запросе с помощью требуемого параметра запроса.|Укажите версию выпуска Microsoft Graph в запросе как часть пути URL-адреса сразу после конечной точки службы.|

Вы можете продолжать использовать те же параметры запроса в Microsoft Graph, что и Azure AD Graph.

### <a name="example-request-comparison"></a>Сравнение примера запроса

Предположим, вам нужен список всех пользователей с именами, начиная с "Dan".

В Azure AD Graph этот запрос можно использовать:

`GET https://graph.windows.net/contoso.com/users?$filter=startswith(givenName,'Dan')&api-version=1.6` или

`GET https://graph.windows.net/myOrganization/users?$filter=startswith(givenName,'Dan')&api-version=1.6`


Этот запрос:

- Целевые показатели версии 1.6 Azure AD Graph.
- Указывает `contoso.com` в качестве ID клиента. Альтернатива показывает использование псевдонима на основе ID клиента в `myOrganization` маркере доступа.
- Вызывает ресурс пользователей.
- Параметр `$filter` запроса используется для ограничения ответа на заданные имена, которые начинаются `Dan` с .

К результатам относятся пользователи с именами Daniel, Danforth, Danielle, Danerys и так далее.

Аналогичный запрос для microsoft Graph будет:

`GET https://graph.microsoft.com/v1.0/users?$filter=startswith(givenName,'Dan')`

Здесь:

- Версия `v1.0` .
- ID клиента высвечен из маркера доступа (не показан).
- Параметр ресурса `$filter` и запроса такой же, как и запрос Azure AD.

> **ПРИМЕЧАНИЕ.** Если вы используете клиентскую библиотеку Azure AD Graph .NET, см. в этой заметке.NET client [libraries](migrate-azure-ad-graph-client-libraries.md) for more specific strategies and assistance to move to the Microsoft Graph .NET client library.

### <a name="key-identifiers-objectid-vs-id"></a>Ключевые идентификаторы: objectId vs id

В Azure AD Graph все типы ресурсов сущности имеют уникальный идентификатор (или ключ) под названием **objectId.**  По большей части (если иное не указано) этот идентификатор называется **id** в Microsoft Graph.

## <a name="default-properties-and-select"></a>Свойства и $select

Используйте параметр `$select` запроса в запросах GET, чтобы настроить ответ, чтобы включить все необходимые свойства приложения.

Microsoft Graph для  получения  или списка операций для пользователей или групповых ресурсов возвращает только подмножество всех свойств, известных как свойства по _умолчанию._ Свойства по умолчанию представляют наиболее часто используемые свойства для ресурса. С другой стороны, Azure AD Graph возвращает полный набор всех свойств для соответствующего ресурса.

Чтобы получить другие свойства в v1.0, приложение должно явно запрашивать их с помощью `$select` параметра запроса. Это включает в себя все расширения схемы каталогов, которые может использовать ваше приложение. Лучше всего запрашивать только свойства, которые действительно нужны вашему приложению.

Чтобы проиллюстрировать разницу, Graph Explorer для запуска следующих запросов и сравнения различных ответов.

```http
GET https://graph.microsoft.com/v1.0/me/
GET https://graph.microsoft.com/beta/me/
```

Просмотрите ответы по каждому запросу. Вы заметите, что сведения о адресе возвращаются бета-версией, но не версией /v1.0.  Это потому, что свойства адресов не в наборе свойств по умолчанию.

Если приложение полагается на свойства адресов, необходимо обновить запросы на v1.0, чтобы включить параметр `$select` запроса:

```http
https://graph.microsoft.com/v1.0/me/?$select=displayName,streetAddress,city,state,postalCode
```

Ответ на этот запрос будет включать свойства адресов.  Оно также включает **свойство displayName,** но только потому, что оно было задано параметром запроса.

Чтобы узнать больше о:

- Свойства по умолчанию для пользователя см. в [записи пользователей](/graph/api/resources/users)
- Параметр `$select` и другие поддерживаемые параметры запроса ODATA см. в руб. Параметры использования запросов [для настройки ответов.](./query-parameters.md)
- Эти и другие рекомендуемые оптимизации см. в [рекомендациях.](./best-practices-concept.md)

## <a name="relationships-and-navigation-properties"></a>Свойства отношений и навигации

Отношения (или свойства навигации) являются ключевой концепцией в Azure AD Graph и Microsoft Graph, создавая сеть связанных ресурсов. Например, свойства **manager** и **directReports** расширяют пользовательский ресурс, чтобы обеспечить организационную иерархию.

Отношения также определяют членство, например группы, к которой принадлежит пользователь, члены, принадлежащие к группе или роли каталога, и так далее.

Azure AD Graph для `$links` указать отношения между ресурсами.  В microsoft Graph вместо этого используется нотация OData v4.01. `$ref`

В следующей таблице показано несколько примеров:

| Задача | Azure AD Graph | Microsoft Graph |
|------|----------------|-----------------|
| Добавление участника        | `POST /groups/{id}/$links/members`        | `POST /groups/{id}/members/$ref`        |
| Ссылки участников списка | `GET /groups/{id}/$links/members`         | `GET /groups/{id}/members/$ref`         |
| Список участников      | `GET /groups/{id}/members`                | `GET /groups/{id}/members`               |
| Удаление участника     | `DELETE /groups/{id}/$links/members/{id}` | `DELETE /groups/{id}/members/{id}/$ref` |

При переносе приложений в Microsoft Graph искать запросы, которые используются для связывания ресурсов; измените `$links` их, чтобы использовать `$ref` вместо них.

## <a name="next-steps"></a>Дальнейшие действия

- Узнайте о [различиях функций](migrate-azure-ad-graph-feature-differences.md) службы между Azure AD Graph Microsoft Graph.
- Снова [просмотрите контрольный](migrate-azure-ad-graph-planning-checklist.md) список.
