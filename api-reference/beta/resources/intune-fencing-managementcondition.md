---
title: тип ресурса managementCondition
description: Условия управления — это события, которые можно запускать динамически, такие как гео-заборы, заборы времени и сетевые заборы.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8db902ca0f5b0fb00a72e9fd8eee8af02d2c8cab
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59030258"
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

## <a name="relationships"></a>Отношения
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



