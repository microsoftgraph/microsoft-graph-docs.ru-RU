---
title: Тип ресурса externalConnection
description: Подключение — это логический контейнер для внешнего контента в Microsoft Graph
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 4355ffe51fe1b160c7fb486272e85f2b2cf0bf2c
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161712"
---
# <a name="externalconnection-resource-type"></a>Тип ресурса externalConnection

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Логический контейнер для добавления контента из внешнего источника в Microsoft Graph.

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a>Методы

| Метод                                                           | Возвращаемый тип                                   | Описание |
|:-----------------------------------------------------------------|:----------------------------------------------|:--|
| [Создание externalConnection](../api/external-post-connections.md) | externalConnection                            | Создание внешнего подключения путем публикации в коллекции подключений. |
| [Список externalConnections](../api/externalconnection-list.md)    | коллекция externalConnection                 | Получить коллекцию объектов externalConnection. |
| [Get externalConnection](../api/externalconnection-get.md)       | externalConnection                            | Чтение свойств и связей объекта externalConnection. |
| [Обновление externalConnection](../api/externalconnection-update.md) | externalConnection                            | Обновление объекта externalConnection. |
| [Удаление externalConnection](../api/externalconnection-delete.md) | Нет                                          | Удаление объекта externalConnection. |
| [Создание схемы](../api/externalconnection-post-schema.md)        | Нет *или* [схема](schema.md)                 | Зарегистрируйте схему подключения. |
| [Получить операцию](../api/connectionoperation-get.md)               | [connectionOperation](connectionoperation.md) | Получите состояние асинхронного запроса для создания схемы подключения. |
| [Создание externalItem](../api/externalconnection-put-items.md)    | [externalItem](externalitem.md)               | Создание внешнегоitem путем публикации в коллекции элементов. |

## <a name="properties"></a>Свойства

| Свойство      | Тип                              | Описание |
|:--------------|:----------------------------------|:------------|
| configuration | [configuration](configuration.md) | Указывает дополнительные ИД приложений, которые разрешено использовать для управления подключением и индексации содержимого подключения. Необязательный параметр. |
| description   | String                            | Описание подключения, отображаемого в Центре администрирования Microsoft 365. Необязательный параметр. |
| id            | String                            | Уникальный ИД подключения в клиенте Azure Active Directory, предоставленный разработчиком. Максимальная длина — 32 символа. Должен содержать только буквы и цифры. Не может начинаться с одного из следующих `Microsoft` значений: `None` , , , , , , , , `Directory` , `Exchange` , `ExchangeArchive` `LinkedIn` `Mailbox` `MicrosoftSearch` `OneDriveBusiness` `SharePoint` `Teams` `Yammer` `Connectors` . Обязательно. |
| name          | String                            | Отображаемого имени подключения, отображаемого в Центре администрирования Microsoft 365. Максимальная длина — 128 символов. Обязательно. |
| state         | connectionState                   | Указывает текущее состояние подключения. Возможные значения: `draft` `ready` , , и `obsolete` `limitExceeded` . Обязательный. |

## <a name="relationships"></a>Связи

| Связь | Тип                                                     | Описание |
|:-------------|:---------------------------------------------------------|:---|
| items        | [коллекция externalItem](externalitem.md)               | Только для чтения. Допускается значение null. |
| operations   | [Коллекция connectionOperation](connectionoperation.md) | Только для чтения. Допускается значение null. |
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
