---
title: Тип ресурса Виндовсаутопилотдеплойментпрофилеассигнмент
description: Назначение профиля развертывания Windows для автопилотной группы группе AAD.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 884f233908f1757fc775cd302fcdd95a8ed38f32
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34993896"
---
# <a name="windowsautopilotdeploymentprofileassignment-resource-type"></a>Тип ресурса Виндовсаутопилотдеплойментпрофилеассигнмент

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

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

## <a name="relationships"></a>Отношения
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
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```





