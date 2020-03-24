---
title: Создание, обновление и удаление подключений к службе "Поиск (Майкрософт)"
description: Узнайте, как использовать Microsoft Graph для управления подключениями к службе "Поиск (Майкрософт)".
localization_priority: Priority
author: snlraju-msft
ms.prod: ''
doc_type: conceptualPageType
ms.openlocfilehash: 99f0ab4591caa6c311f2771f1c6a0772a8f16087
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/21/2020
ms.locfileid: "42892802"
---
# <a name="create-update-and-delete-connections-to-the-microsoft-search-service"></a>Создание, обновление и удаление подключений к службе "Поиск (Майкрософт)"

Подключения внешних служб к службе "Поиск (Майкрософт)" представляются ресурсом [externalConnection](/graph/api/resources/externalconnection?view=graph-rest-beta) в Microsoft Graph.

[!INCLUDE [search-api-preview-signup](../includes/search-api-preview-signup.md)]

Подключение позволяет приложению [определить схему](/graph/api/externalconnection-post-schema?view=graph-rest-beta) для индексируемых элементов, а также предоставляет службе конечную точку для [добавления, обновления и удаления элементов индекса](search-index-manage-items.md). Создание подключения — первый шаг приложения к добавлению элементов в индекс поиска.

## <a name="create-a-connection"></a>Создание подключения

Чтобы приложение могло добавлять элементы в индекс поиска, ему необходимо создать и настроить подключение, выполнив указанные ниже действия.

- [Создание подключения](/graph/api/external-post-connections?view=graph-rest-beta) с уникальным идентификатором, отображаемым именем и описанием.
- [Зарегистрируйте схему](/graph/api/externalconnection-post-schema?view=graph-rest-beta), чтобы определить поля, которые будут включены в индекс.

> [!IMPORTANT]
> После регистрации схемы ее невозможно изменить для существующего подключения.

## <a name="update-a-connection"></a>Обновление подключения

Вы можете изменить отображаемое имя или описание существующего подключения, [обновив подключение](/graph/api/externalconnection-update?view=graph-rest-beta).

## <a name="delete-a-connection"></a>Удаление подключения

Вы можете [удалить подключение](/graph/api/externalconnection-delete?view=graph-rest-beta) и удалить все элементы, индексированные через него.

## <a name="next-steps"></a>Дальнейшие действия

- [Зачем использовать API Поиска (Майкрософт)?](search-concept-overview.md#why-use-the-microsoft-search-api)
- [Обзор индексирования справочных материалов по API](/graph/api/resources/indexing-api-overview?view=graph-rest-beta)
- [Обзор соединителей Microsoft Graph](/microsoftsearch/connectors-overview)
- Скачайте [образец соединителя поиска](https://github.com/microsoftgraph/msgraph-search-connector-sample) с сайта GitHub.
