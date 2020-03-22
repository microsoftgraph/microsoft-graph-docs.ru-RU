---
title: Индексирование данных с помощью API Поиска (Майкрософт)
description: Используйте Microsoft Graph для индексирования пользовательских элементов в службе поиска Microsoft.
localization_priority: Priority
author: snlraju-msft
ms.prod: search
doc_type: conceptualPageType
ms.openlocfilehash: 2d6c49fcdb0a25c0c15fce6c7f7ae0880a3968dd
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/21/2020
ms.locfileid: "42892627"
---
# <a name="use-the-microsoft-search-api-to-index-data"></a>Индексирование данных с помощью API Поиска (Майкрософт)

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Вы можете использовать Microsoft Graph для добавления пользовательских элементов в результаты поиска в режиме [поиска Microsoft](/microsoftsearch/overview-microsoft-search).

Запросы на индексирование данных выполняются от имени приложения без вошедшего пользователя, указываемого [маркером доступа с разрешением приложения](/graph/auth-v2-service).

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="common-use-cases"></a>Основные варианты использования

Варианты использования интерфейсов API в этом разделе содержат создание [соединителей Microsoft Graph](/microsoftsearch/connectors-overview), включая следующие основные этапы:

1. [Создание подключения](../api/external-post-connections.md) к внешнему источнику данных.
2. [Создание и регистрация схемы](../api/externalconnection-post-schema.md), описывающей тип и способ индексирования внешних данных.
3. [Индексируйте данные](../api/externalconnection-put-items.md) как внешний элемент.

| Варианты использования                                        | Ресурсы REST                              | См. также |
|:-------------------------------------------------|:--------------------------------------------|:--|
| **Действия для настройки**                        |                                             |   |
| Создание, обновление или удаление подключения           | [externalConnection](externalconnection.md) | [Методы externalConnection](externalconnection.md#methods) |
| Регистрация схемы для внешних данных          | [schema](schema.md)                         | [Методы schema](schema.md#methods) |
| **Действия для индексирования**                             |                                             |   |
| Добавление, обновление или удаление пользовательского элемента индекса | [externalItem](externalitem.md)             | [Методы externalItem](externalItem.md#methods) |

## <a name="known-limitations"></a>Известные ограничения

Далее представлены известные ограничения:

- Организациям доступно до 10 подключений.
- Поддерживаются только удостоверения Azure Active Directory.
- Вы можете создавать только четыре `externalItem` элемента ресурсов в секунду.
- Приложение может выполнять до четырех одновременных операций с подключением.
- Емкость подключений ограничена до 700 000 элементов, или примерно 70 ГБ данных.
- Максимальный размер объекта `externalItem` составляет 4 МБ.
- Уточнение и сортировка результатов не поддерживается.
- Результаты ранжируются наилучшим возможным способом.

## <a name="next-steps"></a>Дальнейшие действия

- См. статью [Обзор API Поиска (Майкрософт)](/graph/search-concept-overview).
- Разверните методы, свойства и отношения ресурсов [externalConnection](externalconnection.md), [схемы](schema.md) и [externalItem](externalitem.md).
- Ознакомьтесь с [примером соединителя поиска](https://github.com/microsoftgraph/msgraph-search-connector-sample) на сайте GitHub.
