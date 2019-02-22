---
title: Тип ресурса Граупполицидефинитион
description: Сущность описывает все сведения об одной групповой политике.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e7649d249a034278741199e1f858f07ea34c7137
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30164059"
---
# <a name="grouppolicydefinition-resource-type"></a>Тип ресурса Граупполицидефинитион

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сущность описывает все сведения об одной групповой политике.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение Граупполицидефинитион](../api/intune-grouppolicy-grouppolicydefinition-get.md)|[Граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md)|Чтение свойств и связей объекта [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md) .|
|[Обновление Граупполицидефинитион](../api/intune-grouppolicy-grouppolicydefinition-update.md)|[Граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md)|Обновление свойств объекта [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|Класстипе|[Граупполицидефинитионкласстипе](../resources/intune-grouppolicy-grouppolicydefinitionclasstype.md)|Определяет тип групп, к которым можно применить политику. Возможные значения: `user`, `machine`, `both`.|
|displayName|String|Имя локализованной политики.|
|Експлаинтекст|String|Локализованное объяснение или текст справки, связанный с политикой. Значение по умолчанию — пустое значение.|
|Категорипас|String|Локализованный полный путь к категории для политики.|
|Суппортедон|String|Локализованная строка, используемая для указания версии операционной системы или приложения, на которые влияет политика.|
|Полицитипе|[Граупполицитипе](../resources/intune-grouppolicy-grouppolicytype.md)|Указывает тип групповой политики. Возможные значения: `admxBacked`, `admxIngested`.|
|id|String|Ключ объекта.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта.|

## <a name="relationships"></a>Отношения
|Связь|Тип|Описание|
|:---|:---|:---|
|Дефинитионфиле|[Граупполицидефинитионфиле](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|Файл групповой политики, связанный с определением.|
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




