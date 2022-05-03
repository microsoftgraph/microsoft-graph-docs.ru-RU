---
title: Работа с API соединителей Microsoft Graph
description: Получите обзор API соединителей Microsoft Graph, включая API внешнего подключения, API схемы, API внешнего элемента и API внешней группы.
author: mecampos
ms.localizationpriority: high
doc_type: conceptualPageType
ms.prod: search
ms.openlocfilehash: 8f43cea536bcec1b371dbdea714d70698ffbc583
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176816"
---
# <a name="work-with-the-microsoft-graph-connectors-api"></a>Работа с API соединителей Microsoft Graph

Соединители Microsoft Graph предлагают интуитивно понятный способ переноса внешних данных в Microsoft Graph и улучшения интеллектуальных возможностей Microsoft 365. Для интеграции со службами, которые недоступны в роли соединителей, созданных корпорацией Майкрософт, необходимо создать настраиваемый соединитель. Для создания настраиваемых соединителей вы используете REST API соединителей Microsoft Graph.

![Изображение внешних данных, исходящих из разных соединителей Microsoft Graph](./images/connectors-images/api-overview.png)

Используйте API Microsoft Graph, чтобы выполнять следующие задачи:

1. Создание подключений к внешним данным и управление ими.
2. Определите и зарегистрируйте схему внешних типов данных.
3. Запись элементов внешних данных в Microsoft Graph.
4. Синхронизация внешних групп.

## <a name="external-connection-api"></a>API внешнего подключения

[externalConnection](/graph/api/resources/externalconnectors-externalconnection?view=graph-rest-1.0&preserve-view=true) — это логический контейнер для внешних данных, которым вы можете управлять как единым блоком.

Подробнее см. в статье [Создание, обновление и удаление подключений в Microsoft Graph](connecting-external-content-manage-connections.md).

## <a name="schema-api"></a>API схем

[Схема](/graph/api/resources/externalconnectors-schema?view=graph-rest-1.0&preserve-view=true) подключения определяет, как содержимое используется в различных возможностях Microsoft 365. Схема представляет собой простой список всех свойств, которые вы планируете добавить в соединение, вместе с их атрибутами, метками и псевдонимами. Перед добавлением элементов в Microsoft Graph вы должны зарегистрировать схему.

Подробнее см. в статье [Регистрация и обновление схемы для подключения Microsoft Graph](connecting-external-content-manage-schema.md).

## <a name="external-item-api"></a>API внешнего элемента

Элементы, добавленные приложением в службу "Поиск (Майкрософт)", представлены ресурсом [externalItem](/graph/api/resources/externalconnectors-externalitem?view=graph-rest-1.0&preserve-view=true) в Microsoft Graph.

Подробнее см. в статье [Создание, обновление и удаление элементов, добавленных вашим приложением с помощью соединителей Microsoft Graph](connecting-external-content-manage-items.md).

## <a name="external-group-api"></a>API внешней группы

Элементам во внешней службе может предоставляться или отказываться в доступе через ACL к различным типам групп, отличных от Azure Active Directory. Например, элементы Salesforce могут иметь наборы разрешений и профили, а элементы ServiceNow могут иметь локальные группы. При записи этих элементов в Microsoft Graph необходимо соблюдать эти ACL.

Вы можете использовать API внешней группы для установки разрешений для внешних элементов, загружаемых в Microsoft Graph. [externalGroup](/graph/api/resources/externalconnectors-externalgroup?view=graph-rest-1.0&preserve-view=true) представляет собой группу или подобную группе структуру, не относящуюся к Azure Active Directory (например, бизнес-подразделения, команды и т. д.), и определяет разрешения на содержимое во внешнем источнике данных.

Дополнительные сведения см. в статье [Использование внешних групп для управления разрешениями на доступ к источникам данных соединителей Microsoft Graph](connecting-external-content-external-groups.md).
