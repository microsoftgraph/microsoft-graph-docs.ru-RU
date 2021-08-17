---
title: тип ресурса managementCondition
description: Условия управления — это события, которые можно запускать динамически, такие как гео-заборы, заборы времени и сетевые заборы.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d048e3f977fd8881e18325ee17dffb15a5c20377
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58259176"
---
# <a name="managementcondition-resource-type"></a>тип ресурса managementCondition

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Условия управления — это события, которые можно запускать динамически, такие как гео-заборы, заборы времени и сетевые заборы.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Управление спискамиКондиции](../api/intune-fencing-managementcondition-list.md)|[коллекция managementCondition](../resources/intune-fencing-managementcondition.md)|Список свойств и связей [объектов managementCondition.](../resources/intune-fencing-managementcondition.md)|
|[Get managementCondition](../api/intune-fencing-managementcondition-get.md)|[managementCondition](../resources/intune-fencing-managementcondition.md)|Чтение свойств и связей [объекта managementCondition.](../resources/intune-fencing-managementcondition.md)|
|[функция getManagementConditionsForPlatform](../api/intune-fencing-managementcondition-getmanagementconditionsforplatform.md)|[коллекция managementCondition](../resources/intune-fencing-managementcondition.md)|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для состояния управления. Созданное в системе значение, назначенное при его создания.|
|uniqueName|Строка|Уникальное имя для состояния управления. Используется в выражениях условий управления.|
|displayName|String|Администратор определил имя условия управления.|
|description|String|Администратор определил описание условия управления.|
|createdDateTime|DateTimeOffset|Время создания условия управления. Сгенерированная сторона службы.|
|modifiedDateTime|DateTimeOffset|Время последнего изменения условия управления. Обновленная сторона службы.|
|eTag|String|ETag состояния управления. Обновленная сторона службы.|
|applicablePlatforms|[коллекция devicePlatformType](../resources/intune-fencing-deviceplatformtype.md)|Применимые платформы для этого условия управления.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|managementConditionStatements|[коллекция managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)|Утверждения условий управления, связанные с состоянием управления.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managementCondition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managementCondition",
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




