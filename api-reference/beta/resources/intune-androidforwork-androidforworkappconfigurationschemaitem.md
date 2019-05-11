---
title: Тип ресурса androidForWorkAppConfigurationSchemaItem
description: Один элемент конфигурации в схеме настраиваемой конфигурации Android for Work.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3313ba3cef3a996d030d25ac1bb24492b28b4b2a
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33950776"
---
# <a name="androidforworkappconfigurationschemaitem-resource-type"></a>Тип ресурса androidForWorkAppConfigurationSchemaItem

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Один элемент конфигурации в схеме настраиваемой конфигурации Android for Work.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|schemaItemKey|Строка|Уникальный ключ, используемый приложением для определения элемента.|
|displayName|Строка|Понятное человеку имя.|
|description|String|Описание компонентов приложения, которыми управляет элемент.|
|defaultBoolValue|Boolean|Значение по умолчанию для элементов логического типа, если указано разработчиком приложения.|
|defaultIntValue|Int32|Значение по умолчанию для элементов целочисленного типа, если указано разработчиком приложения.|
|defaultStringValue|String|Значение по умолчанию для элементов строкового типа, если указано разработчиком приложения.|
|defaultStringArrayValue|Коллекция объектов string|Значение по умолчанию для элементов типа "массив строк", если указано разработчиком приложения.|
|dataType|[Андроидфорворкаппконфигуратионсчемаитемдататипе](../resources/intune-androidforwork-androidforworkappconfigurationschemaitemdatatype.md)|Тип значения, который описывает этот элемент. Возможные значения: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.|
|selections|Коллекция объектов [keyValuePair](../resources/intune-shared-keyvaluepair.md)|Список понятных человеку пар имя-значение для допустимых значений, которые можно задать для этого элемента (только для элементов одиночного и множественного выбора).|

## <a name="relationships"></a>Связи
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




