---
title: тип ресурса networkManagementCondition
description: Содержит сведения для определения состояния управления сетью.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 009020fa94ed34144dc1f872001054da3bd64c01
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59063925"
---
# <a name="networkmanagementcondition-resource-type"></a>тип ресурса networkManagementCondition

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит сведения для определения состояния управления сетью.


Наследует от [managementCondition](../resources/intune-fencing-managementcondition.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список networkManagementConditions](../api/intune-fencing-networkmanagementcondition-list.md)|[коллекция networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md)|Список свойств и связей объектов [networkManagementCondition.](../resources/intune-fencing-networkmanagementcondition.md)|
|[Get networkManagementCondition](../api/intune-fencing-networkmanagementcondition-get.md)|[networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md)|Чтение свойств и связей объекта [networkManagementCondition.](../resources/intune-fencing-networkmanagementcondition.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для состояния управления. Созданное в системе значение, назначенное при его создания. Унаследованный от [managementCondition](../resources/intune-fencing-managementcondition.md)|
|uniqueName|Строка|Уникальное имя для состояния управления. Используется в выражениях условий управления. Унаследованный от [managementCondition](../resources/intune-fencing-managementcondition.md)|
|displayName|String|Администратор определил имя условия управления. Унаследованный от [managementCondition](../resources/intune-fencing-managementcondition.md)|
|description|String|Администратор определил описание условия управления. Унаследованный от [managementCondition](../resources/intune-fencing-managementcondition.md)|
|createdDateTime|DateTimeOffset|Время создания условия управления. Сгенерированная сторона службы. Унаследованный от [managementCondition](../resources/intune-fencing-managementcondition.md)|
|modifiedDateTime|DateTimeOffset|Время последнего изменения условия управления. Обновленная сторона службы. Унаследованный от [managementCondition](../resources/intune-fencing-managementcondition.md)|
|eTag|String|ETag состояния управления. Обновленная сторона службы. Унаследованный от [managementCondition](../resources/intune-fencing-managementcondition.md)|
|applicablePlatforms|[коллекция devicePlatformType](../resources/intune-fencing-deviceplatformtype.md)|Применимые платформы для этого условия управления. Унаследованный от [managementCondition](../resources/intune-fencing-managementcondition.md)|

## <a name="relationships"></a>Отношения
|Связь|Тип|Описание|
|:---|:---|:---|
|managementConditionStatements|[коллекция managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)|Утверждения условий управления, связанные с состоянием управления. Унаследованный от [managementCondition](../resources/intune-fencing-managementcondition.md)|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.networkManagementCondition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.networkManagementCondition",
  "id": "String (identifier)",
  "uniqueName": "String",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "eTag": "String",
  "applicablePlatforms": [
    "String"
  ]
}
```



