---
title: тип ресурса externalConnection
description: Подключение является логическим контейнером для внешнего контента в Microsoft Graph
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 76fa391d1ce9937bc1799e9bc4ae9470c0794497
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467824"
---
# <a name="externalconnection-resource-type"></a>тип ресурса externalConnection

Пространство имен: microsoft.graph.externalConnectors

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Логический контейнер для добавления контента из внешнего источника в Microsoft Graph.

## <a name="methods"></a>Методы

| Метод                                                           | Возвращаемый тип                                   | Описание |
|:-----------------------------------------------------------------|:----------------------------------------------|:--|
| [Создание externalConnection](../api/externalconnectors-external-post-connections.md) | externalConnection                            | Создайте новую externalConnection, разместив в коллекции подключений. |
| [Список externalConnections](../api/externalconnectors-externalconnection-list.md)    | коллекция externalConnection                 | Получите коллекцию объектов externalConnection. |
| [Get externalConnection](../api/externalconnectors-externalconnection-get.md)       | externalConnection                            | Чтение свойств и связей объекта externalConnection. |
| [Обновление externalConnection](../api/externalconnectors-externalconnection-update.md) | externalConnection                            | Обновление объекта externalConnection. |
| [Удаление externalConnection](../api/externalconnectors-externalconnection-delete.md) | Нет                                          | Удаление объекта externalConnection. |
| [Создание схемы](../api/externalconnectors-externalconnection-post-schema.md)        | Нет *или* [схемы](externalconnectors-schema.md)                 | Схема подключения для регистрации. |
| [Получить операцию](../api/externalconnectors-connectionoperation-get.md)               | [connectionOperation](externalconnectors-connectionoperation.md) | Получите состояние асинхронного запроса для создания схемы подключения. |
| [Создание externalItem](../api/externalconnectors-externalconnection-put-items.md)    | [externalItem](externalconnectors-externalitem.md)               | Создайте новый externalItem, разместив в коллекции элементов. |

## <a name="properties"></a>Свойства

| Свойство      | Тип                              | Описание |
|:--------------|:----------------------------------|:------------|
| configuration | [microsoft.graph.externalConnectors.configuration](externalconnectors-configuration.md) | Указывает дополнительные ID-адреса приложений, которые разрешены для управления подключением и индексации контента в подключении. Необязательное. |
| description   | String                            | Описание подключения, отображаемого в Центр администрирования Microsoft 365. Необязательное. |
| id            | String                            | Уникальный ID подключения, предоставленный разработчиком в Azure Active Directory клиента. Длина должна быть от 3 до 32 символов. Должны содержаться только буквамерные символы. Не может `Microsoft` начаться или быть одним из следующих значений: `None` , , , , , `Directory` `Exchange` `ExchangeArchive` `LinkedIn` `Mailbox` `OneDriveBusiness` `SharePoint` `Teams` `Yammer` `Connectors` `TaskFabric` `PowerBI` `Assistant` `TopicEngine` `MSFT_All_Connectors` . Обязательный элемент. |
| name          | String                            | Отображает имя подключения, отображаемого в Центр администрирования Microsoft 365. Максимальная длина 128 символов. Обязательный элемент. |
| state         | microsoft.graph.externalConnectors.connectionState                   | Указывает текущее состояние подключения. Возможные значения `draft` , `ready` и `obsolete` `limitExceeded` . Обязательный. |

## <a name="relationships"></a>Связи

| Связь | Тип                                                     | Описание |
|:-------------|:---------------------------------------------------------|:---|
| items        | [коллекция microsoft.graph.externalConnectors.externalItem](externalconnectors-externalitem.md)               | Только для чтения. Допускается значение null. |
| operations   | [коллекция microsoft.graph.externalConnectors.connectionOperation](externalconnectors-connectionoperation.md) | Только для чтения. Допускается значение null. |
| schema       | [microsoft.graph.externalConnectors.schema](externalconnectors-schema.md)                                      | Только для чтения. Допускается значение null. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalConnectors.externalConnection",
  "keyProperty": "id"
}-->

```json
{
  "description": "String",
  "id": "String (identifier)",
  "name": "String",
  "state": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "connection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
