---
title: тип ресурса deviceManagementSettingCategory
description: Объект, представляющий категорию параметра
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7dd0e8d84dbe5f55f6c6e24764d5cddabe036174
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59091435"
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
|id|String|ID категории|
|displayName|String|Имя категории|
|hasRequiredSetting|Логическое|Категория содержит требуемую настройку верхнего уровня|

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



