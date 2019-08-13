---
title: Тип ресурса Манажементкондитионстатемент
description: Оператор условия управления — это группа условий управления, которые позволяют включать и отключать конфигурации устройств и приложений при выполнении всех включенных условий управления.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2829f320704acc438cce9a416001715517291c32
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36331632"
---
# <a name="managementconditionstatement-resource-type"></a>Тип ресурса Манажементкондитионстатемент

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Оператор условия управления — это группа условий управления, которые позволяют включать и отключать конфигурации устройств и приложений при выполнении всех включенных условий управления.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Манажементкондитионстатементс](../api/intune-fencing-managementconditionstatement-list.md)|Коллекция [манажементкондитионстатемент](../resources/intune-fencing-managementconditionstatement.md)|Список свойств и связей объектов [манажементкондитионстатемент](../resources/intune-fencing-managementconditionstatement.md) .|
|[Получение Манажементкондитионстатемент](../api/intune-fencing-managementconditionstatement-get.md)|[манажементкондитионстатемент](../resources/intune-fencing-managementconditionstatement.md)|Чтение свойств и связей объекта [манажементкондитионстатемент](../resources/intune-fencing-managementconditionstatement.md) .|
|[Создание Манажементкондитионстатемент](../api/intune-fencing-managementconditionstatement-create.md)|[манажементкондитионстатемент](../resources/intune-fencing-managementconditionstatement.md)|Создание нового объекта [манажементкондитионстатемент](../resources/intune-fencing-managementconditionstatement.md) .|
|[Удаление Манажементкондитионстатемент](../api/intune-fencing-managementconditionstatement-delete.md)|Нет|Удаляет объект [манажементкондитионстатемент](../resources/intune-fencing-managementconditionstatement.md).|
|[Обновление Манажементкондитионстатемент](../api/intune-fencing-managementconditionstatement-update.md)|[манажементкондитионстатемент](../resources/intune-fencing-managementconditionstatement.md)|Обновление свойств объекта [манажементкондитионстатемент](../resources/intune-fencing-managementconditionstatement.md) .|
|[Функция Жетманажементкондитионстатементекспрессионстринг](../api/intune-fencing-managementconditionstatement-getmanagementconditionstatementexpressionstring.md)|[манажементкондитионекспрессионстринг](../resources/intune-fencing-managementconditionexpressionstring.md)|Пока не задокументировано.|
|[Функция Жетманажементкондитионстатементсфорплатформ](../api/intune-fencing-managementconditionstatement-getmanagementconditionstatementsforplatform.md)|Коллекция [манажементкондитионстатемент](../resources/intune-fencing-managementconditionstatement.md)|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор оператора условия управления. Созданное системой значение, назначаемое при создании.|
|displayName|Строка|Имя, определенное администратором оператора условия управления.|
|description|String|Заданное администратором описание оператора условия управления.|
|createdDateTime|DateTimeOffset|Время создания оператора условия управления. Созданная сторона службы.|
|modifiedDateTime|DateTimeOffset|Время последнего изменения оператора условия управления. Обновленная сторона службы.|
|выражение|[манажементкондитионекспрессион](../resources/intune-fencing-managementconditionexpression.md)|Выражение оператора условия управления, используемое для оценки активации или деактивации оператора условия управления.|
|eTag|String|Тег ETag оператора условия управления. Обновленная сторона службы.|
|аппликаблеплатформс|Коллекция [девицеплатформтипе](../resources/intune-shared-deviceplatformtype.md)|Соответствующие платформы для этого оператора условия управления.
Это рассчитывается на основе условий управления, связанных с оператором условия управления, и поиском пересечения соответствующих платформ.|

## <a name="relationships"></a>Отношения
|Отношение|Тип|Описание|
|:---|:---|:---|
|манажементкондитионс|Коллекция [манажементкондитион](../resources/intune-fencing-managementcondition.md)|Условия управления, связанные с оператором условия управления.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managementConditionStatement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managementConditionStatement",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "expression": {
    "@odata.type": "microsoft.graph.managementConditionExpression"
  },
  "eTag": "String",
  "applicablePlatforms": [
    "String"
  ]
}
```



