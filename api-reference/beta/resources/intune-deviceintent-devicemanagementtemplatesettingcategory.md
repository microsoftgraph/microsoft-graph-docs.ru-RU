---
title: тип ресурса deviceManagementTemplateSettingCategory
description: Объект, представляющий категорию параметра шаблона
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: db744fc2b5888881cef52962fbe259354a47f62142afa8ed7d8bd2ae0a5a349c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54139448"
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
|id|Строка|ID категории, унаследованный от [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|
|displayName|Строка|Имя категории, унаследованные от [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|
|hasRequiredSetting|Логический|Категория содержит обязательный параметр верхнего уровня, унаследованный от [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|

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




