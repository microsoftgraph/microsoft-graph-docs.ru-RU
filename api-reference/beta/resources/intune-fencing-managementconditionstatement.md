---
title: Тип ресурса Манажементкондитионстатемент
description: Оператор условия управления — это группа условий управления, которые позволяют включать и отключать конфигурации устройств и приложений при выполнении всех включенных условий управления.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5bf18a43c7e971b2e81915d4f5f917f2e99e41b2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48031307"
---
# <a name="managementconditionstatement-resource-type"></a>Тип ресурса Манажементкондитионстатемент

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

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
|displayName|String|Имя, определенное администратором оператора условия управления.|
|description|String|Заданное администратором описание оператора условия управления.|
|createdDateTime|DateTimeOffset|Время создания оператора условия управления. Созданная сторона службы.|
|modifiedDateTime|DateTimeOffset|Время последнего изменения оператора условия управления. Обновленная сторона службы.|
|выражение|[манажементкондитионекспрессион](../resources/intune-fencing-managementconditionexpression.md)|Выражение оператора условия управления, используемое для оценки активации или деактивации оператора условия управления.|
|eTag|String|Тег ETag оператора условия управления. Обновленная сторона службы.|
|аппликаблеплатформс|Коллекция [девицеплатформтипе](../resources/intune-shared-deviceplatformtype.md)|Соответствующие платформы для этого оператора условия управления.
Это рассчитывается на основе условий управления, связанных с оператором условия управления, и поиском пересечения соответствующих платформ.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
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
    "@odata.type": "microsoft.graph.managementConditionExpressionString",
    "value": "String"
  },
  "eTag": "String",
  "applicablePlatforms": [
    "String"
  ]
}
```






