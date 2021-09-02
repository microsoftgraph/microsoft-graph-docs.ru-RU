---
title: тип ресурса deviceManagementIntentSettingCategory
description: Объект, представляющий категорию заданной цели
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ea9a9b63a30e0de8ad8fadf167cdbb51ce5df6a5
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58803513"
---
# <a name="devicemanagementintentsettingcategory-resource-type"></a>тип ресурса deviceManagementIntentSettingCategory

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект, представляющий категорию заданной цели


Наследует [от deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список deviceManagementIntentSettingCategories](../api/intune-deviceintent-devicemanagementintentsettingcategory-list.md)|[коллекция deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md)|Список свойств и связей [объектов deviceManagementIntentSettingCategory.](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md)|
|[Get deviceManagementIntentSettingCategory](../api/intune-deviceintent-devicemanagementintentsettingcategory-get.md)|[deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md)|Чтение свойств и связей [объекта deviceManagementIntentSettingCategory.](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md)|
|[Создание deviceManagementIntentSettingCategory](../api/intune-deviceintent-devicemanagementintentsettingcategory-create.md)|[deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md)|Создание нового [объекта deviceManagementIntentSettingCategory.](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md)|
|[Удаление deviceManagementIntentSettingCategory](../api/intune-deviceintent-devicemanagementintentsettingcategory-delete.md)|Нет|Удаляет [устройствоManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md).|
|[Обновление deviceManagementIntentSettingCategory](../api/intune-deviceintent-devicemanagementintentsettingcategory-update.md)|[deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md)|Обновление свойств объекта [deviceManagementIntentSettingCategory.](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|ID категории, унаследованный от [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|
|displayName|Строка|Имя категории, унаследованные от [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|
|hasRequiredSetting|Логический|Категория содержит обязательный параметр верхнего уровня, унаследованный от [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|settingDefinitions|[коллекция deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)|Определения параметров этой категории содержат унаследованные от [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|
|settings|[коллекция deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|Параметры, которые содержит эта категория|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementIntentSettingCategory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementIntentSettingCategory",
  "id": "String (identifier)",
  "displayName": "String",
  "hasRequiredSetting": true
}
```



