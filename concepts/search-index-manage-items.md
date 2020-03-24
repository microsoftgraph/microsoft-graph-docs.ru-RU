---
title: Создание, обновление и удаление элементов, добавленных приложением в индекс службы "Поиск (Майкрософт)"
description: Узнайте, как использовать Microsoft Graph для управления элементами, добавленными приложением в службу "Поиск (Майкрософт)".
localization_priority: Priority
author: snlraju-msft
ms.prod: ''
doc_type: conceptualPageType
ms.openlocfilehash: 5b969bd058b8c1e2790b0039a4369623287f641d
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/21/2020
ms.locfileid: "42892788"
---
# <a name="create-update-and-delete-items-added-by-your-application-in-the-microsoft-search-service-index"></a>Создание, обновление и удаление элементов, добавленных приложением в индекс службы "Поиск (Майкрософт)"

Элементы, добавленные приложением в службу "Поиск (Майкрософт)", представлены ресурсом [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta) в Microsoft Graph.

[!INCLUDE [search-api-preview-signup](../includes/search-api-preview-signup.md)]

## <a name="add-an-item"></a>Добавление элемента

Вы можете добавить элемент в индекс, [создав объект externalItem](/graph/api/externalconnection-put-items?view=graph-rest-beta). При создании элемента ему назначается уникальный идентификатор в URL-адресе.

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

При обновлении элемента во внешней службе (переназначении запросов в службу технической поддержки или обновлении описания продукта), вы можете обновить соответствующую запись в индексе, [обновив externalItem](/graph/api/externalitem-update?view=graph-rest-beta) по уникальному идентификатору, назначенному элементу при его создании.

```http
PATCH /external/connections/contosohelpdesk/items/SR00145
Content-Type: application/json

{
  "assignee": "alexw@contoso.com"
}
```

## <a name="delete-an-item"></a>Удаление элемента

Вы можете удалить элементы из индекса, [удалив externalItem](/graph/api/externalitem-delete?view=graph-rest-beta) по уникальному идентификатору, назначенному при его создании.

```http
DELETE /external/connections/contosohelpdesk/items/SR00145
```

## <a name="next-steps"></a>Дальнейшие действия

- [Зачем использовать API Поиска (Майкрософт)?](search-concept-overview.md#why-use-the-microsoft-search-api)
- [Обзор индексирования справочных материалов по API](/graph/api/resources/indexing-api-overview?view=graph-rest-beta)
- [Настройка страницы результатов поиска Microsoft](/MicrosoftSearch/configure-connector#next-steps-customize-the-search-results-page)
- [Поиск объектов настраиваемого типа (externalItem)](search-concept-custom-types.md)
- Скачайте [образец соединителя поиска](https://github.com/microsoftgraph/msgraph-search-connector-sample) с сайта GitHub.
