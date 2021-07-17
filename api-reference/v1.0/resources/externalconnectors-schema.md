---
title: Тип ресурса схемы
description: Схема подключения определяет, как содержимое, добавленное в подключение, будет использоваться в различных Graph microsoft.
author: mecampos
localization_priority: Normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: c0ca5e88d9d4ac7d7b63dea49f8ff4aace8cc348
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467461"
---
# <a name="schema-resource-type"></a>Тип ресурса схемы

Пространство имен: microsoft.graph.externalConnectors

Схема [подключения](externalconnectors-externalconnection.md) определяет, как внешний контент будет использоваться в различных Graph Microsoft. Схема — это плоский список всех свойств, которые вы планируете добавить в связь, а также их атрибуты, метки и псевдонимы. Перед добавлением элементов в связь вы должны зарегистрировать схему.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Создание схемы](../api/externalconnectors-schema-create.md)|[schema](../resources/externalconnectors-schema.md)|Создайте новый [объект схемы.](../resources/externalconnectors-schema.md)|
|[Получение схемы](../api/externalconnectors-schema-get.md)|[schema](../resources/externalconnectors-schema.md)|Ознакомьтесь с свойствами и отношениями объекта [схемы.](../resources/externalconnectors-schema.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|baseType|String|Необходимо указать значение `microsoft.graph.externalConnector.externalItem`. Обязательный элемент.|
|properties|[коллекция](../resources/externalconnectors-property.md) свойств|Свойства, определенные для элементов в подключении. Минимальное число свойств — одно, максимальное — 128.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.externalConnectors.schema",
  "openType": false
}
-->
``` json
{
  "baseType": "String",
  "properties": [
    {
      "name": "String",
      "type": "String",
    }
  ]
}
```

