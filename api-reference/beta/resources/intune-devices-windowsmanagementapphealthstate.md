---
title: Тип ресурса Виндовсманажементапфеалсстате
description: Объект состояния работоспособности приложения управления Windows.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d4cf9c680e929e06abce33b96fb89b232dc928ac
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48731045"
---
# <a name="windowsmanagementapphealthstate-resource-type"></a>Тип ресурса Виндовсманажементапфеалсстате

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

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
|id|Строка|Уникальный идентификатор для состояния работоспособности приложения управления Windows. Это свойство доступно только для чтения.|
|healthState|[healthState](../resources/intune-devices-healthstate.md)|Состояние работоспособности приложения управления Windows. Возможные значения: `unknown`, `healthy`, `unhealthy`.|
|инсталледверсион|Строка|Установленная версия приложения управления Windows.|
|ластчеккиндатетиме|DateTimeOffset|Время последнего возврата приложения управления Windows.|
|deviceName|String|Имя устройства, на котором установлено приложение "Управление Windows".|
|девицеосверсион|Строка|Версия Windows 10 OS устройства, на котором установлено приложение "Управление Windows".|

## <a name="relationships"></a>Связи
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





