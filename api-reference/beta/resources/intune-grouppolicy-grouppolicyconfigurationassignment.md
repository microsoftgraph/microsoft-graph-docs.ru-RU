---
title: Тип ресурса Граупполициконфигуратионассигнмент
description: Объект назначения настройки групповой политики назначает одну или несколько групп AAD определенной конфигурации групповой политики.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0f45bab9ecb7c564e0cda8bd8bff37b1e90048ec
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43377051"
---
# <a name="grouppolicyconfigurationassignment-resource-type"></a>Тип ресурса Граупполициконфигуратионассигнмент

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект назначения настройки групповой политики назначает одну или несколько групп AAD определенной конфигурации групповой политики.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Граупполициконфигуратионассигнментс](../api/intune-grouppolicy-grouppolicyconfigurationassignment-list.md)|Коллекция [граупполициконфигуратионассигнмент](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|Список свойств и связей объектов [граупполициконфигуратионассигнмент](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) .|
|[Получение Граупполициконфигуратионассигнмент](../api/intune-grouppolicy-grouppolicyconfigurationassignment-get.md)|[граупполициконфигуратионассигнмент](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|Чтение свойств и связей объекта [граупполициконфигуратионассигнмент](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) .|
|[Создание Граупполициконфигуратионассигнмент](../api/intune-grouppolicy-grouppolicyconfigurationassignment-create.md)|[граупполициконфигуратионассигнмент](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|Создание нового объекта [граупполициконфигуратионассигнмент](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) .|
|[Удаление Граупполициконфигуратионассигнмент](../api/intune-grouppolicy-grouppolicyconfigurationassignment-delete.md)|Нет|Удаляет объект [граупполициконфигуратионассигнмент](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md).|
|[Обновление Граупполициконфигуратионассигнмент](../api/intune-grouppolicy-grouppolicyconfigurationassignment-update.md)|[граупполициконфигуратионассигнмент](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|Обновление свойств объекта [граупполициконфигуратионассигнмент](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта.|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|Тип групп, нацеленных на конфигурацию групповой политики.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyConfigurationAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyConfigurationAssignment",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



