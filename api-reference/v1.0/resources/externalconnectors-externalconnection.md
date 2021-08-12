---
title: тип ресурса externalConnection
description: Подключение является логическим контейнером для внешнего контента в Microsoft Graph
author: mecampos
localization_priority: Normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: beb0a9b424f1207a7cf378e6bbb17c747ca68ca50617381766ee4dc8d5232828
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54180861"
---
# <a name="externalconnection-resource-type"></a>тип ресурса externalConnection

Пространство имен: microsoft.graph.externalConnectors

Логический контейнер для добавления контента из внешнего источника в Microsoft Graph.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Создание externalConnection](../api/externalconnectors-external-post-connections.md)|[externalConnection](../resources/externalconnectors-externalconnection.md)|Создайте новый [объект externalConnection.](../resources/externalconnectors-externalconnection.md)|
|[Список externalConnections](../api/externalconnectors-externalconnection-list.md)|[коллекция externalConnection](../resources/externalconnectors-externalconnection.md)|Получите список объектов [externalConnection](../resources/externalconnectors-externalconnection.md) и их свойств.|
|[Get externalConnection](../api/externalconnectors-externalconnection-get.md)|[externalConnection](../resources/externalconnectors-externalconnection.md)|Ознакомьтесь с свойствами и отношениями [объекта externalConnection.](../resources/externalconnectors-externalconnection.md)|
|[Обновление externalConnection](../api/externalconnectors-externalconnection-update.md)|[externalConnection](../resources/externalconnectors-externalconnection.md)|Обновление свойств объекта [externalConnection.](../resources/externalconnectors-externalconnection.md)|
|[Удаление externalConnection](../api/externalconnectors-externalconnection-delete.md)|Нет|Удаляет объект [externalConnection.](../resources/externalconnectors-externalconnection.md)|
|[Создание схемы](../api/externalconnectors-schema-create.md)|[schema](../resources/externalconnectors-schema.md)|Создайте новый объект схемы.|
|[Создание externalItem](../api/externalconnectors-externalitem-create.md)|[externalItem](../resources/externalconnectors-externalitem.md)|Создайте новый объект externalItem.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|configuration|[microsoft.graph.externalConnectors.configuration](../resources/externalconnectors-configuration.md)|Указывает дополнительные ID-адреса приложений, которые разрешены для управления подключением и индексации контента в подключении. Необязательно.|
|description|String|Описание подключения, отображаемого в Центр администрирования Microsoft 365. Необязательно.|
|id|String| Уникальный ID подключения, предоставленный разработчиком в Azure Active Directory клиента. Длина должна быть от 3 до 32 символов. Должны содержаться только буквамерные символы. Не может `Microsoft` начаться или быть одним из следующих значений: `None` , , , , , `Directory` `Exchange` `ExchangeArchive` `LinkedIn` `Mailbox` `OneDriveBusiness` `SharePoint` `Teams` `Yammer` `Connectors` `TaskFabric` `PowerBI` `Assistant` `TopicEngine` `MSFT_All_Connectors` . Обязательный элемент. |
|name|String|Отображает имя подключения, отображаемого в Центр администрирования Microsoft 365. Максимальная длина 128 символов. Обязательный элемент.|
|state|microsoft.graph.externalConnectors.connectionState|Указывает текущее состояние подключения. Возможные значения: `draft`, `ready`, `obsolete`, `limitExceeded`, `unknownFutureValue`.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|items|[коллекция microsoft.graph.externalConnectors.externalItem](../resources/externalconnectors-externalitem.md)|Только для чтения. Допускается значение null.|
|operations|[коллекция microsoft.graph.externalConnectors.connectionOperation](../resources/externalconnectors-connectionoperation.md)|Только для чтения. Допускается значение null.|
|schema|[microsoft.graph.externalConnectors.schema](../resources/externalconnectors-schema.md)|Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.externalConnectors.externalConnection",
  "openType": false
}
-->
``` json
{
  "id": "String (identifier)",
  "name": "String",
  "description": "String",
  "state": "String"
}
```

