---
title: тип ресурса deviceManagementIntentDeviceState
description: Объект, представляют состояние устройства для намерения
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: cca33420504e14c4452cde88f47a8ab4f6282b6f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59137954"
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



