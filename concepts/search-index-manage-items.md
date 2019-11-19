---
title: Создание, обновление и удаление элементов, добавленных приложением в индекс службы "Поиск (Майкрософт)"
description: Узнайте, как использовать Microsoft Graph для управления элементами, добавленными приложением в службу "Поиск (Майкрософт)".
localization_priority: Priority
author: snlraju-msft
ms.prod: ''
doc_type: conceptualPageType
ms.openlocfilehash: c5017943f966792e0246d3764a1c3e373718c63c
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/19/2019
ms.locfileid: "38704338"
---
# <a name="create-update-and-delete-items-added-by-your-application-in-the-microsoft-search-service-index"></a>Создание, обновление и удаление элементов, добавленных приложением в индекс службы "Поиск (Майкрософт)"

Элементы, добавленные приложением в службу "Поиск (Майкрософт)", представлены ресурсами [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta) и [externalFile](/graph/api/resources/externalfile?view=graph-rest-beta) в Microsoft Graph.

[!INCLUDE [search-api-preview-signup](../includes/search-api-preview-signup.md)]

Ресурс **externalItem** представляет настраиваемый тип. Его следует использовать, если элементы, добавленные в индекс, основаны на пользовательской схеме, не представленной ресурсом **externalFile**. Например, это могут быть запросы в службу технической поддержки или описания продуктов.

Ресурс **externalFile** представляет файл во внешней системе.

> [!NOTE]
> Схему **externalFile** невозможно расширить.

## <a name="add-an-item-or-file"></a>Добавление элемента или файла

Вы можете добавить элемент или файл в индекс, [создав объект externalItem](/graph/api/externalconnection-put-items?view=graph-rest-beta). При создании элемента ему назначается уникальный идентификатор в URL-адресе.

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

## <a name="update-an-item-or-file"></a>Обновление элемента или файла

При обновлении элемента или файла во внешней службе (переназначении запросов в службу технической поддержки или обновлении описания продукта), вы можете обновить соответствующую запись в индексе, [обновив объект externalItem](/graph/api/externalitem-update?view=graph-rest-beta) по уникальному идентификатору, назначенному элементу при его создании.

```http
PATCH /external/connections/contosohelpdesk/items/SR00145
Content-Type: application/json

{
  "assignee": "alexw@contoso.com"
}
```

## <a name="delete-an-item-or-file"></a>Удаление элемента или файла

Вы можете удалить элементы или файлы из индекса, [удалив объект externalItem](/graph/api/externalitem-delete?view=graph-rest-beta) по уникальному идентификатору, назначенному при его создании.

```http
DELETE /external/connections/contosohelpdesk/items/SR00145
```

## <a name="next-steps"></a>Дальнейшие действия

- [Зачем использовать API Поиска (Майкрософт)?](search-concept-overview.md#why-use-the-microsoft-search-api)
- [Использование API Поиска (Майкрософт) для индексирования данных](/graph/api/resources/indexing-api-overview?view=graph-rest-beta)
- [Поиск объектов настраиваемого типа (externalItem)](search-concept-custom-types.md)
- [Поиск файлов (включая externalFile)](search-concept-files.md)
- Скачайте [образец соединителя поиска](https://github.com/microsoftgraph/msgraph-search-connector-sample) с сайта GitHub.
