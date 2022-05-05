---
title: Создание, обновление и удаление элементов, добавленных приложением в связь Microsoft Graph
description: Узнайте, как использовать Microsoft Graph для управления элементами, добавленными приложением в службу "Поиск (Майкрософт)".
ms.localizationpriority: high
author: mecampos
doc_type: conceptualPageType
ms.prod: search
ms.openlocfilehash: 5ef77fd98e055d9b60b76f4aa3728f20f6cbff7e
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65211034"
---
<!---<author of this doc: rsamai>--->

# <a name="create-update-and-delete-items-added-by-your-application-via-microsoft-graph-connectors"></a>Создание, обновление и удаление элементов, добавленных приложением с помощью соединителей Microsoft Graph

Соединители Microsoft Graph — это интуитивно понятный способ добавления внешних данных в Microsoft Graph. Элементы, добавленные приложением в службу "Поиск (Майкрософт)", представлены ресурсом [externalItem](/graph/api/resources/externalconnectors-externalitem?view=graph-rest-1.0&preserve-view=true) в Microsoft Graph.

После [создания соединения](/graph/api/externalconnectors-external-post-connections?view=graph-rest-1.0&preserve-view=true&tabs=http) вы можете добавить содержимое. Каждый элемент из источника данных должен быть представлен в виде externalItem в Microsoft Graph с уникальным идентификатором элемента. Этот идентификатор используется для создания, обновления или удаления элемента в Microsoft Graph. Вы можете использовать первичный ключ из источника данных в качестве ИД элемента или получить его из одного или нескольких полей. 

## <a name="key-components"></a>Ключевые компоненты

externalItem содержит три основных компонента: список управления доступом, свойства и содержимое.

### <a name="access-control-list"></a>Список управления доступом

Список управления доступом (ACL) используется для указания того, предоставляется ли определенным ролям доступ для просмотра элементов в интерфейсах Майкрософт. ACL — это массив записей управления доступом, каждая из которых представляет пользователя или группу Azure Active Directory (Azure AD). Существует третий тип записей управления доступом: `Everyone`, представляющий всех пользователей в клиенте.

![Пример списка управления доступом.](./images/connectors-images/connecting-external-content-manage-items-acl.png)

*Пример списка управления доступом.*

Значение **accessType** `deny` имеет приоритет над `grant`. Например, хотя в представленном ранее элементе доступ предоставлен с помощью параметра `Everyone`, а конкретному пользователю доступ запрещен, действующим разрешением для этого пользователя будет вариант `deny`.

Если ваш источник данных не содержит групп Azure AD (например, группы в вашей службе поддержки), применяемых для настройки разрешений для элемента, вы можете создать внешние группы в Microsoft Graph, используя API синхронизации группы для репликации разрешений `allow` или `deny`. Избегайте расширения участия ваших внешних групп непосредственно в списках управления доступом отдельных элементов, так как каждое участие группы может привести к многочисленным обновлениям элементов.

Внешние группы могут состоять из других внешних групп, пользователе и групп Azure AD. Если у вас есть пользователи, не являющиеся пользователями Azure AD, вы должны преобразовать их в пользователей Azure AD в своем списке управления доступом.

### <a name="properties"></a>Свойства

С помощью компонента свойств можно добавлять метаданные элементов, которые удобно применять в интерфейсах Microsoft Graph. Вы должны [зарегистрировать схему](connecting-external-content-manage-schema.md) для связи перед добавлением в нее элементов и преобразованием **типов данных** в [поддерживаемые типы данных](/graph/api/resources/externalconnectors-property?view=graph-rest-1.0&preserve-view=true).

![Пример компонента свойства.](./images/connectors-images/connecting-external-content-manage-items-1.png)

*Пример компонента свойства.*

### <a name="content"></a>Содержимое

Компонент содержимого используется для массового добавления элементов, которые должны быть полнотекстовым индексом. Примеры включают описание запроса, проанализированный текст из файла или вики-страницы.

Содержимое — одно из ключевых полей, влияющих на [релевантность](connecting-external-content-manage-schema.md#relevance) в интерфейсах Майкрософт. Поддерживаются типы контента: `text` и `html`. Если источник данных содержит контент других типов, например двоичные файлы, видео или изображения, вы можете преобразовать их в текстовую форму перед добавлением в Microsoft Graph. Например, для извлечения из изображений пригодного для поиска текста можно использовать распознавание текста.

![Пример компонента содержимого.](./images/connectors-images/connecting-external-content-manage-items-2.png)

*Пример компонента содержимого.*

Содержимое нельзя непосредственно добавить в шаблон результатов поиска, но вы можете использовать созданный фрагмент результатов, являющийся динамически создаваемым предварительным просмотром соответствующих разделов в содержимом.

![Снимок экрана с шаблоном результатов поиска.](./images/connectors-images/connecting-external-content-manage-items-3.svg)

*Шаблон результатов поиска.*

При изменении содержимого в источнике данных вы должны синхронизировать его с элементами связи. Вы можете обновить весь элемент или обновить один или несколько его компонентов. После добавления содержимого в Microsoft Graph вы можете искать его с помощью интерфейса Поиска (Майкрософт), настроив [вертикали поиска](/en-us/microsoftsearch/manage-verticals) и [типы результатов](/en-us/microsoftsearch/manage-result-types) или воспользовавшись [API поиска Microsoft Graph](/graph/api/resources/search-api-overview?view=graph-rest-1.0&preserve-view=true).

## <a name="add-an-item"></a>Добавление элемента

Чтобы добавить элемент в индекс, необходимо [создать externalItem](/graph/api/externalconnectors-externalconnection-put-items?view=graph-rest-beta&preserve-view=true&tabs=http&viewFallbackFrom=graph-rest-1.0). При создании элемента ему назначается уникальный идентификатор в URL-адресе.

Например, приложение может индексировать запросы в службу технической поддержки по их номерам. Если запросу назначен номер `SR00145`, он может выглядеть так:

```http
PUT /external/connections/contosohelpdesk/items/SR00145
Content-Type: application/json

{
  "title": "WiFi outage in Conference Room A",
  "status": "New",
  "assignee": "meganb@contoso.com"
}
```

> [!NOTE]
> Перед поиском индексированных элементов в пользовательском интерфейсе "Поиск (Майкрософт)", администратор должен [настроить страницу результатов поиска](/en-us/microsoftsearch/configure-connector#next-steps-customize-the-search-results-page) для соответствующего подключения.

## <a name="update-an-item"></a>Обновление элемента

При обновлении элемента во внешней службе (переназначении запросов в службу технической поддержки или обновлении описания продукта), вы можете [обновить соответствующую запись в индексе, обновив externalItem](/graph/api/externalconnectors-externalitem-update?view=graph-rest-1.0&preserve-view=true&tabs=http) по уникальному идентификатору, назначенному элементу при его создании.

```http
PATCH /external/connections/contosohelpdesk/items/SR00145
Content-Type: application/json

{
  "assignee": "alexw@contoso.com"
}
```

## <a name="delete-an-item"></a>Удаление элемента

Чтобы удалить элементы из индекса, [удалите externalItem](/graph/api/externalconnectors-externalitem-delete?view=graph-rest-1.0&preserve-view=true&tabs=http), используя уникальный идентификатор, присвоенный элементу при его создания.

```http
DELETE /external/connections/contosohelpdesk/items/SR00145
```

## <a name="next-steps"></a>Дальнейшие действия

- [Использование внешних групп для управления разрешениями](connecting-external-content-external-groups.md)
- [Запросы с использованием API Поиска (Майкрософт)](search-concept-overview.md#why-use-the-microsoft-search-api)
- [Обзор справочника API соединителей Microsoft Graph](/graph/api/resources/indexing-api-overview?view=graph-rest-1.0&preserve-view=true)
- [Поиск объектов настраиваемого типа (externalItem)](search-concept-custom-types.md)
- [Скачайте образец соединителя поиска с сайта GitHub](https://github.com/microsoftgraph/msgraph-search-connector-sample)