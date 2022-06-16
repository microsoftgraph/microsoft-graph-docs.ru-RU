---
title: Работа с API соединителей Microsoft Graph
description: Используйте API соединителей Microsoft Graph для создания настраиваемых соединителей, которые переносят внешние данные в Microsoft Graph с целью улучшения интеллектуальных возможностей Microsoft 365.
author: mecampos
ms.localizationpriority: high
doc_type: conceptualPageType
ms.prod: search
ms.openlocfilehash: 4c2359f7e565b9d1ff00e623649e833363fc6231
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/15/2022
ms.locfileid: "66094419"
---
# <a name="work-with-the-microsoft-graph-connectors-api"></a>Работа с API соединителей Microsoft Graph

Соединители Microsoft Graph добавляют внешние данные в Microsoft Graph и улучшают интеллектуальные возможности Microsoft 365. Для интеграции со службами, которые недоступны в роли соединителей, созданных корпорацией Майкрософт, необходимо создать настраиваемый соединитель. Для создания настраиваемых соединителей вы используете REST API соединителей Microsoft Graph.

![Изображение внешних данных, исходящих из разных соединителей Microsoft Graph](./images/connectors-images/api-overview.png)

Используйте API Microsoft Graph, чтобы выполнять следующие задачи:

1. Создание подключений к внешним данным и управление ими.
2. Определите и зарегистрируйте схему внешних типов данных.
3. Запись элементов внешних данных в Microsoft Graph.
4. Синхронизация внешних групп.

## <a name="create-and-manage-external-data-connections"></a>Создание подключений к внешним данным и управление ими

Ресурс [externalConnection](/graph/api/resources/externalconnectors-externalconnection) (API внешнего подключения) — это логический контейнер для внешних данных, которым вы можете управлять как единым блоком.

Подробнее см. в статье [Создание, обновление и удаление подключений в Microsoft Graph](connecting-external-content-manage-connections.md).

## <a name="define-and-register-the-schema-of-the-external-data-types"></a>Определение и регистрация схем внешних типов данных

Подключение [schema](/graph/api/resources/externalconnectors-schema) (API схемы) определяет, как содержимое используется в различных возможностях Microsoft 365. Схема представляет собой простой список всех свойств, которые вы планируете добавить в соединение, вместе с их атрибутами, метками и псевдонимами. Перед добавлением элементов в Microsoft Graph вы должны зарегистрировать схему.

Подробнее см. в статье [Регистрация и обновление схемы для подключения Microsoft Graph](connecting-external-content-manage-schema.md).

## <a name="ingest-external-data-items-into-microsoft-graph"></a>Запись элементов внешних данных в Microsoft Graph

Элементы, добавленные приложением в службу "Поиск (Майкрософт)", представлены ресурсом [externalItem](/graph/api/resources/externalconnectors-externalitem) (API внешнего элемента) в Microsoft Graph.

Подробнее см. в статье [Создание, обновление и удаление элементов, добавленных вашим приложением с помощью соединителей Microsoft Graph](connecting-external-content-manage-items.md).

## <a name="sync-external-groups"></a>Синхронизация внешних групп

Элементам во внешней службе может предоставляться или отказываться в доступе через ACL к различным типам групп, отличных от Azure Active Directory. Например, элементы Salesforce могут иметь наборы разрешений и профили, а элементы ServiceNow могут иметь локальные группы. При записи этих элементов в Microsoft Graph необходимо соблюдать эти ACL.

Вы можете использовать API внешней группы для установки разрешений для внешних элементов, загружаемых в Microsoft Graph. [externalGroup](/graph/api/resources/externalconnectors-externalgroup) представляет собой группу или подобную группе структуру, не относящуюся к Azure Active Directory (например, бизнес-подразделения, команды и т. д.), и определяет разрешения на содержимое во внешнем источнике данных.

Дополнительные сведения см. в статье [Использование внешних групп для управления разрешениями на доступ к источникам данных соединителей Microsoft Graph](connecting-external-content-external-groups.md).

## <a name="next-steps"></a>Дальнейшие действия

- [Создание пользовательского соединителя](/graph/connecting-external-content-build-quickstart)