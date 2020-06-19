---
title: Тип ресурса Виндовсаутопилотдеплойментпрофилеассигнмент
description: Назначение профиля развертывания Windows для автопилотной группы группе AAD.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: bd2a538899a93f43c73d03d0f788e036efe3112f
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793544"
---
# <a name="windowsautopilotdeploymentprofileassignment-resource-type"></a>Тип ресурса Виндовсаутопилотдеплойментпрофилеассигнмент

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Назначение профиля развертывания Windows для автопилотной группы группе AAD.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Виндовсаутопилотдеплойментпрофилеассигнментс](../api/intune-enrollment-windowsautopilotdeploymentprofileassignment-list.md)|Коллекция [виндовсаутопилотдеплойментпрофилеассигнмент](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)|Список свойств и связей объектов [виндовсаутопилотдеплойментпрофилеассигнмент](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) .|
|[Получение Виндовсаутопилотдеплойментпрофилеассигнмент](../api/intune-enrollment-windowsautopilotdeploymentprofileassignment-get.md)|[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)|Чтение свойств и связей объекта [виндовсаутопилотдеплойментпрофилеассигнмент](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) .|
|[Создание Виндовсаутопилотдеплойментпрофилеассигнмент](../api/intune-enrollment-windowsautopilotdeploymentprofileassignment-create.md)|[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)|Создание нового объекта [виндовсаутопилотдеплойментпрофилеассигнмент](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) .|
|[Удаление Виндовсаутопилотдеплойментпрофилеассигнмент](../api/intune-enrollment-windowsautopilotdeploymentprofileassignment-delete.md)|Нет|Удаляет объект [виндовсаутопилотдеплойментпрофилеассигнмент](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md).|
|[Обновление Виндовсаутопилотдеплойментпрофилеассигнмент](../api/intune-enrollment-windowsautopilotdeploymentprofileassignment-update.md)|[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)|Обновление свойств объекта [виндовсаутопилотдеплойментпрофилеассигнмент](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ назначения.|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|Цель назначения для профиля развертывания Windows для автопилота.|
|source|[deviceAndAppManagementAssignmentSource](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|Тип ресурса, используемого для развертывания в группу, Direct или в упаковке/набор политик. Возможные значения: `direct`, `policySets`.|
|Идентификатор|String|Идентификатор ресурса, используемого для развертывания в группе|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsAutopilotDeploymentProfileAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeploymentProfileAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String"
  },
  "source": "String",
  "sourceId": "String"
}
```



