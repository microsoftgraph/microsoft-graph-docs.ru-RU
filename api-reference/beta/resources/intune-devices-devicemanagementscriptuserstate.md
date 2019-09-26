---
title: Тип ресурса Девицеманажементскриптусерстате
description: Содержит свойства для состояния выполнения пользователя скрипта управления устройствами.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a7ec0bba4bbbc6550ea7e2200a994a987f2bf499
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37197010"
---
# <a name="devicemanagementscriptuserstate-resource-type"></a>Тип ресурса Девицеманажементскриптусерстате

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства для состояния выполнения пользователя скрипта управления устройствами.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Девицеманажементскриптусерстатес](../api/intune-devices-devicemanagementscriptuserstate-list.md)|Коллекция [девицеманажементскриптусерстате](../resources/intune-devices-devicemanagementscriptuserstate.md)|Список свойств и связей объектов [девицеманажементскриптусерстате](../resources/intune-devices-devicemanagementscriptuserstate.md) .|
|[Получение Девицеманажементскриптусерстате](../api/intune-devices-devicemanagementscriptuserstate-get.md)|[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md);|Чтение свойств и связей объекта [девицеманажементскриптусерстате](../resources/intune-devices-devicemanagementscriptuserstate.md) .|
|[Создание Девицеманажементскриптусерстате](../api/intune-devices-devicemanagementscriptuserstate-create.md)|[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md);|Создание нового объекта [девицеманажементскриптусерстате](../resources/intune-devices-devicemanagementscriptuserstate.md) .|
|[Удаление Девицеманажементскриптусерстате](../api/intune-devices-devicemanagementscriptuserstate-delete.md)|Нет|Удаляет объект [девицеманажементскриптусерстате](../resources/intune-devices-devicemanagementscriptuserstate.md).|
|[Обновление Девицеманажементскриптусерстате](../api/intune-devices-devicemanagementscriptuserstate-update.md)|[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md);|Обновление свойств объекта [девицеманажементскриптусерстате](../resources/intune-devices-devicemanagementscriptuserstate.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта состояния пользователя скрипта управления устройствами. Это свойство доступно только для чтения.|
|сукцессдевицекаунт|Int32|Число устройств для указанного пользователя.|
|errorDeviceCount|Int32|Количество устройств с ошибками для определенного пользователя.|
|userPrincipalName|String|Имя участника, указанного пользователем.|

## <a name="relationships"></a>Отношения
|Отношение|Тип|Описание|
|:---|:---|:---|
|deviceRunStates|Коллекция [девицеманажементскриптдевицестате](../resources/intune-devices-devicemanagementscriptdevicestate.md)|Список состояний запуска для этого сценария на всех устройствах определенного пользователя.|

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



