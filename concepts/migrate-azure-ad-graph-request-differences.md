---
title: Запрос различий между Azure AD Graph и Microsoft Graph
description: Сведения о том, как запросы Microsoft Graph отличаются от запросов Azure AD, которые помогают перенести приложения в более новую службу..
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8130daf4037e6ef1a433ca537a8fecec996a34ce
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/23/2020
ms.locfileid: "44845920"
---
# <a name="request-differences-between-azure-ad-graph-and-microsoft-graph"></a>Запрос различий между Azure AD Graph и Microsoft Graph

Эта статья входит в *Шаг 1: Ознакомьтесь с различиями* в API [процесса переноса приложений](migrate-azure-ad-graph-planning-checklist.md).

Microsoft Graph и API Graph для Azure AD — это интерфейсы API REST и каждая из них поддерживает соглашения ODATA для параметров запроса. Тем не менее синтаксис различается для этих двух интерфейсов API.

Используйте [проводник Graph](https://aka.ms/ge) , чтобы использовать эти шаблоны запросов для собственных данных, так как это отличный способ узнать о различиях в запросах и ответах.

## <a name="basic-requests"></a>Основные запросы

В следующей таблице показаны основные различия между двумя API-интерфейсами:

|Сведения о запросе| Azure AD Graph | Microsoft Graph |
|---|---|---|
|Синтаксис запроса| `https://graph.windows.net/{tenant_id}/` <br> `{resource}?{version}&query-parameters` | `https://graph.microsoft.com/`<br>`{version}/{resource}?query-parameters`|
|&nbsp;Конечные точки служб:||
|-&nbsp;Глобального|`https://graph.windows.net`|`https://graph.microsoft.com`|
|-&nbsp;&nbsp;Gov &nbsp; 4 для США|`https://graph.microsoftazure.us`|`https://graph.microsoft.us`|
|-&nbsp;Американский &nbsp; gov на &nbsp; уровне 5 &nbsp; (DoD)|`https://graph.microsoftazure.us`|`https://dod-graph.microsoft.us`|
|-&nbsp;Германия|`https://graph.cloudapi.de`|`https://graph.microsoft.de`|
|-&nbsp;Китай &nbsp; (21vianet)| `https://graph.chinacloudapi.cn`|`https://microsoftgraph.chinacloudapi.cn`|
|{tenant_id}|Укажите идентификатор клиента в запросе.|Необязательно указывать идентификатор клиента в запросе, так как он выводится из маркера доступа.<br><br>Если указать идентификатор клиента, он поместится между параметром `{version}` и `{resource}` в URL-адресе запроса.|
|Отслеживание|Укажите в запросе окончательную версию Azure AD Graph, используя обязательный параметр запроса.|Укажите версию Microsoft Graph в запросе в качестве части URL-пути сразу после конечной точки службы.|

Вы можете продолжать использовать одни и те же параметры запроса в Microsoft Graph как Azure AD Graph.

### <a name="example-request-comparison"></a>Пример сравнения запросов

Предположим, что вам нужен список всех пользователей с именами, начинающимися с "" "").

В Azure AD Graph можно использовать следующий запрос:

`https://graph.windows.net/contoso.com/users?$filter=startswith(givenName,'Dan')&api-version=1.6`

Этот запрос:

- Targets версии 1,6 для Azure AD Graph.
- Задает `contoso.com` идентификатор клиента.
- Вызывает ресурс Users.
- Использует `$filter` параметр запроса, чтобы ограничить ответ на заданные имена, начинающиеся с `Dan` .

Результаты включают пользователей с именами, такими как Дэниэл, Данфорс, Даниелле, Данерис и т. д.

Аналогичный запрос для Microsoft Graph выглядит следующим образом:

`https://graph.microsoft.com/v1.0/users?$filter=startswith(givenName,'Dan')`

Существует

- Версия `v1.0` .
- Идентификатор клиента извлекается из маркера доступа (не показан).
- Параметр resource и `$filter` Query совпадает с запросом Azure AD.

> **Примечание**. Если вы используете клиентскую библиотеку .NET для Azure AD Graph, ознакомьтесь с разработкой клиентских [библиотек .NET](migrate-azure-ad-graph-client-libraries.md) для получения более подробных стратегий и помощи в переходе на клиентскую библиотеку Microsoft Graph .NET.

### <a name="key-identifiers-objectid-vs-id"></a>Идентификаторы ключа: objectId VS ID

В Azure AD Graph все типы ресурсов сущностей имеют уникальный идентификатор (или ключ) с именем **ObjectID**.  Для большинства частей (если не указано иное) такой же идентификатор называется **идентификатором** в Microsoft Graph.

## <a name="default-properties-and-select"></a>Свойства по умолчанию и $select

Используйте `$select` параметр запроса в запросах GET, чтобы настроить ответ на включение всех свойств, необходимых вашему приложению.

Операции **получения** или получения **списка** Microsoft Graph для ресурсов пользователей или групп возвращают только подмножество свойств, известных как _свойства по умолчанию_. Свойства по умолчанию представляют наиболее часто используемые свойства ресурса. С другой стороны, Azure AD Graph возвращает полный набор всех свойств для соответствующего ресурса.

Чтобы получить другие свойства в версии 1.0, ваше приложение должно явно запрашивать их, используя `$select` параметр запроса. Сюда входят все расширения схемы каталогов, которые может использовать ваше приложение. Рекомендуется запрашивать только те свойства, которые действительно необходимы вашему приложению.

Чтобы продемонстрировать разницу, используйте проводник Graph для выполнения следующих запросов и сравнения различных ответов.

```http
GET https://graph.microsoft.com/v1.0/me/
GET https://graph.microsoft.com/beta/me/
```

Просмотрите ответы от каждого запроса. Вы заметите, что сведения об адресе возвращаются версией/Beta, но не версией/v1.0.  Это вызвано тем, что свойства адреса не входят в набор свойств по умолчанию.

Если ваше приложение использует свойства адреса, необходимо обновить запросы версии 1.0, чтобы включить `$select` параметр запроса:

```http
https://graph.microsoft.com/v1.0/me/?$select=displayName,streetAddress,city,state,postalCode
```

Ответ на этот запрос будет включать в себя свойства Address.  Он также включает свойство **DisplayName** , но только потому, что оно было задано с помощью параметра запроса.

Дополнительные сведения:

- Свойства по умолчанию для пользователя, обратитесь к разделу [Пользователи](/graph/api/resources/users?view=graph-rest-1.0)
- `$select`Параметр и другие поддерживаемые параметры запроса ODATA в разделе [Использование параметров запроса для настройки ответов](/graph/query-parameters).
- Эта и другие Рекомендуемые [оптимизации приведены в разделе рекомендации.](/graph/best-practices-concept)

## <a name="relationships-and-navigation-properties"></a>Отношения и свойства навигации

Отношения (или свойства навигации) являются ключевыми понятиями в Azure AD Graph и Microsoft Graph, создавая сеть связанных ресурсов. Например, свойства **Manager** и **directReports** расширяют пользовательский ресурс для предоставления организационной иерархии.

Отношения также определяют членство, например группы, к которым принадлежит пользователь, членов, принадлежащих группе или роли каталога, и т. д.

Запросы Azure AD Graph используются `$link` для обозначения отношений между ресурсами.  В Microsoft Graph `$ref` вместо этого используется нотация ODATA 4,01.

В следующей таблице приведено несколько примеров.

| Task | Azure AD Graph | Microsoft Graph |
|------|----------------|-----------------|
| Добавление участника        | ```POST /groups/{id}/$link/members```        | ```POST /groups/{id}/members/$ref```        |
| Ссылки на элементы списка | ```GET /groups/{id}/$link/members```         | ```GET /groups/{id}/members/$ref```         |
| Список участников      | ```GET /groups/{id}/members```                | ```GET /groups/{id}/members```               |
| Удаление участника     | ```DELETE /groups/{id}/$link/members/{id}``` | ```DELETE /groups/{id}/members/{id}/$ref``` |

При переносе приложений в Microsoft Graph ищите запросы, которые используют `$link` для связи ресурсов, а вместо этого измените их для использования `$ref` .

## <a name="next-steps"></a>Дальнейшие действия

- Сведения о [различиях функций служб](migrate-azure-ad-graph-feature-differences.md) в Azure AD Graph и Microsoft Graph.
- Ознакомьтесь с основными понятиями и рекомендациями [Microsoft Graph](/graph/overview) .
- Поэкспериментируйте с Microsoft Graph с помощью [проводника диаграмм](https://aka.ms/ge) .
