---
title: Тип ресурса Екстерналконнектион
description: Подключение к Microsoft Search из внешнего источника.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 4a77afc0aeef6c68d7bd58e554848068f25e1142
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40866842"
---
# <a name="externalconnection-resource-type"></a>Тип ресурса Екстерналконнектион

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Подключение к Microsoft Search из внешнего источника.

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a>Методы

| Метод                                                           | Возвращаемый тип                                   | Описание |
|:-----------------------------------------------------------------|:----------------------------------------------|:--|
| [Создание Екстерналконнектион](../api/external-post-connections.md) | externalConnection                            | Создание нового Екстерналконнектион путем публикации в коллекции Connections. |
| [Список Екстерналконнектионс](../api/externalconnection-list.md)    | Коллекция Екстерналконнектион                 | Получение коллекции объектов Екстерналконнектион. |
| [Получение Екстерналконнектион](../api/externalconnection-get.md)       | externalConnection                            | Чтение свойств и связей объекта Екстерналконнектион. |
| [Обновление Екстерналконнектион](../api/externalconnection-update.md) | externalConnection                            | Обновление объекта Екстерналконнектион. |
| [Удаление Екстерналконнектион](../api/externalconnection-delete.md) | Нет.                                          | Удаление объекта Екстерналконнектион. |
| [Создание схемы](../api/externalconnection-post-schema.md)        | Нет *или* [схема](schema.md)                 | Регистрация схемы подключения. |
| [Получение операции](../api/connectionoperation-get.md)               | [коннектионоператион](connectionoperation.md) | Получение состояния асинхронного запроса для создания схемы подключения. |
| [Создание Екстерналитем](../api/externalconnection-put-items.md)    | [externalItem](externalitem.md)               | Создание нового Екстерналитем путем публикации в коллекции Items. |

## <a name="properties"></a>Свойства

| Свойство      | Тип                              | Описание |
|:--------------|:----------------------------------|:------------|
| конфигурацион | [configuration](configuration.md) | Задает дополнительные идентификаторы приложений, которым разрешено управлять подключением и индексировать содержимое в подключении. Необязательный атрибут. |
| description   | String                            | Описание подключения, отображаемое в центре администрирования Microsoft 365. Необязательный атрибут. |
| id            | Строка                            | Предоставленный разработчиком уникальный идентификатор подключения в клиенте Azure Active Directory. Максимальная длина 32 символов. Должно содержать только буквенно-цифровые символы. `Microsoft` Не может начинаться с одного из следующих значений: `None`, `Directory`, `Exchange`, `ExchangeArchive` `LinkedIn` `Mailbox` `MicrosoftSearch` `OneDriveBusiness` `SharePoint` `Teams`,,,,,,, `Yammer`,. `Connectors` Обязательный атрибут. |
| name          | String                            | Отображаемое имя подключения, отображаемое в центре администрирования Microsoft 365. Максимальная длина 128 символов. Обязательный атрибут. |

## <a name="relationships"></a>Отношения

| Связь | Тип                                                     | Описание |
|:-------------|:---------------------------------------------------------|:---|
| items        | Коллекция [екстерналитем](externalitem.md)               | Только для чтения. Допускается значение null. |
| operations   | Коллекция [коннектионоператион](connectionoperation.md) | Только для чтения. Допускается значение null. |
| схемы       | [schema](schema.md)                                      | Только для чтения. Допускается значение null. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalConnection",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "configuration": {"@odata.type": "microsoft.graph.configuration"},
  "description": "String",
  "id": "String (identifier)",
  "name": "String"
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
