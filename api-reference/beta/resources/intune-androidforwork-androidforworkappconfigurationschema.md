---
title: Тип ресурса androidForWorkAppConfigurationSchema
description: Схема, описывающая пользовательские конфигурации приложения Android for Work.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 645cdf0440bfbeefbfed239c5dcb2c8e0a2ff057
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006194"
---
# <a name="androidforworkappconfigurationschema-resource-type"></a>Тип ресурса androidForWorkAppConfigurationSchema

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Схема, описывающая пользовательские конфигурации приложения Android for Work.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов androidForWorkAppConfigurationSchema](../api/intune-androidforwork-androidforworkappconfigurationschema-list.md)|Коллекция [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md)|Список свойств и связей объектов [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md).|
|[Получение объекта androidForWorkAppConfigurationSchema](../api/intune-androidforwork-androidforworkappconfigurationschema-get.md)|[androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md);|Чтение свойств и связей объекта [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md).|
|[Создание объекта androidForWorkAppConfigurationSchema](../api/intune-androidforwork-androidforworkappconfigurationschema-create.md)|[androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md);|Создание объекта [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md).|
|[Удаление объекта androidForWorkAppConfigurationSchema](../api/intune-androidforwork-androidforworkappconfigurationschema-delete.md)|Нет|Удаляет объект [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md).|
|[Обновление объекта androidForWorkAppConfigurationSchema](../api/intune-androidforwork-androidforworkappconfigurationschema-update.md)|[androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md)|Обновление свойств объекта [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта, которому соответствует имя пакета Android для схемы приложений.|
|exampleJson|Binary|Массив байтов в кодировке UTF8, содержащий образец соответствующей схеме строки JSON, который иллюстрирует настройку приложения.|
|schemaItems|Коллекция [androidForWorkAppConfigurationSchemaItem](../resources/intune-androidforwork-androidforworkappconfigurationschemaitem.md)|Коллекция элементов, каждый из которых представляет именованный параметр конфигурации в схеме|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidForWorkAppConfigurationSchema"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidForWorkAppConfigurationSchema",
  "id": "String (identifier)",
  "exampleJson": "binary",
  "schemaItems": [
    {
      "@odata.type": "microsoft.graph.androidForWorkAppConfigurationSchemaItem",
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





