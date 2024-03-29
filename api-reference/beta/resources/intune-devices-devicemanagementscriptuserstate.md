---
title: тип ресурса deviceManagementScriptUserState
description: Содержит свойства для состояния запуска пользователя скрипта управления устройствами.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 683084b1505c91718e10661e8605c6c8fa7003b7
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59125968"
---
# <a name="devicemanagementscriptuserstate-resource-type"></a>тип ресурса deviceManagementScriptUserState

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства для состояния запуска пользователя скрипта управления устройствами.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список deviceManagementScriptUserStates](../api/intune-devices-devicemanagementscriptuserstate-list.md)|[коллекция deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)|Список свойств и связей [объектов deviceManagementScriptUserState.](../resources/intune-devices-devicemanagementscriptuserstate.md)|
|[Get deviceManagementScriptUserState](../api/intune-devices-devicemanagementscriptuserstate-get.md)|[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md);|Чтение свойств и связей [объекта deviceManagementScriptUserState.](../resources/intune-devices-devicemanagementscriptuserstate.md)|
|[Создание deviceManagementScriptUserState](../api/intune-devices-devicemanagementscriptuserstate-create.md)|[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md);|Создайте новый [объект deviceManagementScriptUserState.](../resources/intune-devices-devicemanagementscriptuserstate.md)|
|[Удаление deviceManagementScriptUserState](../api/intune-devices-devicemanagementscriptuserstate-delete.md)|Нет|Удаляет [устройствоManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md).|
|[Обновление deviceManagementScriptUserState](../api/intune-devices-devicemanagementscriptuserstate-update.md)|[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md);|Обновление свойств объекта [deviceManagementScriptUserState.](../resources/intune-devices-devicemanagementscriptuserstate.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ пользовательского состояния скрипта управления устройствами. Это свойство доступно только для чтения.|
|successDeviceCount|Int32|Количество устройств успешности для определенного пользователя.|
|errorDeviceCount|Int32|Количество устройств ошибки для определенного пользователя.|
|userPrincipalName|String|Имя принципа пользователя конкретного пользователя.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|deviceRunStates|[коллекция deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)|Список состояния запуска для этого скрипта на всех устройствах определенного пользователя.|

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



