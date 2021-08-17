---
title: тип ресурса deviceManagementIntentDeviceState
description: Объект, представляют состояние устройства для намерения
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 30cb1fcb0d8078ad6707a535a687cc617c9f0bcd1175f4437b959800d7edb744
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54164225"
---
# <a name="devicemanagementintentdevicestate-resource-type"></a>тип ресурса deviceManagementIntentDeviceState

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект, представляют состояние устройства для намерения

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список deviceManagementIntentDeviceStates](../api/intune-deviceintent-devicemanagementintentdevicestate-list.md)|[коллекция deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md)|Список свойств и связей [объектов deviceManagementIntentDeviceState.](../resources/intune-deviceintent-devicemanagementintentdevicestate.md)|
|[Get deviceManagementIntentDeviceState](../api/intune-deviceintent-devicemanagementintentdevicestate-get.md)|[deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md)|Чтение свойств и связей [объекта deviceManagementIntentDeviceState.](../resources/intune-deviceintent-devicemanagementintentdevicestate.md)|
|[Создание deviceManagementIntentDeviceState](../api/intune-deviceintent-devicemanagementintentdevicestate-create.md)|[deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md)|Создание нового [объекта deviceManagementIntentDeviceState.](../resources/intune-deviceintent-devicemanagementintentdevicestate.md)|
|[Удаление deviceManagementIntentDeviceState](../api/intune-deviceintent-devicemanagementintentdevicestate-delete.md)|Нет|Удаляет [устройствоManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md).|
|[Обновление deviceManagementIntentDeviceState](../api/intune-deviceintent-devicemanagementintentdevicestate-update.md)|[deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md)|Обновление свойств объекта [deviceManagementIntentDeviceState.](../resources/intune-deviceintent-devicemanagementintentdevicestate.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|The ID|
|userPrincipalName|String|Основное имя пользователя, которое сообщается на устройстве|
|userName|String|Имя пользователя, которое сообщается на устройстве|
|deviceDisplayName|String|Имя устройства, которое сообщается|
|lastReportedDateTime|DateTimeOffset|Последнее измененное время даты отчета о намерениях|
|state|[complianceStatus](../resources/intune-shared-compliancestatus.md)|Состояние устройства для намерения. Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.|
|deviceId|String|ID устройства, который сообщается|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementIntentDeviceState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementIntentDeviceState",
  "id": "String (identifier)",
  "userPrincipalName": "String",
  "userName": "String",
  "deviceDisplayName": "String",
  "lastReportedDateTime": "String (timestamp)",
  "state": "String",
  "deviceId": "String"
}
```




