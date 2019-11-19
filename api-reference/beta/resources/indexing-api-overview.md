---
title: Индексирование данных с помощью API Поиска (Майкрософт)
description: Microsoft Graph позволяет приложению индексировать пользовательские элементы или внешние файлы в службе "Поиск (Майкрософт)".
localization_priority: Priority
author: snlraju-msft
ms.prod: ''
doc_type: conceptualPageType
ms.openlocfilehash: e6afa7be0f1bf7dbda0561f8bd0e89ce8b0a3e4d
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/19/2019
ms.locfileid: "38703786"
---
# <a name="use-the-microsoft-search-api-to-index-data"></a>Индексирование данных с помощью API Поиска (Майкрософт)

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Microsoft Graph позволяет приложению добавлять настраиваемые элементы или внешние файлы в результаты поиска в службе [Поиск (Майкрософт)](/microsoftsearch/overview-microsoft-search).

Запросы на индексирование данных выполняются от имени приложения без вошедшего пользователя, указываемого [маркером доступа с разрешением приложения](/graph/auth-v2-service).

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="common-use-cases"></a>Распространенные варианты использования

Варианты использования интерфейсов API в этом разделе сосредоточены на создании [соединителей Microsoft Graph](/microsoftsearch/connectors-overview), включающем следующие основные этапы:

1. [создание подключения](../api/external-post-connections.md) к внешнему источнику данных;
2. [создание и регистрация схемы](../api/externalconnection-post-schema.md), описывающей тип и способ индексирования внешних данных;
3. [индексирование данных](../api/externalconnection-put-items.md) в качестве внешнего элемента или файла.

| Варианты использования                                        | Ресурсы REST                              | См. также |
|:-------------------------------------------------|:--------------------------------------------|:--|
| **Действия для настройки**                        |                                             |   |
| Создание, обновление или удаление подключения           | [externalConnection](externalconnection.md) | [Методы объекта externalConnection](externalconnection.md#methods) |
| Регистрация схемы для внешних данных          | [schema](schema.md)                         | [Методы объекта schema](schema.md#methods) |
| **Действия для индексирования**                             |                                             |   |
| Добавление, обновление или удаление пользовательского элемента индекса | [externalItem](externalitem.md)             | [Методы объекта externalItem](externalItem.md#methods) |
| Добавление, обновление или удаление файла в индексе        | [externalFile](externalfile.md)             | [Методы объекта externalFile](externalfile.md#methods) |

## <a name="known-limitations"></a>Известные ограничения

Работая с предварительной версией, учитывайте описанные ниже факторы.

- Организациям доступно до 10 подключений.
- Настраиваемые свойства не поддерживаются при индексировании файлов с помощью ресурса `externalFile`.
- Поддерживаются только удостоверения Azure Active Directory.
- Создание ресурсов `externalItem` или `externalFile` ограничено до 4 элементов в секунду.
- Приложение может выполнять до 4 одновременных операций с подключением.
- Емкость подключений ограничена до 700 000 элементов, или примерно 70 ГБ данных.
- Максимальный размер объекта `externalItem` или `externalFile` составляет 4 МБ.
- Уточнение и сортировка результатов не поддерживается.
- Результаты ранжируются наилучшим возможным способом.

## <a name="next-steps"></a>Дальнейшие действия

- [Обзор API Поиска (Майкрософт)](/graph/search-concept-overview)
- Подробное описание методов, свойств и связей ресурсов [externalConnection](externalconnection.md), [schema](schema.md), [externalItem](externalitem.md) и [externalFile](externalfile.md).
- Ознакомьтесь с [примером соединителя поиска](https://github.com/microsoftgraph/msgraph-search-connector-sample) на сайте GitHub.
