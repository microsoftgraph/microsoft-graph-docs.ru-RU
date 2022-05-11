---
title: Тип ресурса externalConnection
description: Подключение — это логический контейнер для внешнего содержимого в Microsoft Graph
ms.localizationpriority: medium
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 417af041fc70ce86e921568b60059948754b942f
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65315701"
---
# <a name="externalconnection-resource-type"></a>Тип ресурса externalConnection

Пространство имен: microsoft.graph.externalConnectors

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Логический контейнер для добавления содержимого из внешнего источника в Microsoft Graph.

## <a name="methods"></a>Методы

| Метод                                                           | Возвращаемый тип                                   | Описание |
|:-----------------------------------------------------------------|:----------------------------------------------|:--|
| [Создание externalConnection](../api/externalconnectors-external-post-connections.md) | externalConnection                            | Создайте **внешнее подключение,** выполнив публикацию в коллекции подключений. |
| [Перечисление внешних подключений](../api/externalconnectors-externalconnection-list.md)    | Коллекция externalConnection                 | Получение коллекции **объектов externalConnection** . |
| [Получение внешнего подключения](../api/externalconnectors-externalconnection-get.md)       | externalConnection                            | Чтение свойств и связей объекта **externalConnection** . |
| [Обновление externalConnection](../api/externalconnectors-externalconnection-update.md) | externalConnection                            | Обновление объекта **externalConnection** . |
| [Удаление externalConnection](../api/externalconnectors-externalconnection-delete.md) | Нет                                          | Удаление объекта **externalConnection** . |
| [Создание схемы](../api/externalconnectors-externalconnection-post-schema.md)        | Нет *или* [схема](externalconnectors-schema.md)                 | Зарегистрируйте схему подключения. |
| [Операция Get](../api/externalconnectors-connectionoperation-get.md)               | [connectionOperation](externalconnectors-connectionoperation.md) | Получение состояния асинхронного запроса для создания схемы подключения. |
| [Создание externalItem](../api/externalconnectors-externalconnection-put-items.md)    | [externalItem](externalconnectors-externalitem.md)               | Создайте новый externalItem, выполнив публикацию в коллекции элементов. |
|[Получение connectionQuota](../api/externalconnectors-connectionquota-get.md)|[connectionQuota](../resources/externalconnectors-connectionquota.md)| Получение свойств и связей **connectionQuota**. |

## <a name="properties"></a>Свойства

| Свойство      | Тип                              | Описание |
|:--------------|:----------------------------------|:------------|
| configuration | [microsoft.graph.externalConnectors.configuration](externalconnectors-configuration.md) | Указывает дополнительные идентификаторы приложений, которым разрешено управлять подключением и индексировать содержимое в соединении. Необязательное. |
| connectorId   |String                             | Идентификатор Teams приложения. Необязательное.|
| description   | String                            | Описание подключения, отображаемого в Центр администрирования Microsoft 365. Необязательное. |
| id            | String                            | Предоставленный разработчиком уникальный идентификатор подключения в Azure Active Directory клиента. Длина должна быть от 3 до 32 символов. Должен содержать только буквенно-цифровые символы. Не может начинаться `Microsoft` с одного из следующих значений: `None`, `Directory`, `Exchange`, , `ExchangeArchive`, `LinkedIn`, `Mailbox`, `OneDriveBusiness`, `Teams``SharePoint`, `Yammer`, `Connectors`, `TaskFabric`, `PowerBI`, , `Assistant`, , `TopicEngine``MSFT_All_Connectors`. Обязательно. |
| ingestedItemsCount           | Int64                            |  Количество элементов, принимаемых в соединение. Это значение обновляется каждые 15 минут. Если состояние подключения равно `draft`, **то параметр ingestedItemsCount** будет иметь значение `null`. |
| name          | String                            | Отображаемое имя подключения, отображаемое в Центр администрирования Microsoft 365. Максимальная длина — 128 символов. Обязательно. |
| searchSettings|[microsoft.graph.externalConnectors.searchSettings](../resources/externalconnectors-searchsettings.md)|Параметры, настраиваемые для поиска содержимого в этом соединении, например шаблоны отображения результатов поиска.|
| state         | microsoft.graph.externalConnectors.connectionState                   | Указывает текущее состояние соединения. Возможные значения: `draft`, `ready`и `obsolete``limitExceeded`. Обязательный. |

## <a name="relationships"></a>Связи

| Связь | Тип                                                     | Описание |
|:-------------|:---------------------------------------------------------|:---|
| groups       | [Коллекция microsoft.graph.externalConnectors.externalGroup](externalconnectors-externalgroup.md)             | Только для чтения. Допускается значение null. |
| items        | [Коллекция microsoft.graph.externalConnectors.externalItem](externalconnectors-externalitem.md)               | Только для чтения. Допускается значение null. |
| operations   | [Коллекция microsoft.graph.externalConnectors.connectionOperation](externalconnectors-connectionoperation.md) | Только для чтения. Допускается значение null. |
| quota        | [microsoft.graph.externalConnectors.connectionQuota](externalconnectors-connectionquota.md)             | Только для чтения. Допускается значение null. |
| Схемы       | [microsoft.graph.externalConnectors.schema](externalconnectors-schema.md)                                      | Только для чтения. Допускается значение null. |

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
  "ingestedItemsCount": "Int64",
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
