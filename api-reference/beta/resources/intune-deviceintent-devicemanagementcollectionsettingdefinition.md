---
title: тип ресурса deviceManagementCollectionSettingDefinition
description: Объект, представляющий дефиенции для параметра коллекции
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6edd80c21d336c43e67e0e509d24cc03a590d16e
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59138010"
---
# <a name="devicemanagementcollectionsettingdefinition-resource-type"></a>тип ресурса deviceManagementCollectionSettingDefinition

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект, представляющий дефиенции для параметра коллекции


Наследует [от deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список deviceManagementCollectionSettingDefinitions](../api/intune-deviceintent-devicemanagementcollectionsettingdefinition-list.md)|[коллекция deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md)|Список свойств и связей [объектов deviceManagementCollectionSettingDefinition.](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md)|
|[Get deviceManagementCollectionSettingDefinition](../api/intune-deviceintent-devicemanagementcollectionsettingdefinition-get.md)|[deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md)|Чтение свойств и связей [объекта deviceManagementCollectionSettingDefinition.](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md)|
|[Создание deviceManagementCollectionSettingDefinition](../api/intune-deviceintent-devicemanagementcollectionsettingdefinition-create.md)|[deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md)|Создайте новый [объект deviceManagementCollectionSettingDefinition.](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md)|
|[Удаление deviceManagementCollectionSettingDefinition](../api/intune-deviceintent-devicemanagementcollectionsettingdefinition-delete.md)|Нет|Удаляет [устройствоManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md).|
|[Обновление deviceManagementCollectionSettingDefinition](../api/intune-deviceintent-devicemanagementcollectionsettingdefinition-update.md)|[deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md)|Обновление свойств объекта [deviceManagementCollectionSettingDefinition.](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|ID определения параметра, унаследованный от [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)|
|valueType|[deviceManangementIntentValueType](../resources/intune-deviceintent-devicemanangementintentvaluetype.md)|Тип данных значения, унаследованный от [deviceManagementSettingDefinition.](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) Возможные значения: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.|
|displayName|String|Имя отображения параметра, унаследованный от [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)|
|isTopLevel|Логический|Если параметр верхнего уровня, его можно настроить без необходимости завернутой в коллекцию или сложный параметр, унаследованный от [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)|
|description|String|Описание параметра Унаследовано от [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)|
|placeholderText|String|Текст placeholder в качестве примера допустимого ввода, наследуемого [из deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)|
|documentationUrl|String|URL-адрес для настройки документации, унаследованной от [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)|
|headerTitle|String|заголовок параметра представляет категорию/раздел параметра/параметров, унаследованных от [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)|
|headerSubtitle|String|субтитры заголовок параметра для получения дополнительных сведений о категории/разделе, унаследованной от [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)|
|keywords|Коллекция объектов string|Ключевые слова, связанные с параметром Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)|
|ограничения|[коллекция deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)|Коллекция ограничений для значения параметра Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)|
|зависимости|[коллекция deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md)|Коллекция зависимостей от других параметров, унаследованных от [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)|
|elementDefinitionId|String|The Setting Definition ID that describes what each element of the collection looks like|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementCollectionSettingDefinition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementCollectionSettingDefinition",
  "id": "String (identifier)",
  "valueType": "String",
  "displayName": "String",
  "isTopLevel": true,
  "description": "String",
  "placeholderText": "String",
  "documentationUrl": "String",
  "headerTitle": "String",
  "headerSubtitle": "String",
  "keywords": [
    "String"
  ],
  "constraints": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingAppConstraint",
      "supportedTypes": [
        "String"
      ]
    }
  ],
  "dependencies": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingDependency",
      "definitionId": "String",
      "constraints": [
        {
          "@odata.type": "microsoft.graph.deviceManagementSettingAppConstraint",
          "supportedTypes": [
            "String"
          ]
        }
      ]
    }
  ],
  "elementDefinitionId": "String"
}
```



