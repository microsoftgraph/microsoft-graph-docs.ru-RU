---
title: Работа с API соединителей
description: Обзор API соединителей Microsoft Graph
author: mecampos
localization_priority: Priority
doc_type: conceptualPageType
ms.prod: search
ms.openlocfilehash: 63e11b086592a46a4e519a2ab7c79c20d049213a
ms.sourcegitcommit: cec76c5a58b359d79df764c849c8b459349b3b52
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2021
ms.locfileid: "52646296"
---
# <a name="working-with-the-connectors-api"></a>Работа с API соединителей

Соединители Microsoft Graph — это простой способ добавления внешних данных в Microsoft Graph и улучшения интеллектуальных технологий Microsoft 365. Для интеграции со службами, которые недоступны в роли соединителей, созданных корпорацией Майкрософт, необходимо создать настраиваемый соединитель. Чтобы создать настраиваемые соединители, используйте REST API соединителей Microsoft Graph.

![Изображение внешних данных, исходящих из разных соединителей Microsoft Graph](./images/connectors-images/api-overview.png)

Используйте API Microsoft Graph, чтобы выполнять следующие задачи:

1. Создание подключений к внешним данным и управление ими.
2. Определение и регистрация схем внешних типов данных.
3. Запись элементов внешних данных в Microsoft Graph.
4. Синхронизация внешних групп.

Дополнительные сведения об этих API можно найти в документации, представленной далее.

## <a name="connections-api"></a>API подключений

Подключение — это логический контейнер для внешних данных, которыми вы можете управлять как единым целым.
Дополнительную информацию о создании, обновлении и удалении подключений в Microsoft Graph можно найти в разделе [Управление подключениями](connecting-external-content-manage-connections.md).

## <a name="schema-api"></a>API схем

[Схема](/graph/api/resources/schema?view=graph-rest-beta&amp;preserve-view=true) связей определяет, как ваше содержимое будет использоваться в различных интерфейсах Microsoft 365. Схема — это плоский список всех свойств, которые вы планируете добавить в связь, а также их атрибуты, метки и псевдонимы. Перед добавлением элементов в Microsoft Graph вы должны зарегистрировать схему.

Дополнительную информацию о регистрации схемы для подключения Microsoft Graph и его свойствах можно найти в разделе [Управление схемой](connecting-external-content-manage-schema.md).

## <a name="ingest-external-data-items"></a>Прием элементов внешних данных

Соединители Microsoft Graph — это простой способ добавления внешних данных в Microsoft Graph. Элементы, добавленные приложением в службу "Поиск (Майкрософт)", представлены ресурсом [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true) в Microsoft Graph.

Дополнительные сведения о создании, обновлении и удалении элементов, добавленных приложением через соединители Microsoft Graph см. в разделе [Управление элементами](connecting-external-content-manage-items.md).

## <a name="external-groups-api"></a>API внешних групп

Элементам во внешней службе может предоставляться или отказываться в доступе через ACL к различным типам групп, отличных от Azure Active Directory. Например, элементы Salesforce могут иметь наборы разрешений и профили. Элементы ServiceNow могут иметь локальные группы. При записи этих элементов в Microsoft Graph необходимо соблюдать эти ACL.

Вы можете использовать API внешних групп, чтобы настроить разрешения для внешних элементов, которые будут записаны в Microsoft Graph. [externalGroup](/graph/api/externalgroup-post-members?view=graph-rest-beta&amp;preserve-view=true) представляет группу, отличную от Azure Active Directory или групповую конструкцию (например, бизнес-единицы, Teams и так далее) и определяет разрешения на содержимое во внешнем источнике данных.