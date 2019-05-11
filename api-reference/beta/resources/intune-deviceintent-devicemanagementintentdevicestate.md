---
title: Тип ресурса Девицеманажементинтентдевицестате
description: Объект, представляющий состояние устройства для намерения
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 03951ac855e699856684e32e9baf36c40ce8e2f2
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943321"
---
# <a name="devicemanagementintentdevicestate-resource-type"></a>Тип ресурса Девицеманажементинтентдевицестате

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект, представляющий состояние устройства для намерения

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Девицеманажементинтентдевицестатес](../api/intune-deviceintent-devicemanagementintentdevicestate-list.md)|Коллекция [девицеманажементинтентдевицестате](../resources/intune-deviceintent-devicemanagementintentdevicestate.md)|Список свойств и связей объектов [девицеманажементинтентдевицестате](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) .|
|[Получение Девицеманажементинтентдевицестате](../api/intune-deviceintent-devicemanagementintentdevicestate-get.md)|[deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md)|Чтение свойств и связей объекта [девицеманажементинтентдевицестате](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) .|
|[Создание Девицеманажементинтентдевицестате](../api/intune-deviceintent-devicemanagementintentdevicestate-create.md)|[deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md)|Создание нового объекта [девицеманажементинтентдевицестате](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) .|
|[Удаление Девицеманажементинтентдевицестате](../api/intune-deviceintent-devicemanagementintentdevicestate-delete.md)|Нет|Удаляет объект [девицеманажементинтентдевицестате](../resources/intune-deviceintent-devicemanagementintentdevicestate.md).|
|[Обновление Девицеманажементинтентдевицестате](../api/intune-deviceintent-devicemanagementintentdevicestate-update.md)|[deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md)|Обновление свойств объекта [девицеманажементинтентдевицестате](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Идентификатор|
|userPrincipalName|String|Имя участника-пользователя, сообщаемое на устройстве|
|userName|Строка|Имя пользователя, сообщаемое на устройстве|
|deviceDisplayName|String|Имя устройства, о котором сообщается|
|lastReportedDateTime|DateTimeOffset|Дата и время последнего изменения отчета о намерениях|
|состояние|[Комплианцестатус](../resources/intune-shared-compliancestatus.md)|Состояние устройства для цели. Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.|
|deviceId|Строка|Идентификатор устройства, о котором сообщается|

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




