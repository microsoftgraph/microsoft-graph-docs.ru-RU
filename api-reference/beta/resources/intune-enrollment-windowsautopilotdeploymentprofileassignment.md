---
title: тип ресурса windowsAutopilotDeploymentProfileAssignment
description: Назначение профиля развертывания Windows автопилота группе AAD.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2ef6a60f640f6049aa0affeda697d8272c06f27c
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58820844"
---
# <a name="windowsautopilotdeploymentprofileassignment-resource-type"></a>тип ресурса windowsAutopilotDeploymentProfileAssignment

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Назначение профиля развертывания Windows автопилота группе AAD.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список windowsAutopilotDeploymentProfileAssignments](../api/intune-enrollment-windowsautopilotdeploymentprofileassignment-list.md)|[коллекция windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)|Список свойств и связей [объектов windowsAutopilotDeploymentProfileAssignment.](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)|
|[Get windowsAutopilotDeploymentProfileAssignment](../api/intune-enrollment-windowsautopilotdeploymentprofileassignment-get.md)|[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)|Чтение свойств и связей [объекта windowsAutopilotDeploymentProfileAssignment.](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)|
|[Создание windowsAutopilotDeploymentProfileAssignment](../api/intune-enrollment-windowsautopilotdeploymentprofileassignment-create.md)|[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)|Создание нового [объекта windowsAutopilotDeploymentProfileAssignment.](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)|
|[Удаление windowsAutopilotDeploymentProfileAssignment](../api/intune-enrollment-windowsautopilotdeploymentprofileassignment-delete.md)|Нет|Удаляет [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md).|
|[Обновление windowsAutopilotDeploymentProfileAssignment](../api/intune-enrollment-windowsautopilotdeploymentprofileassignment-update.md)|[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)|Обновление свойств объекта [windowsAutopilotDeploymentProfileAssignment.](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ назначения.|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|Цель назначения для Windows профиля развертывания автопилота.|
|source|[deviceAndAppManagementAssignmentSource](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|Тип ресурса, используемого для развертывания в группу, прямую или пакетную группу/policySet. Возможные значения: `direct`, `policySets`.|
|sourceId|String|Идентификатор ресурса, используемой для развертывания в группе|

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



