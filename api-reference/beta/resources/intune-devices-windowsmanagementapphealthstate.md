---
title: Тип ресурса Виндовсманажементапфеалсстате
description: Объект состояния работоспособности приложения управления Windows.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8841b79b9a284a15999db701e82a2b5062e2930b
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148540"
---
# <a name="windowsmanagementapphealthstate-resource-type"></a>Тип ресурса Виндовсманажементапфеалсстате

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект состояния работоспособности приложения управления Windows.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Виндовсманажементапфеалсстатес](../api/intune-devices-windowsmanagementapphealthstate-list.md)|Коллекция [виндовсманажементапфеалсстате](../resources/intune-devices-windowsmanagementapphealthstate.md)|Список свойств и связей объектов [виндовсманажементапфеалсстате](../resources/intune-devices-windowsmanagementapphealthstate.md) .|
|[Получение Виндовсманажементапфеалсстате](../api/intune-devices-windowsmanagementapphealthstate-get.md)|[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)|Чтение свойств и связей объекта [виндовсманажементапфеалсстате](../resources/intune-devices-windowsmanagementapphealthstate.md) .|
|[Создание Виндовсманажементапфеалсстате](../api/intune-devices-windowsmanagementapphealthstate-create.md)|[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)|Создание нового объекта [виндовсманажементапфеалсстате](../resources/intune-devices-windowsmanagementapphealthstate.md) .|
|[Удаление Виндовсманажементапфеалсстате](../api/intune-devices-windowsmanagementapphealthstate-delete.md)|Нет|Удаляет объект [виндовсманажементапфеалсстате](../resources/intune-devices-windowsmanagementapphealthstate.md).|
|[Обновление Виндовсманажементапфеалсстате](../api/intune-devices-windowsmanagementapphealthstate-update.md)|[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)|Обновление свойств объекта [виндовсманажементапфеалсстате](../resources/intune-devices-windowsmanagementapphealthstate.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор для состояния работоспособности приложения управления Windows|
|healthState|[healthState](../resources/intune-devices-healthstate.md)|Состояние работоспособности приложения управления Windows. Возможные значения: `unknown`, `healthy`, `unhealthy`.|
|Инсталледверсион|String|Установленная версия приложения управления Windows.|
|Ластчеккиндатетиме|DateTimeOffset|Время последнего возврата приложения управления Windows.|
|deviceName|String|Имя устройства, на котором установлено приложение "Управление Windows".|
|Девицеосверсион|String|Версия Windows 10 OS устройства, на котором установлено приложение "Управление Windows".|

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




