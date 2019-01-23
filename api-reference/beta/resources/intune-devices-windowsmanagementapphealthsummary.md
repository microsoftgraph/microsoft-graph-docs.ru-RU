---
title: Тип ресурса windowsManagementAppHealthSummary
description: Содержит свойства для Сводка работоспособности приложения управления Windows.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3ca46f61259b8b956439c541bf8d5703a35aa93b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29393853"
---
# <a name="windowsmanagementapphealthsummary-resource-type"></a>Тип ресурса windowsManagementAppHealthSummary

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства для Сводка работоспособности приложения управления Windows.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение windowsManagementAppHealthSummary](../api/intune-devices-windowsmanagementapphealthsummary-get.md)|[windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md).|Чтение свойства и связи объекта [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) .|
|[Обновление windowsManagementAppHealthSummary](../api/intune-devices-windowsmanagementapphealthsummary-update.md)|[windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md).|Обновление свойства объекта [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ сущности сводки работоспособности приложения управления, Windows.|
|healthyDeviceCount|Int32|Счетчик работоспособном устройства.|
|unhealthyDeviceCount|Int32|Счетчик неработоспособные устройства.|
|unknownDeviceCount|Int32|Счетчик неизвестные устройства.|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsManagementAppHealthSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsManagementAppHealthSummary",
  "id": "String (identifier)",
  "healthyDeviceCount": 1024,
  "unhealthyDeviceCount": 1024,
  "unknownDeviceCount": 1024
}
```




