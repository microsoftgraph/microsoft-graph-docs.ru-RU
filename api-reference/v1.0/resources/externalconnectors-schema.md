---
title: Тип ресурса схемы
description: Схема подключения определяет, как содержимое, добавленное в подключение, будет использоваться в различных Graph microsoft.
author: mecampos
ms.localizationpriority: medium
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: dcfea02e76c97a8bd946a3c1aa5294b843b0b739
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59036587"
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
|baseType|Строка|Необходимо указать значение `microsoft.graph.externalConnector.externalItem`. Обязательный.|
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

