---
title: тип ресурса windowsDefenderApplicationControlSupplementalPolicyAssignment
description: Класс, содержащий свойства, используемые для назначения дополнительной политики WindowsDefenderApplicationControl для группы.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a15f6aada4c052b7fb7fc85c0c1b1a8f8d67830c
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58782898"
---
# <a name="windowsdefenderapplicationcontrolsupplementalpolicyassignment-resource-type"></a>тип ресурса windowsDefenderApplicationControlSupplementalPolicyAssignment

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Класс, содержащий свойства, используемые для назначения дополнительной политики WindowsDefenderApplicationControl для группы.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список windowsDefenderApplicationControlSupplementalPolicyAssignments](../api/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment-list.md)|[коллекция windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md)|Список свойств и связей [объектов windowsDefenderApplicationControlSupplementalPolicyAssignment.](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md)|
|[Get windowsDefenderApplicationControlSupplementalPolicyAssignment](../api/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment-get.md)|[windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md)|Ознакомьтесь с свойствами и отношениями [объекта windowsDefenderApplicationControlSupplementalPolicyAssignment.](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md)|
|[Создание windowsDefenderApplicationControlSupplementalPolicyAssignment](../api/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment-create.md)|[windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md)|Создайте [новый объект WindowsDefenderApplicationControlSupplementalPolicyAssignment.](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md)|
|[Удаление windowsDefenderApplicationControlSupplementalPolicyAssignment](../api/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment-delete.md)|Нет|Удаляет [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md).|
|[Обновление windowsDefenderApplicationControlSupplementalPolicyAssignment](../api/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment-update.md)|[windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md)|Обновление свойств объекта [WindowsDefenderApplicationControlSupplementalPolicyAssignment.](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта.|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|Целевое назначение группы, определенное администратором.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsDefenderApplicationControlSupplementalPolicyAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsDefenderApplicationControlSupplementalPolicyAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String"
  }
}
```



