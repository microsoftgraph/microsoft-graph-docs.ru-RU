---
title: тип ресурса externalConnection
description: Подключение является логическим контейнером для внешнего контента в Microsoft Graph
ms.localizationpriority: medium
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: f7eeddc207206e6bcfcd526e8ac3e2cd00d481b3
ms.sourcegitcommit: 2a9b82dae63d8a998711679a379ae1fa89df80e0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/06/2021
ms.locfileid: "60214741"
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
| configuration | [microsoft.graph.externalConnectors.configuration](externalconnectors-configuration.md) | Указывает дополнительные ID-адреса приложений, которые разрешены для управления подключением и индексации контента в подключении. Необязательный параметр. |
| connectorId   |String                             | ID Teams app. Необязательный параметр.|
| description   | Строка                            | Описание подключения, отображаемого в Центр администрирования Microsoft 365. Необязательный параметр. |
| id            | String                            | Уникальный ID подключения, предоставленный разработчиком в Azure Active Directory клиента. Длина должна быть от 3 до 32 символов. Должны содержаться только буквамерные символы. Не может `Microsoft` начаться или быть одним из следующих значений: `None` , , , , , `Directory` `Exchange` `ExchangeArchive` `LinkedIn` `Mailbox` `OneDriveBusiness` `SharePoint` `Teams` `Yammer` `Connectors` `TaskFabric` `PowerBI` `Assistant` `TopicEngine` `MSFT_All_Connectors` . Обязательно. |
| name          | String                            | Отображает имя подключения, отображаемого в Центр администрирования Microsoft 365. Максимальная длина 128 символов. Обязательно. |
| searchSettings|[microsoft.graph.externalConnectors.searchSettings](../resources/externalconnectors-searchsettings.md)|Параметры, настраивающие опытом поиска контента в этом подключении, например шаблоны отображения результатов поиска.|
| state         | microsoft.graph.externalConnectors.connectionState                   | Указывает текущее состояние подключения. Возможные значения `draft` , `ready` и `obsolete` `limitExceeded` . Обязательный. |

## <a name="relationships"></a>Связи

| Связь | Тип                                                     | Описание |
|:-------------|:---------------------------------------------------------|:---|
| items        | [коллекция microsoft.graph.externalConnectors.externalItem](externalconnectors-externalitem.md)               | Только для чтения. Допускается значение null. |
| operations   | [коллекция microsoft.graph.externalConnectors.connectionOperation](externalconnectors-connectionoperation.md) | Только для чтения. Допускается значение null. |
| схема       | [microsoft.graph.externalConnectors.schema](externalconnectors-schema.md)                                      | Только для чтения. Допускается значение null. |
| groups       | [коллекция microsoft.graph.externalConnectors.externalGroup](externalconnectors-externalgroup.md)             | Только для чтения. Допускается значение null. |

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
