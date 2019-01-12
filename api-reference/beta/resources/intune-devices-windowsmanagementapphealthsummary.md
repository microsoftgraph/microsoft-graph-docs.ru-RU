---
title: Тип ресурса windowsManagementAppHealthSummary
description: Содержит свойства для Сводка работоспособности приложения управления Windows.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: d2e8dbc0af1d814ecd47210c4def5a7c7e02edd9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27967461"
---
# <a name="windowsmanagementapphealthsummary-resource-type"></a>Тип ресурса windowsManagementAppHealthSummary

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Содержит свойства для Сводка работоспособности приложения управления Windows.
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение windowsManagementAppHealthSummary](../api/intune-devices-windowsmanagementapphealthsummary-get.md)|[windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md).|Чтение свойства и связи объекта [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) .|
|[Обновление windowsManagementAppHealthSummary](../api/intune-devices-windowsmanagementapphealthsummary-update.md)|[windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md).|Обновление свойства объекта [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ сущности сводки работоспособности приложения управления, Windows.|
|healthyDeviceCount|Int32|Счетчик работоспособном устройства.|
|unhealthyDeviceCount|Int32|Счетчик неработоспособные устройства.|
|unknownDeviceCount|Int32|Счетчик неизвестные устройства.|

## <a name="relationships"></a>Связи
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





