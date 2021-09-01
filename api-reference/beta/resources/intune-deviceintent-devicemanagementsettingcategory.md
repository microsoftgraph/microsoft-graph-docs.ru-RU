---
title: тип ресурса deviceManagementSettingCategory
description: Объект, представляющий категорию параметра
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e5bb023319284c4d1a455f9cac98c2b62f227129
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58797263"
---
# <a name="devicemanagementsettingcategory-resource-type"></a>тип ресурса deviceManagementSettingCategory

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект, представляющий категорию параметра

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список deviceManagementSettingCategories](../api/intune-deviceintent-devicemanagementsettingcategory-list.md)|[коллекция deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|Список свойств и связей [объектов deviceManagementSettingCategory.](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|
|[Get deviceManagementSettingCategory](../api/intune-deviceintent-devicemanagementsettingcategory-get.md)|[deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|Чтение свойств и связей [объекта deviceManagementSettingCategory.](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|
|[Создание deviceManagementSettingCategory](../api/intune-deviceintent-devicemanagementsettingcategory-create.md)|[deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|Создание нового [объекта deviceManagementSettingCategory.](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|
|[Удаление deviceManagementSettingCategory](../api/intune-deviceintent-devicemanagementsettingcategory-delete.md)|Нет|Удаляет [устройствоManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md).|
|[Обновление deviceManagementSettingCategory](../api/intune-deviceintent-devicemanagementsettingcategory-update.md)|[deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|Обновление свойств объекта [deviceManagementSettingCategory.](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|ID категории|
|displayName|String|Имя категории|
|hasRequiredSetting|Логический|Категория содержит требуемую настройку верхнего уровня|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|settingDefinitions|[коллекция deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)|Определения параметров, которые содержит эта категория|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementSettingCategory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingCategory",
  "id": "String (identifier)",
  "displayName": "String",
  "hasRequiredSetting": true
}
```



