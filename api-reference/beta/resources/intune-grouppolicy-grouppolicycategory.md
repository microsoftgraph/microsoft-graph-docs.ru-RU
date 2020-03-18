---
title: Тип ресурса Граупполицикатегори
description: Сущность Category сохраняет категорию определения групповой политики
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0b754020cc4a7c4f7e9fdf7cc35f74d9dcc4c4c1
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783125"
---
# <a name="grouppolicycategory-resource-type"></a>Тип ресурса Граупполицикатегори

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сущность Category сохраняет категорию определения групповой политики

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение Граупполицикатегори](../api/intune-grouppolicy-grouppolicycategory-get.md)|[граупполицикатегори](../resources/intune-grouppolicy-grouppolicycategory.md)|Чтение свойств и связей объекта [граупполицикатегори](../resources/intune-grouppolicy-grouppolicycategory.md) .|
|[Обновление Граупполицикатегори](../api/intune-grouppolicy-grouppolicycategory-update.md)|[граупполицикатегори](../resources/intune-grouppolicy-grouppolicycategory.md)|Обновление свойств объекта [граупполицикатегори](../resources/intune-grouppolicy-grouppolicycategory.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|Строка|Идентификатор строки отображаемого имени категории|
|Корень|Логический|Определяет, является ли категория корневой категорией|
|id|String|Ключ объекта.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|верхнего|[граупполицикатегори](../resources/intune-grouppolicy-grouppolicycategory.md)|Родительская категория|
|children|Коллекция [граупполицикатегори](../resources/intune-grouppolicy-grouppolicycategory.md)|Категории дочерних элементов|
|определения|Коллекция [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md)|Непосредственный дочерний элемент Граупполицидефинитион в категории|
|дефинитионфиле|[граупполицидефинитионфиле](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|Идентификатор файла определения, из которого получена Категория|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyCategory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyCategory",
  "displayName": "String",
  "isRoot": true,
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```



