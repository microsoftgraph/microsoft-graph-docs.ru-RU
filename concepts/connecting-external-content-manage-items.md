---
title: Создание, обновление и удаление элементов, добавленных приложением в связь Microsoft Graph
description: Узнайте, как использовать Microsoft Graph для управления элементами, добавленными приложением в службу "Поиск (Майкрософт)".
ms.localizationpriority: high
author: mecampos
doc_type: conceptualPageType
ms.prod: search
ms.openlocfilehash: 5da57fe2bca541786addf0e4472497965ff9b038
ms.sourcegitcommit: f5382652b6880fab42040df40a08de7cb2d74d35
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/17/2022
ms.locfileid: "63559795"
---
<!---<author of this doc: rsamai>--->

# <a name="create-update-and-delete-items-added-by-your-application-via-microsoft-graph-connectors"></a>Создание, обновление и удаление элементов, добавленных приложением с помощью соединителей Microsoft Graph

Соединители Microsoft Graph — это простой способ добавления внешних данных в Microsoft Graph. Элементы, добавленные приложением в службу "Поиск (Майкрософт)", представлены ресурсом [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true) в Microsoft Graph.

После [создания связи](/graph/api/external-post-connections?view=graph-rest-beta&preserve-view=true) вы можете добавить содержимое. Каждый элемент из источника данных должен быть представлен в виде [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true) в Microsoft Graph с уникальным идентификатором элемента. Этот идентификатор используется для создания, обновления или удаления элемента в Microsoft Graph. Вы можете использовать первичный ключ из источника данных в качестве itemId или получить его из одного или нескольких полей. **externalItem** содержит три основных компонента: список управления доступом, свойства и содержимое.

## <a name="access-control-list"></a>Список управления доступом

Список управления доступом используется для указания того, предоставляется ли определенным ролям доступ для просмотра элементов в интерфейсах Майкрософт. Это массив записей управления доступом, каждая из которых представляет пользователя или группу Azure Active Directory. Существует третий тип записей управления доступом: `Everyone`, который представляет всех пользователей в клиенте.

![Пример списка управления доступом](./images/connectors-images/connecting-external-content-manage-items-acl.png)

Значение **accessType** `deny` имеет приоритет над `grant`. Например, хотя в представленном ранее элементе доступ предоставлен с помощью параметра `Everyone`, а конкретному пользователю доступ запрещен, действующим разрешением для этого пользователя будет вариант `deny`.

Если ваш источник данных не содержит групп Azure Active Directory, таких как группы в вашей службе поддержки, применяемых для настройки разрешений для элемента, вы можете создать внешние группы в Microsoft Graph, используя API синхронизации группы для репликации разрешений `allow` или `deny`. Избегайте расширения участия ваших внешних групп непосредственно в списках управления доступом отдельных элементов, так как каждое участие группы может привести к многочисленным обновлениям элементов.

Внешние группы могут состоять из других внешних групп, пользователей Azure Active Directory и групп Azure Active Directory. Если у вас есть пользователи не из Azure Active Directory, вы должны преобразовать их в пользователей Azure Active Directory в своем списке управления доступом.

## <a name="properties"></a>Свойства

С помощью компонента свойств можно добавлять метаданные элементов, которые удобно применять в интерфейсах Microsoft Graph. Вы должны [зарегистрировать схему](./connecting-external-content-manage-schema.md) для связи перед добавлением в нее элементов и преобразованием **типов данных** в [поддерживаемые типы данных](/graph/api/resources/property?view=graph-rest-beta&preserve-view=true).

![Пример компонента свойства](./images/connectors-images/connecting-external-content-manage-items-1.png)

## <a name="content"></a>Содержимое

Компонент содержимого используется для массового добавления элементов, которые должны быть полнотекстовым индексом. Примеры включают описание запроса, проанализированный текст из файла или вики-страницы.

Содержимое — одно из ключевых полей, влияющих на [релевантность](./connecting-external-content-manage-schema.md#relevance) в интерфейсах Майкрософт. Поддерживаются типы контента: `text` и `html`. Если источник данных содержит контент других типов, например двоичные файлы, видео или изображения, вы можете преобразовать их в текстовую форму перед добавлением в Microsoft Graph. Например, для извлечения из изображений пригодного для поиска текста можно использовать распознавание текста.

![Пример компонента содержимого](./images/connectors-images/connecting-external-content-manage-items-2.png)

Содержимое нельзя непосредственно добавить в шаблон результатов поиска, но вы можете использовать созданный фрагмент результатов, являющийся динамически создаваемым предварительным просмотром соответствующих разделов в содержимом.

![Снимок экрана с шаблоном результатов поиска](./images/connectors-images/connecting-external-content-manage-items-3.svg)

При изменении содержимого в источнике данных вы должны синхронизировать его с элементами связи. Вы можете обновить весь элемент или обновить один или несколько его компонентов. После добавления содержимого в Microsoft Graph вы можете искать его с помощью интерфейса Поиска (Майкрософт), настроив [вертикали и типы результатов](/MicrosoftSearch/customize-search-page) или воспользовавшись [API поиска Microsoft Graph](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true).

## <a name="add-an-item"></a>Добавление элемента

Вы можете добавить элемент в индекс, [создав объект externalItem](/graph/api/externalconnection-put-items?view=graph-rest-beta&preserve-view=true). При создании элемента ему назначается уникальный идентификатор в URL-адресе.

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

> ![ПРИМЕЧАНИЕ] Перед поиском индексированных элементов в пользовательском интерфейсе "Поиск (Майкрософт)", администратор должен [настроить страницу результатов поиска](/MicrosoftSearch/configure-connector#next-steps-customize-the-search-results-page) для соответствующего подключения.

## <a name="update-an-item"></a>Обновление элемента

При обновлении элемента во внешней службе (переназначении запросов в службу технической поддержки или обновлении описания продукта), вы можете обновить соответствующую запись в индексе, [обновив externalItem](/graph/api/externalitem-update?view=graph-rest-beta&preserve-view=true) по уникальному идентификатору, назначенному элементу при его создании.

```http
PATCH /external/connections/contosohelpdesk/items/SR00145
Content-Type: application/json

{
  "assignee": "alexw@contoso.com"
}
```

## <a name="delete-an-item"></a>Удаление элемента

Вы можете удалить элементы из индекса, [удалив externalItem](/graph/api/externalitem-delete?view=graph-rest-beta&preserve-view=true) по уникальному идентификатору, назначенному при его создании.

```http
DELETE /external/connections/contosohelpdesk/items/SR00145
```

## <a name="see-also"></a>См. также

- [Запросы с использованием API Поиска (Майкрософт)](search-concept-overview.md#why-use-the-microsoft-search-api)
- [Обзор индексирования справочных материалов по API](/graph/api/resources/indexing-api-overview?view=graph-rest-beta&preserve-view=true)
- [Настройка страницы результатов поиска Microsoft](/MicrosoftSearch/customize-search-page)
- [Поиск объектов настраиваемого типа (externalItem)](search-concept-custom-types.md)
- Скачайте [образец соединителя поиска](https://github.com/microsoftgraph/msgraph-search-connector-sample) с сайта GitHub.
