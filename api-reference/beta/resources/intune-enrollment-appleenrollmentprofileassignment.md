---
title: Тип ресурса Апплинроллментпрофилеассигнмент
description: Назначение профиля Apple.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b4a86d0ea1b50f3630288ad142cc9d6d1a340683
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528360"
---
# <a name="appleenrollmentprofileassignment-resource-type"></a>Тип ресурса Апплинроллментпрофилеассигнмент

Пространство имен: Microsoft. Graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Назначение профиля Apple.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Апплинроллментпрофилеассигнментс](../api/intune-enrollment-appleenrollmentprofileassignment-list.md)|Коллекция [апплинроллментпрофилеассигнмент](../resources/intune-enrollment-appleenrollmentprofileassignment.md)|Список свойств и связей объектов [апплинроллментпрофилеассигнмент](../resources/intune-enrollment-appleenrollmentprofileassignment.md) .|
|[Получение Апплинроллментпрофилеассигнмент](../api/intune-enrollment-appleenrollmentprofileassignment-get.md)|[appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md)|Чтение свойств и связей объекта [апплинроллментпрофилеассигнмент](../resources/intune-enrollment-appleenrollmentprofileassignment.md) .|
|[Создание Апплинроллментпрофилеассигнмент](../api/intune-enrollment-appleenrollmentprofileassignment-create.md)|[appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md)|Создание нового объекта [апплинроллментпрофилеассигнмент](../resources/intune-enrollment-appleenrollmentprofileassignment.md) .|
|[Удаление Апплинроллментпрофилеассигнмент](../api/intune-enrollment-appleenrollmentprofileassignment-delete.md)|Нет|Удаляет объект [апплинроллментпрофилеассигнмент](../resources/intune-enrollment-appleenrollmentprofileassignment.md).|
|[Обновление Апплинроллментпрофилеассигнмент](../api/intune-enrollment-appleenrollmentprofileassignment-update.md)|[appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md)|Обновление свойств объекта [апплинроллментпрофилеассигнмент](../resources/intune-enrollment-appleenrollmentprofileassignment.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ назначения.|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|Цель назначения для профиля развертывания, инициированного пользователем Apple.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.appleEnrollmentProfileAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appleEnrollmentProfileAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



