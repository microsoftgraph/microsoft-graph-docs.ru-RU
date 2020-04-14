---
title: Тип ресурса Граупполициуплоадедкатегори
description: Сущность Category сохраняет категорию определения групповой политики
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2c6848a8d505980243c721ba0dabcc19f8e56ed6
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43442740"
---
# <a name="grouppolicyuploadedcategory-resource-type"></a>Тип ресурса Граупполициуплоадедкатегори

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сущность Category сохраняет категорию определения групповой политики


Наследуется от [граупполицикатегори](../resources/intune-grouppolicy-grouppolicycategory.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Граупполициуплоадедкатегориес](../api/intune-grouppolicy-grouppolicyuploadedcategory-list.md)|Коллекция [граупполициуплоадедкатегори](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md)|Список свойств и связей объектов [граупполициуплоадедкатегори](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) .|
|[Получение Граупполициуплоадедкатегори](../api/intune-grouppolicy-grouppolicyuploadedcategory-get.md)|[граупполициуплоадедкатегори](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md)|Чтение свойств и связей объекта [граупполициуплоадедкатегори](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) .|
|[Создание Граупполициуплоадедкатегори](../api/intune-grouppolicy-grouppolicyuploadedcategory-create.md)|[граупполициуплоадедкатегори](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md)|Создание нового объекта [граупполициуплоадедкатегори](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) .|
|[Удаление Граупполициуплоадедкатегори](../api/intune-grouppolicy-grouppolicyuploadedcategory-delete.md)|Нет|Удаляет объект [граупполициуплоадедкатегори](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md).|
|[Обновление Граупполициуплоадедкатегори](../api/intune-grouppolicy-grouppolicyuploadedcategory-update.md)|[граупполициуплоадедкатегори](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md)|Обновление свойств объекта [граупполициуплоадедкатегори](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|Строка|Идентификатор строки отображаемого имени категории, унаследованной от [граупполицикатегори](../resources/intune-grouppolicy-grouppolicycategory.md)|
|Корень|Логическое|Определяет, является ли категория корневой категорией, унаследованной от [граупполицикатегори](../resources/intune-grouppolicy-grouppolicycategory.md)|
|id|String|Ключ объекта. Наследуется от [граупполицикатегори](../resources/intune-grouppolicy-grouppolicycategory.md)|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от [граупполицикатегори](../resources/intune-grouppolicy-grouppolicycategory.md)|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|верхнего|[groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)|Родительская категория, унаследованная от [граупполицикатегори](../resources/intune-grouppolicy-grouppolicycategory.md)|
|children|Коллекция [граупполицикатегори](../resources/intune-grouppolicy-grouppolicycategory.md)|Категории дочерних элементов, наследуемых от [граупполицикатегори](../resources/intune-grouppolicy-grouppolicycategory.md)|
|определения|Коллекция [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md)|Непосредственный дочерний элемент Граупполицидефинитион в категории, унаследованной от [граупполицикатегори](../resources/intune-grouppolicy-grouppolicycategory.md)|
|дефинитионфиле|[граупполицидефинитионфиле](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|Идентификатор файла определения, из которого получена Категория, унаследованная из [граупполицикатегори](../resources/intune-grouppolicy-grouppolicycategory.md)|

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



