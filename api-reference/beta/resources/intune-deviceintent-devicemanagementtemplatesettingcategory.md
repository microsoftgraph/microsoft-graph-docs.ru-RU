---
title: тип ресурса deviceManagementTemplateSettingCategory
description: Объект, представляющий категорию параметра шаблона
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: cdcc998b69b413b685c09a58ce05bae06d5b385f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59086393"
---
# <a name="devicemanagementtemplatesettingcategory-resource-type"></a>тип ресурса deviceManagementTemplateSettingCategory

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект, представляющий категорию параметра шаблона


Наследует [от deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список deviceManagementTemplateSettingCategories](../api/intune-deviceintent-devicemanagementtemplatesettingcategory-list.md)|[коллекция deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md)|Список свойств и связей [объектов deviceManagementTemplateSettingCategory.](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md)|
|[Get deviceManagementTemplateSettingCategory](../api/intune-deviceintent-devicemanagementtemplatesettingcategory-get.md)|[deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md)|Чтение свойств и связей [объекта deviceManagementTemplateSettingCategory.](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md)|
|[Создание deviceManagementTemplateSettingCategory](../api/intune-deviceintent-devicemanagementtemplatesettingcategory-create.md)|[deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md)|Создайте новый [объект deviceManagementTemplateSettingCategory.](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md)|
|[Удаление deviceManagementTemplateSettingCategory](../api/intune-deviceintent-devicemanagementtemplatesettingcategory-delete.md)|Нет|Удаляет [устройствоManagementTemplateSettingCategory.](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md)|
|[Обновление deviceManagementTemplateSettingCategory](../api/intune-deviceintent-devicemanagementtemplatesettingcategory-update.md)|[deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md)|Обновление свойств объекта [deviceManagementTemplateSettingCategory.](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|ID категории, унаследованный от [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|
|displayName|String|Имя категории, унаследованные от [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|
|hasRequiredSetting|Логическое|Категория содержит обязательный параметр верхнего уровня, унаследованный от [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|settingDefinitions|[коллекция deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)|Определения параметров этой категории содержат унаследованные от [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|
|recommendedSettings|[коллекция deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|Параметры, которые содержит эта категория|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementTemplateSettingCategory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementTemplateSettingCategory",
  "id": "String (identifier)",
  "displayName": "String",
  "hasRequiredSetting": true
}
```



