---
title: тип ресурса groupPolicyUploadedCategory
description: Объект категории сохраняет категорию определения групповой политики
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bc1a97c16cf3d5ca132d2c78233c6627a1fae2a2
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58791812"
---
# <a name="grouppolicyuploadedcategory-resource-type"></a>тип ресурса groupPolicyUploadedCategory

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект категории сохраняет категорию определения групповой политики


Наследует [от groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[List groupPolicyUploadedCategories](../api/intune-grouppolicy-grouppolicyuploadedcategory-list.md)|[коллекция groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md)|Список свойств и связей [объектов groupPolicyUploadedCategory.](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md)|
|[Get groupPolicyUploadedCategory](../api/intune-grouppolicy-grouppolicyuploadedcategory-get.md)|[groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md)|Чтение свойств и связей объекта [groupPolicyUploadedCategory.](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md)|
|[Создание groupPolicyUploadedCategory](../api/intune-grouppolicy-grouppolicyuploadedcategory-create.md)|[groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md)|Создайте новый [объект GroupPolicyUploadedCategory.](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md)|
|[Удаление groupPolicyUploadedCategory](../api/intune-grouppolicy-grouppolicyuploadedcategory-delete.md)|Нет|Удаляет [группуPolicyUploadedCategory.](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md)|
|[Update groupPolicyUploadedCategory](../api/intune-grouppolicy-grouppolicyuploadedcategory-update.md)|[groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md)|Обновление свойств объекта [groupPolicyUploadedCategory.](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Строковой id имени отображения категории, унаследованной от [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)|
|isRoot|Логический|Определяет, является ли категория корневой категорией, унаследованной от [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)|
|id|String|Ключ объекта. Унаследованный от [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Унаследованный от [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|родитель|[groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)|Родительская категория, наследуемая [из groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)|
|children|[коллекция groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)|Категории детей, унаследованные от [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)|
|определения|[коллекция groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|Ближайшие дети GroupPolicyDefinition категории, унаследованные от [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)|
|definitionFile|[groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|ID файла определения категории пришел из унаследованных от [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyUploadedCategory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyUploadedCategory",
  "displayName": "String",
  "isRoot": true,
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```



