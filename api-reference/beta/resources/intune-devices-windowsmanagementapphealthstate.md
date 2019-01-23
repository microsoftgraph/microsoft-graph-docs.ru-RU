---
title: Тип ресурса windowsManagementAppHealthState
description: Сущность состояние работоспособности приложения управления Windows.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 171ae2492eb5077567f4398af678d14044a0b7e2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395736"
---
# <a name="windowsmanagementapphealthstate-resource-type"></a>Тип ресурса windowsManagementAppHealthState

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сущность состояние работоспособности приложения управления Windows.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список windowsManagementAppHealthStates](../api/intune-devices-windowsmanagementapphealthstate-list.md)|[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) коллекции|Свойства списка и связей объектов [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) .|
|[Получение windowsManagementAppHealthState](../api/intune-devices-windowsmanagementapphealthstate-get.md)|[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)|Чтение свойства и связи объекта [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) .|
|[Создание windowsManagementAppHealthState](../api/intune-devices-windowsmanagementapphealthstate-create.md)|[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)|Создание нового объекта [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) .|
|[Удаление windowsManagementAppHealthState](../api/intune-devices-windowsmanagementapphealthstate-delete.md)|Нет|Удаляет [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md).|
|[Обновление windowsManagementAppHealthState](../api/intune-devices-windowsmanagementapphealthstate-update.md)|[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)|Обновление свойства объекта [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для состояния работоспособности приложения управления Windows|
|healthState|[healthState](../resources/intune-devices-healthstate.md)|Состояния работоспособности приложения управления Windows. Возможные значения: `unknown`, `healthy`, `unhealthy`.|
|installedVersion|String|Управление приложения установленной версии Windows.|
|lastCheckInDateTime|DateTimeOffset|Приложение управления Windows последний раз.|
|deviceName|String|Имя устройства, на какие Windows установлено приложение управления.|
|deviceOSVersion|String|10 версии Windows устройства, на какие Windows установлено приложение управления.|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsManagementAppHealthState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsManagementAppHealthState",
  "id": "String (identifier)",
  "healthState": "String",
  "installedVersion": "String",
  "lastCheckInDateTime": "String (timestamp)",
  "deviceName": "String",
  "deviceOSVersion": "String"
}
```




