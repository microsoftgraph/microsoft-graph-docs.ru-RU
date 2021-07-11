---
title: тип ресурса externalConnection
description: Подключение является логическим контейнером для внешнего контента в Microsoft Graph
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 4b0c0a56fc415c4f2f75ec4972909e31fc9bea14
ms.sourcegitcommit: 3873c85f53e026073addca92d31d234af244444c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/10/2021
ms.locfileid: "53366571"
---
# <a name="externalconnection-resource-type"></a>тип ресурса externalConnection

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Логический контейнер для добавления контента из внешнего источника в Microsoft Graph.

## <a name="methods"></a>Методы

| Метод                                                           | Возвращаемый тип                                   | Описание |
|:-----------------------------------------------------------------|:----------------------------------------------|:--|
| [Создание externalConnection](../api/external-post-connections.md) | externalConnection                            | Создайте новую externalConnection, разместив в коллекции подключений. |
| [Список externalConnections](../api/externalconnection-list.md)    | коллекция externalConnection                 | Получите коллекцию объектов externalConnection. |
| [Get externalConnection](../api/externalconnection-get.md)       | externalConnection                            | Чтение свойств и связей объекта externalConnection. |
| [Обновление externalConnection](../api/externalconnection-update.md) | externalConnection                            | Обновление объекта externalConnection. |
| [Удаление externalConnection](../api/externalconnection-delete.md) | Нет                                          | Удаление объекта externalConnection. |
| [Создание схемы](../api/externalconnection-post-schema.md)        | Нет *или* [схемы](schema.md)                 | Схема подключения для регистрации. |
| [Получить операцию](../api/connectionoperation-get.md)               | [connectionOperation](connectionoperation.md) | Получите состояние асинхронного запроса для создания схемы подключения. |
| [Создание externalItem](../api/externalconnection-put-items.md)    | [externalItem](externalitem.md)               | Создайте новый externalItem, разместив в коллекции элементов. |

## <a name="properties"></a>Свойства

| Свойство      | Тип                              | Описание |
|:--------------|:----------------------------------|:------------|
| configuration | [configuration](configuration.md) | Указывает дополнительные ID-адреса приложений, которые разрешены для управления подключением и индексации контента в подключении. Необязательный параметр. |
| description   | String                            | Описание подключения, отображаемого в Центр администрирования Microsoft 365. Необязательный параметр. |
| id            | String                            | Уникальный ID подключения, предоставленный разработчиком в Azure Active Directory клиента. Максимальная длина — 32 символа. Должны содержаться только буквамерные символы. Не может начаться с или быть `Microsoft` одним из следующих значений: `None` , , , , , , `Directory` `Exchange` `ExchangeArchive` `LinkedIn` `Mailbox` `MicrosoftSearch` `OneDriveBusiness` `SharePoint` `Teams` `Yammer` `Connectors` . Обязательный. |
| name          | String                            | Отображает имя подключения, отображаемого в Центр администрирования Microsoft 365. Максимальная длина 128 символов. Обязательный. |
| state         | connectionState                   | Указывает текущее состояние подключения. Возможные значения `draft` , `ready` и `obsolete` `limitExceeded` . Обязательный. |

## <a name="relationships"></a>Связи

| Связь | Тип                                                     | Описание |
|:-------------|:---------------------------------------------------------|:---|
| items        | [коллекция externalItem](externalitem.md)               | Только для чтения. Допускается значение null. |
| operations   | [коллекция connectionOperation](connectionoperation.md) | Только для чтения. Допускается значение null. |
| схема       | [schema](schema.md)                                      | Только для чтения. Допускается значение null. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalConnection",
  "keyProperty": "id"
}-->

```json
{
  "configuration": {"@odata.type": "microsoft.graph.configuration"},
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
