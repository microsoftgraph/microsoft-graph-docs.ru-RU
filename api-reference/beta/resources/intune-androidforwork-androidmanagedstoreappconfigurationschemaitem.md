---
title: Тип ресурса Андроидманажедстореаппконфигуратионсчемаитем
description: Один элемент конфигурации внутри настраиваемой схемы конфигурации приложения Android.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 964916f9f6a46cd8b276e304bfb341d6504db0d2
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31785820"
---
# <a name="androidmanagedstoreappconfigurationschemaitem-resource-type"></a>Тип ресурса Андроидманажедстореаппконфигуратионсчемаитем

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Один элемент конфигурации внутри настраиваемой схемы конфигурации приложения Android.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|schemaItemKey|String|Уникальный ключ, используемый приложением для определения элемента.|
|displayName|Строка|Понятное человеку имя.|
|description|String|Описание компонентов приложения, которыми управляет элемент.|
|defaultBoolValue|Boolean|Значение по умолчанию для элементов логического типа, если указано разработчиком приложения.|
|defaultIntValue|Int32|Значение по умолчанию для элементов целочисленного типа, если указано разработчиком приложения.|
|defaultStringValue|String|Значение по умолчанию для элементов строкового типа, если указано разработчиком приложения.|
|defaultStringArrayValue|Коллекция объектов string|Значение по умолчанию для элементов типа "массив строк", если указано разработчиком приложения.|
|dataType|[Андроидманажедстореаппконфигуратионсчемаитемдататипе](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitemdatatype.md)|Тип значения, который описывает этот элемент. Возможные значения: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.|
|selections|Коллекция объектов [keyValuePair](../resources/intune-shared-keyvaluepair.md)|Список понятных человеку пар имя-значение для допустимых значений, которые можно задать для этого элемента (только для элементов одиночного и множественного выбора).|

## <a name="relationships"></a>Отношения
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





