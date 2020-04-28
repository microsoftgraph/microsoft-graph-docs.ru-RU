---
title: Тип ресурса Граупполициуплоадеддефинитион
description: Сущность описывает все сведения об одной групповой политике.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 480e6010b1f140a35a3a1ff1449770f81d43783d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43469098"
---
# <a name="grouppolicyuploadeddefinition-resource-type"></a>Тип ресурса Граупполициуплоадеддефинитион

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сущность описывает все сведения об одной групповой политике.


Наследуется от [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Граупполициуплоадеддефинитионс](../api/intune-grouppolicy-grouppolicyuploadeddefinition-list.md)|Коллекция [граупполициуплоадеддефинитион](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md)|Список свойств и связей объектов [граупполициуплоадеддефинитион](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) .|
|[Получение Граупполициуплоадеддефинитион](../api/intune-grouppolicy-grouppolicyuploadeddefinition-get.md)|[граупполициуплоадеддефинитион](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md)|Чтение свойств и связей объекта [граупполициуплоадеддефинитион](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) .|
|[Создание Граупполициуплоадеддефинитион](../api/intune-grouppolicy-grouppolicyuploadeddefinition-create.md)|[граупполициуплоадеддефинитион](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md)|Создание нового объекта [граупполициуплоадеддефинитион](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) .|
|[Удаление Граупполициуплоадеддефинитион](../api/intune-grouppolicy-grouppolicyuploadeddefinition-delete.md)|Нет|Удаляет объект [граупполициуплоадеддефинитион](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md).|
|[Обновление Граупполициуплоадеддефинитион](../api/intune-grouppolicy-grouppolicyuploadeddefinition-update.md)|[граупполициуплоадеддефинитион](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md)|Обновление свойств объекта [граупполициуплоадеддефинитион](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|класстипе|[граупполицидефинитионкласстипе](../resources/intune-grouppolicy-grouppolicydefinitionclasstype.md)|Определяет тип групп, к которым можно применить политику. Наследуется от [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md). Возможные значения: `user`, `machine`.|
|displayName|Строка|Имя локализованной политики. Наследуется от [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md)|
|експлаинтекст|String|Локализованное объяснение или текст справки, связанный с политикой. По умолчанию это значение пусто. Наследуется от [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md)|
|категорипас|String|Локализованный полный путь к категории для политики. Наследуется от [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md)|
|суппортедон|String|Локализованная строка, используемая для указания версии операционной системы или приложения, на которые влияет политика. Наследуется от [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md)|
|полицитипе|[граупполицитипе](../resources/intune-grouppolicy-grouppolicytype.md)|Указывает тип групповой политики. Наследуется от [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md). Возможные значения: `admxBacked`, `admxIngested`.|
|граупполицикатегорид|GUID|Идентификатор категории родительской категории, унаследованной от [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md)|
|id|String|Ключ объекта. Наследуется от [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md)|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md)|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|дефинитионфиле|[граупполицидефинитионфиле](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|Файл групповой политики, связанный с определением. Наследуется от [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md)|
|category|[groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)|Категория групповой политики, связанная с определением. Наследуется от [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md)|
|материалы|Коллекция [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)|Презентации групповой политики, связанные с определением. Наследуется от [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md)|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyUploadedDefinition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyUploadedDefinition",
  "classType": "String",
  "displayName": "String",
  "explainText": "String",
  "categoryPath": "String",
  "supportedOn": "String",
  "policyType": "String",
  "groupPolicyCategoryId": "Guid",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```



