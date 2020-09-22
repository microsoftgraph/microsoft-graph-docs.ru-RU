---
title: Тип ресурса androidForWorkAppConfigurationSchemaItem
description: Один элемент конфигурации в схеме настраиваемой конфигурации Android for Work.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 13af3b581498a4285773b2fda02d5596127c3012
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48019672"
---
# <a name="androidforworkappconfigurationschemaitem-resource-type"></a>Тип ресурса androidForWorkAppConfigurationSchemaItem

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Один элемент конфигурации в схеме настраиваемой конфигурации Android for Work.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|schemaItemKey|String|Уникальный ключ, используемый приложением для определения элемента.|
|displayName|String|Понятное человеку имя.|
|description|String|Описание компонентов приложения, которыми управляет элемент.|
|defaultBoolValue|Boolean|Значение по умолчанию для элементов логического типа, если указано разработчиком приложения.|
|defaultIntValue|Int32|Значение по умолчанию для элементов целочисленного типа, если указано разработчиком приложения.|
|defaultStringValue|String|Значение по умолчанию для элементов строкового типа, если указано разработчиком приложения.|
|defaultStringArrayValue|Коллекция объектов string|Значение по умолчанию для элементов типа "массив строк", если указано разработчиком приложения.|
|dataType|[андроидфорворкаппконфигуратионсчемаитемдататипе](../resources/intune-androidforwork-androidforworkappconfigurationschemaitemdatatype.md)|Тип значения, который описывает этот элемент. Возможные значения: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.|
|selections|Коллекция объектов [keyValuePair](../resources/intune-shared-keyvaluepair.md)|Список понятных человеку пар имя-значение для допустимых значений, которые можно задать для этого элемента (только для элементов одиночного и множественного выбора).|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidForWorkAppConfigurationSchemaItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidForWorkAppConfigurationSchemaItem",
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






