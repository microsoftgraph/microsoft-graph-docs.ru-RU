---
title: тип ресурса androidManagedStoreAppConfigurationSchemaItem
description: Элемент единой конфигурации в пользовательской схеме конфигурации android-приложения.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e40612aa0486f6aeaa6c28394cc3bea338dbc66d
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58801208"
---
# <a name="androidmanagedstoreappconfigurationschemaitem-resource-type"></a>тип ресурса androidManagedStoreAppConfigurationSchemaItem

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Элемент единой конфигурации в пользовательской схеме конфигурации android-приложения.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|index|Int32|Уникальный индекс, который приложение использует для поддержания вложенных элементов схемы|
|parentIndex|Int32|Индекс родительской схемы элемента для отслеживания вложенных элементов схемы|
|schemaItemKey|String|Уникальный ключ, используемый приложением для определения элемента.|
|displayName|Строка|Понятное человеку имя.|
|description|Строка|Описание компонентов приложения, которыми управляет элемент.|
|defaultBoolValue|Boolean|Значение по умолчанию для элементов логического типа, если указано разработчиком приложения.|
|defaultIntValue|Int32|Значение по умолчанию для элементов целочисленного типа, если указано разработчиком приложения.|
|defaultStringValue|String|Значение по умолчанию для элементов строкового типа, если указано разработчиком приложения.|
|defaultStringArrayValue|Коллекция объектов string|Значение по умолчанию для элементов типа "массив строк", если указано разработчиком приложения.|
|dataType|[AndroidManagedStoreAppConfigurationSchemaItemDataType](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitemdatatype.md)|Тип значения, описанного в этом элементе. Возможные значения: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.|
|selections|Коллекция объектов [keyValuePair](../resources/intune-androidforwork-keyvaluepair.md)|Список понятных человеку пар имя-значение для допустимых значений, которые можно задать для этого элемента (только для элементов одиночного и множественного выбора).|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidManagedStoreAppConfigurationSchemaItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidManagedStoreAppConfigurationSchemaItem",
  "index": 1024,
  "parentIndex": 1024,
  "schemaItemKey": "String",
  "displayName": "String",
  "description": "String",
  "defaultBoolValue": true,
  "defaultIntValue": 1024,
  "defaultStringValue": "String",
  "defaultStringArrayValue": [
    "String"
  ],
  "dataType": "String",
  "selections": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ]
}
```



