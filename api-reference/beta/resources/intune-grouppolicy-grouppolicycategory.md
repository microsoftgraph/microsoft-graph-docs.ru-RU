---
title: тип ресурса groupPolicyCategory
description: Объект категории сохраняет категорию определения групповой политики
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3ef4f3f8fa0c8304a1cd0b6383a25340765200916b4d5ec4a48bbbe6d8a8c858
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54182758"
---
# <a name="grouppolicycategory-resource-type"></a>тип ресурса groupPolicyCategory

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект категории сохраняет категорию определения групповой политики

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Get groupPolicyCategory](../api/intune-grouppolicy-grouppolicycategory-get.md)|[groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)|Чтение свойств и связей объекта [groupPolicyCategory.](../resources/intune-grouppolicy-grouppolicycategory.md)|
|[Update groupPolicyCategory](../api/intune-grouppolicy-grouppolicycategory-update.md)|[groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)|Обновление свойств объекта [groupPolicyCategory.](../resources/intune-grouppolicy-grouppolicycategory.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|Строка|Строковой id имени отображения категории|
|isRoot|Логический|Определяет, является ли категория корневой.|
|id|Строка|Ключ объекта.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|родитель|[groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)|Родительская категория|
|children|[коллекция groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)|Категории детей|
|определения|[коллекция groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|Ближайшие дети GroupPolicyDefinition этой категории|
|definitionFile|[groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|ID файла определения, из|

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




