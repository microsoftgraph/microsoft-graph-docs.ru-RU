---
title: Тип ресурса схемы
description: Схема подключения определяет, как содержимое, добавленное в подключение, будет использоваться в различных Graph microsoft.
author: mecampos
ms.localizationpriority: medium
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 3e7c214b3f5151a13a93dd1a200f13dffe13f8b3
ms.sourcegitcommit: 64d27a0e3dcccc9d857e62aace4153e5d98fb3d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60730524"
---
# <a name="schema-resource-type"></a>Тип ресурса схемы

Пространство имен: microsoft.graph.externalConnectors

Схема [подключения](externalconnectors-externalconnection.md) определяет, как внешний контент будет использоваться в различных Graph Microsoft. Схема — это плоский список всех свойств, которые вы планируете добавить в соединение, а также их атрибуты, метки и псевдонимы. Перед добавлением элементов в соединение вы должны зарегистрировать схему.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Создание схемы](../api/externalconnectors-schema-create.md)|[schema](../resources/externalconnectors-schema.md)|Создайте новый [объект схемы.](../resources/externalconnectors-schema.md)|
|[Получение схемы](../api/externalconnectors-schema-get.md)|[schema](../resources/externalconnectors-schema.md)|Ознакомьтесь с свойствами и отношениями объекта [схемы.](../resources/externalconnectors-schema.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|baseType|String|Необходимо указать значение `microsoft.graph.externalConnector.externalItem`. Обязательный.|
|properties|[коллекция](../resources/externalconnectors-property.md) свойств|Свойства, определенные для элементов в подключении. Минимальное число свойств — одно, максимальное — 128.|

## <a name="relationships"></a>Отношения
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
      "type": "String"
    }
  ]
}
```

