---
title: Индексирование данных с помощью API Поиска (Майкрософт)
description: Используйте Microsoft Graph, чтобы индексировать пользовательские элементы или внешние файлы в службе Поиска (Майкрософт).
localization_priority: Priority
author: snlraju-msft
ms.prod: search
doc_type: conceptualPageType
ms.openlocfilehash: f1a39a42f94a072c501c288b55a6b665af0fc640
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870231"
---
# <a name="use-the-microsoft-search-api-to-index-data"></a>Индексирование данных с помощью API Поиска (Майкрософт)

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Вы можете использовать Microsoft Graph для добавления пользовательских элементов или внешних файлов в результаты поиска в интерфейсе [Поиска (Майкрософт)](/microsoftsearch/overview-microsoft-search).

Запросы на индексирование данных выполняются от имени приложения без вошедшего пользователя, указываемого [маркером доступа с разрешением приложения](/graph/auth-v2-service).

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="common-use-cases"></a>Основные варианты использования

Варианты использования интерфейсов API в этом разделе содержат создание [соединителей Microsoft Graph](/microsoftsearch/connectors-overview), включая следующие основные этапы:

1. [Создание подключения](../api/external-post-connections.md) к внешнему источнику данных.
2. [Создание и регистрация схемы](../api/externalconnection-post-schema.md), описывающей тип и способ индексирования внешних данных.
3. [Индексирование данных](../api/externalconnection-put-items.md) в качестве внешнего элемента или файла.

| Варианты использования                                        | Ресурсы REST                              | См. также |
|:-------------------------------------------------|:--------------------------------------------|:--|
| **Действия для настройки**                        |                                             |   |
| Создание, обновление или удаление подключения           | [externalConnection](externalconnection.md) | [Методы externalConnection](externalconnection.md#methods) |
| Регистрация схемы для внешних данных          | [schema](schema.md)                         | [Методы schema](schema.md#methods) |
| **Действия для индексирования**                             |                                             |   |
| Добавление, обновление или удаление пользовательского элемента индекса | [externalItem](externalitem.md)             | [Методы externalItem](externalItem.md#methods) |
| Добавление, обновление или удаление файла в индексе        | [externalFile](externalfile.md)             | [Методы externalFile](externalfile.md#methods) |

## <a name="known-limitations"></a>Известные ограничения

Далее представлены известные ограничения:

- Организациям доступно до 10 подключений.
- Настраиваемые свойства не поддерживаются при индексировании файлов с помощью ресурса `externalFile`.
- Поддерживаются только удостоверения Azure Active Directory.
- В секунду можно создавать только четыре элемента ресурсов `externalItem` или `externalFile` в секунду.
- Приложение может выполнять до четырех одновременных операций с подключением.
- Емкость подключений ограничена до 700 000 элементов, или примерно 70 ГБ данных.
- Максимальный размер объекта `externalItem` или `externalFile` составляет 4 МБ.
- Уточнение и сортировка результатов не поддерживается.
- Результаты ранжируются наилучшим возможным способом.

## <a name="next-steps"></a>Дальнейшие действия

- См. статью [Обзор API Поиска (Майкрософт)](/graph/search-concept-overview).
- Подробное описание методов, свойств и связей ресурсов [externalConnection](externalconnection.md), [schema](schema.md), [externalItem](externalitem.md) и [externalFile](externalfile.md).
- Ознакомьтесь с [примером соединителя поиска](https://github.com/microsoftgraph/msgraph-search-connector-sample) на сайте GitHub.
