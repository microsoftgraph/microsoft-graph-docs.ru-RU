---
title: Тип ресурса mobileAppAssignment
description: Класс, содержащий свойства, которые используются для назначения групп в мобильном приложении.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 012ce8e1e67ea89f1cb8e62c6cfda04d8007e526
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49281126"
---
# <a name="mobileappassignment-resource-type"></a>Тип ресурса mobileAppAssignment

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Класс, содержащий свойства, которые используются для назначения групп в мобильном приложении.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов mobileAppAssignment](../api/intune-apps-mobileappassignment-list.md)|Коллекция [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)|Список свойств и связей объектов [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).|
|[Получение объекта mobileAppAssignment](../api/intune-apps-mobileappassignment-get.md)|[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)|Чтение свойств и связей объекта [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).|
|[Создание объекта mobileAppAssignment](../api/intune-apps-mobileappassignment-create.md)|[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)|Создание объекта [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).|
|[Удаление объекта mobileAppAssignment](../api/intune-apps-mobileappassignment-delete.md)|Нет|Удаляет объект [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).|
|[Обновление объекта mobileAppAssignment](../api/intune-apps-mobileappassignment-update.md)|[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)|Обновление свойств объекта [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
|intent|[installIntent](../resources/intune-shared-installintent.md)|Цель установки, определенная администратором. Возможные значения: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|Целевое назначение группы, определенное администратором.|
|settings|[mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)|Параметры целевого назначения, определенные администратором.|
|source|[deviceAndAppManagementAssignmentSource](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|Тип ресурса, который является источником для назначения. Возможные значения: `direct`, `policySets`.|
|Идентификатор|String|Идентификатор источника назначения.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppAssignment",
  "id": "String (identifier)",
  "intent": "String",
  "target": {
    "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String"
  },
  "settings": {
    "@odata.type": "microsoft.graph.iosLobAppAssignmentSettings",
    "vpnConfigurationId": "String",
    "uninstallOnDeviceRemoval": true
  },
  "source": "String",
  "sourceId": "String"
}
```




