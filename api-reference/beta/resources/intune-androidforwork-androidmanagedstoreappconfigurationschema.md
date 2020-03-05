---
title: Тип ресурса Андроидманажедстореаппконфигуратионсчема
description: Схема, описывающая настраиваемые конфигурации приложения Android.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4c54ba00a2756950c1e4cecbb6e61e7458427d58
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42494613"
---
# <a name="androidmanagedstoreappconfigurationschema-resource-type"></a>Тип ресурса Андроидманажедстореаппконфигуратионсчема

Пространство имен: Microsoft. Graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Схема, описывающая настраиваемые конфигурации приложения Android.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Андроидманажедстореаппконфигуратионсчемас](../api/intune-androidforwork-androidmanagedstoreappconfigurationschema-list.md)|Коллекция [андроидманажедстореаппконфигуратионсчема](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)|Список свойств и связей объектов [андроидманажедстореаппконфигуратионсчема](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) .|
|[Получение Андроидманажедстореаппконфигуратионсчема](../api/intune-androidforwork-androidmanagedstoreappconfigurationschema-get.md)|[androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md);|Чтение свойств и связей объекта [андроидманажедстореаппконфигуратионсчема](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) .|
|[Создание Андроидманажедстореаппконфигуратионсчема](../api/intune-androidforwork-androidmanagedstoreappconfigurationschema-create.md)|[androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md);|Создание нового объекта [андроидманажедстореаппконфигуратионсчема](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) .|
|[Удаление Андроидманажедстореаппконфигуратионсчема](../api/intune-androidforwork-androidmanagedstoreappconfigurationschema-delete.md)|Нет|Удаляет объект [андроидманажедстореаппконфигуратионсчема](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md).|
|[Обновление Андроидманажедстореаппконфигуратионсчема](../api/intune-androidforwork-androidmanagedstoreappconfigurationschema-update.md)|[androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md);|Обновление свойств объекта [андроидманажедстореаппконфигуратионсчема](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта, которому соответствует имя пакета Android для схемы приложений.|
|exampleJson|Binary|Массив байтов в кодировке UTF8, содержащий образец соответствующей схеме строки JSON, который иллюстрирует настройку приложения.|
|schemaItems|Коллекция [андроидманажедстореаппконфигуратионсчемаитем](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitem.md)|Коллекция элементов, каждый из которых представляет именованный параметр конфигурации в схеме. Он содержит только конфигурацию корневого уровня.|
|нестедсчемаитемс|Коллекция [андроидманажедстореаппконфигуратионсчемаитем](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitem.md)|Коллекция элементов, каждый из которых представляет именованный параметр конфигурации в схеме. Он содержит плоский список всех конфигураций.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidManagedStoreAppConfigurationSchema"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidManagedStoreAppConfigurationSchema",
  "id": "String (identifier)",
  "exampleJson": "binary",
  "schemaItems": [
    {
      "@odata.type": "microsoft.graph.androidManagedStoreAppConfigurationSchemaItem",
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
  ],
  "nestedSchemaItems": [
    {
      "@odata.type": "microsoft.graph.androidManagedStoreAppConfigurationSchemaItem",
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
  ]
}
```



