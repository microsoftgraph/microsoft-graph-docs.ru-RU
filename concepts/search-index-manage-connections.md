---
title: Создание, обновление и удаление подключений к службе "Поиск (Майкрософт)"
description: Узнайте, как использовать Microsoft Graph для управления подключениями к службе "Поиск (Майкрософт)".
localization_priority: Priority
author: snlraju-msft
ms.prod: ''
doc_type: conceptualPageType
ms.openlocfilehash: 9f2d09cbd82a21874cf870c3214100115b225a1f
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/19/2019
ms.locfileid: "38704381"
---
# <a name="create-update-and-delete-connections-to-the-microsoft-search-service"></a>Создание, обновление и удаление подключений к службе "Поиск (Майкрософт)"

Подключения внешних служб к службе "Поиск (Майкрософт)" представляются ресурсом [externalConnection](/graph/api/resources/externalconnection?view=graph-rest-beta) в Microsoft Graph.

[!INCLUDE [search-api-preview-signup](../includes/search-api-preview-signup.md)]

Подключение позволяет приложению [определить схему](/graph/api/externalconnection-post-schema?view=graph-rest-beta) для индексируемых элементов, а также предоставляет службе конечную точку для [добавления, обновления и удаления элементов индекса](search-index-manage-items.md). Создание подключения — первый шаг приложения к добавлению элементов в индекс поиска.

## <a name="create-a-connection"></a>Создание подключения

Чтобы приложение могло добавлять элементы в индекс поиска, ему необходимо создать и настроить подключение, выполнив указанные ниже действия.

- [Создание подключения](/graph/api/external-post-connections?view=graph-rest-beta) с уникальным идентификатором, отображаемым именем и описанием.
- [Регистрация схемы](/graph/api/externalconnection-post-schema?view=graph-rest-beta).
  - Для пользовательских элементов (например, обращений в службу технической поддержки, записей базы данных инвентаризации и т. д.) необходимо определить поля, включенные в индекс.
  - Для внешних файлов следует задать тип `microsoft.graph.externalFile`.

> [!IMPORTANT]
> После регистрации схемы ее невозможно изменить для существующего подключения.

## <a name="update-a-connection"></a>Обновление подключения

Вы можете изменить отображаемое имя или описание существующего подключения, [обновив подключение](/graph/api/externalconnection-update?view=graph-rest-beta).

## <a name="delete-a-connection"></a>Удаление подключения

Вы можете [удалить подключение](/graph/api/externalconnection-delete?view=graph-rest-beta) и удалить все элементы, индексированные через него.

## <a name="next-steps"></a>Дальнейшие действия

- [Зачем использовать API Поиска (Майкрософт)?](search-concept-overview.md#why-use-the-microsoft-search-api)
- [Использование API Поиска (Майкрософт) для индексирования данных](/graph/api/resources/indexing-api-overview?view=graph-rest-beta)
- [Обзор соединителей Microsoft Graph](/microsoftsearch/connectors-overview)
- Скачайте [образец соединителя поиска](https://github.com/microsoftgraph/msgraph-search-connector-sample) с сайта GitHub.
