---
title: Тип ресурса Граупполицидефинитион
description: Сущность описывает все сведения об одной групповой политике.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 038647f4e40036db89ecf61cdece531662658c46
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528091"
---
# <a name="grouppolicydefinition-resource-type"></a>Тип ресурса Граупполицидефинитион

Пространство имен: Microsoft. Graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сущность описывает все сведения об одной групповой политике.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение Граупполицидефинитион](../api/intune-grouppolicy-grouppolicydefinition-get.md)|[граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md)|Чтение свойств и связей объекта [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md) .|
|[Обновление Граупполицидефинитион](../api/intune-grouppolicy-grouppolicydefinition-update.md)|[граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md)|Обновление свойств объекта [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|класстипе|[граупполицидефинитионкласстипе](../resources/intune-grouppolicy-grouppolicydefinitionclasstype.md)|Определяет тип групп, к которым можно применить политику. Возможные значения: `user`, `machine`.|
|displayName|Строка|Имя локализованной политики.|
|експлаинтекст|String|Локализованное объяснение или текст справки, связанный с политикой. По умолчанию это значение пусто.|
|категорипас|String|Локализованный полный путь к категории для политики.|
|суппортедон|String|Локализованная строка, используемая для указания версии операционной системы или приложения, на которые влияет политика.|
|полицитипе|[граупполицитипе](../resources/intune-grouppolicy-grouppolicytype.md)|Указывает тип групповой политики. Возможные значения: `admxBacked`, `admxIngested`.|
|id|String|Ключ объекта.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|дефинитионфиле|[граупполицидефинитионфиле](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|Файл групповой политики, связанный с определением.|
|материалы|Коллекция [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)|Презентации групповой политики, связанные с определением.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyDefinition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyDefinition",
  "classType": "String",
  "displayName": "String",
  "explainText": "String",
  "categoryPath": "String",
  "supportedOn": "String",
  "policyType": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```



