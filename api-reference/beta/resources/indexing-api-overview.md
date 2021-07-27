---
title: Индексирование данных с помощью API Поиска (Майкрософт)
description: Используйте Microsoft Graph для индексирования пользовательских элементов в службе поиска Microsoft.
localization_priority: Priority
author: snlraju-msft
ms.prod: search
doc_type: conceptualPageType
ms.openlocfilehash: 37e98b3cebd75f08a4193c312994af7c697a0bab
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467108"
---
# <a name="use-the-microsoft-search-api-to-index-data"></a>Индексирование данных с помощью API Поиска (Майкрософт)

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Вы можете использовать Microsoft Graph для добавления пользовательских элементов в результаты поиска в режиме [поиска Microsoft](/microsoftsearch/overview-microsoft-search).

Запросы на индексирование данных выполняются от имени приложения без вошедшего пользователя, указываемого [маркером доступа с разрешением приложения](/graph/auth-v2-service).

## <a name="common-use-cases"></a>Основные варианты использования

Варианты использования интерфейсов API в этом разделе содержат создание [соединителей Microsoft Graph](/microsoftsearch/connectors-overview), включая следующие основные этапы:

1. [Создание подключения](../api/externalconnectors-external-post-connections.md) к внешнему источнику данных.
2. [Создание и регистрация схемы](../api/externalconnectors-externalconnection-post-schema.md), описывающей тип и способ индексирования внешних данных.
3. [Индексируйте данные](../api/externalconnectors-externalconnection-put-items.md) как внешний элемент.

| Варианты использования                                        | Ресурсы REST                              | См. также |
|:-------------------------------------------------|:--------------------------------------------|:--|
| **Действия для настройки**                        |                                             |   |
| Создание, обновление или удаление подключения           | [externalConnection](externalconnectors-externalconnection.md) | [Методы externalConnection](externalconnectors-externalconnection.md#methods) |
| Регистрация схемы для внешних данных          | [schema](externalconnectors-schema.md)                         | [Методы schema](externalconnectors-schema.md#methods) |
| **Действия для индексирования**                             |                                             |   |
| Добавление, обновление или удаление пользовательского элемента индекса | [externalItem](externalconnectors-externalitem.md)             | [Методы externalItem](externalconnectors-externalitem.md#methods) |

## <a name="known-limitations"></a>Известные ограничения

Далее представлены текущие известные ограничения:

- Организациям доступно до 10 подключений.
- Вы можете создавать только четыре `externalItem` элемента ресурсов в секунду.
- Приложение может выполнять до четырех одновременных операций с подключением.
- Емкость подключений ограничена до 700 000 элементов, или примерно 70 ГБ данных.
- Максимальный размер объекта `externalItem` составляет 4 МБ.
- Сортировка результатов не поддерживается.

## <a name="whats-new"></a>Новые возможности
Узнайте о [новых функциях и обновлениях](/graph/whats-new-overview) для этого набора API.

## <a name="next-steps"></a>Дальнейшие действия

- См. статью [Обзор API Поиска (Майкрософт)](/graph/search-concept-overview).
- Разверните методы, свойства и отношения ресурсов [externalConnection](externalconnectors-externalconnection.md), [схемы](externalconnectors-schema.md) и [externalItem](externalconnectors-externalitem.md).
- Ознакомьтесь с [коллекцией Postman Microsoft Graph](https://www.postman.com/microsoftgraph/workspace/microsoft-graph/folder/455214-66cbb476-ad94-448e-ba5a-ef58e1da7a90?ctx=documentation) ([подробнее](https://developer.microsoft.com/ru-RU/graph/blogs/postman-collections))
- Ознакомьтесь с [примером соединителя поиска](https://github.com/microsoftgraph/msgraph-search-connector-sample) на сайте GitHub.


