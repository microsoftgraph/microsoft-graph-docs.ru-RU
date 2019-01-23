---
title: Тип ресурса deviceManagementScriptUserState
description: Содержит свойства для пользователя, состояние сценарий управления устройства выполнения.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d1884967707be8e126724148afa5d04b07f80a48
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29407286"
---
# <a name="devicemanagementscriptuserstate-resource-type"></a>Тип ресурса deviceManagementScriptUserState

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства для пользователя, состояние сценарий управления устройства выполнения.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список deviceManagementScriptUserStates](../api/intune-devices-devicemanagementscriptuserstate-list.md)|[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) коллекции|Свойства списка и связей объектов [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) .|
|[Получение deviceManagementScriptUserState](../api/intune-devices-devicemanagementscriptuserstate-get.md)|[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md);|Чтение свойства и связи объекта [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) .|
|[Создание deviceManagementScriptUserState](../api/intune-devices-devicemanagementscriptuserstate-create.md)|[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md);|Создание нового объекта [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) .|
|[Удаление deviceManagementScriptUserState](../api/intune-devices-devicemanagementscriptuserstate-delete.md)|Нет|Удаляет [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md).|
|[Обновление deviceManagementScriptUserState](../api/intune-devices-devicemanagementscriptuserstate-update.md)|[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md);|Обновление свойства объекта [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ сущности состояние пользователя устройства управления скрипта.|
|successDeviceCount|Int32|Число допустимых устройства для определенного пользователя.|
|errorDeviceCount|Int32|Число ошибок устройства для определенного пользователя.|
|userPrincipalName|String|Имени участника-пользователя для определенного пользователя.|

## <a name="relationships"></a>Отношения
|Связь|Тип|Описание|
|:---|:---|:---|
|deviceRunStates|[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) коллекции|Список выполнения состояний для этого скрипта на всех устройствах определенного пользователя.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementScriptUserState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementScriptUserState",
  "id": "String (identifier)",
  "successDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "userPrincipalName": "String"
}
```




