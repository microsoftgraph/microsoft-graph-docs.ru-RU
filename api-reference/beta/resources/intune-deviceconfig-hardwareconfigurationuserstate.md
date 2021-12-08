---
title: тип ресурса hardwareConfigurationUserState
description: Содержит свойства состояния пользователя конфигурации оборудования
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ecd964d5c5f2d18ffef71e04ebba40de8f3759ff
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2021
ms.locfileid: "61345658"
---
# <a name="hardwareconfigurationuserstate-resource-type"></a>тип ресурса hardwareConfigurationUserState

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства состояния пользователя конфигурации оборудования

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список hardwareConfigurationUserStates](../api/intune-deviceconfig-hardwareconfigurationuserstate-list.md)|[коллекция hardwareConfigurationUserState](../resources/intune-deviceconfig-hardwareconfigurationuserstate.md)|Список свойств и связей объектов [hardwareConfigurationUserState.](../resources/intune-deviceconfig-hardwareconfigurationuserstate.md)|
|[Get hardwareConfigurationUserState](../api/intune-deviceconfig-hardwareconfigurationuserstate-get.md)|[hardwareConfigurationUserState](../resources/intune-deviceconfig-hardwareconfigurationuserstate.md)|Чтение свойств и связей объекта [hardwareConfigurationUserState.](../resources/intune-deviceconfig-hardwareconfigurationuserstate.md)|
|[Создание hardwareConfigurationUserState](../api/intune-deviceconfig-hardwareconfigurationuserstate-create.md)|[hardwareConfigurationUserState](../resources/intune-deviceconfig-hardwareconfigurationuserstate.md)|Создание нового [объекта hardwareConfigurationUserState.](../resources/intune-deviceconfig-hardwareconfigurationuserstate.md)|
|[Удаление hardwareConfigurationUserState](../api/intune-deviceconfig-hardwareconfigurationuserstate-delete.md)|Нет|Удаляет [hardwareConfigurationUserState](../resources/intune-deviceconfig-hardwareconfigurationuserstate.md).|
|[Обновление hardwareConfigurationUserState](../api/intune-deviceconfig-hardwareconfigurationuserstate-update.md)|[hardwareConfigurationUserState](../resources/intune-deviceconfig-hardwareconfigurationuserstate.md)|Обновление свойств объекта [hardwareConfigurationUserState.](../resources/intune-deviceconfig-hardwareconfigurationuserstate.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта состояния состояния скрипта конфигурации оборудования. Это свойство доступно только для чтения.|
|upn|Строка|Имя участника-пользователя (UPN)|
|userEmail|String|Адрес электронной почты пользователя|
|userName|String|Имя пользователя|
|lastStateUpdateDateTime|DateTimeOffset|Последний период времени при выполнении конфигурации оборудования|
|successfulDeviceCount|Int32|Количество устройств успеха для конкретного пользователя|
|failedDeviceCount|Int32|Неудалось количество устройств для конкретного пользователя|
|pendingDeviceCount|Int32|Ожидание подсчета устройств для определенного пользователя.|
|errorDeviceCount|Int32|Количество устройств ошибки для определенного пользователя.|
|notApplicableDeviceCount|Int32|Не применимое количество устройств для конкретного пользователя.|
|unknownDeviceCount|Int32|Неизвестное количество устройств для определенного пользователя.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.hardwareConfigurationUserState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.hardwareConfigurationUserState",
  "id": "String (identifier)",
  "upn": "String",
  "userEmail": "String",
  "userName": "String",
  "lastStateUpdateDateTime": "String (timestamp)",
  "successfulDeviceCount": 1024,
  "failedDeviceCount": 1024,
  "pendingDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "unknownDeviceCount": 1024
}
```




