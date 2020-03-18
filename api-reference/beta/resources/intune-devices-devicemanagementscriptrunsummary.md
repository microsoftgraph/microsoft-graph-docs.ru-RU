---
title: Тип ресурса Девицеманажементскриптрунсуммари
description: Содержит свойства сводки по запуску сценария управления устройствами.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ce974f3d5e024a9559f454e8837fd04183e4de9d
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42784897"
---
# <a name="devicemanagementscriptrunsummary-resource-type"></a>Тип ресурса Девицеманажементскриптрунсуммари

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства сводки по запуску сценария управления устройствами.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение Девицеманажементскриптрунсуммари](../api/intune-devices-devicemanagementscriptrunsummary-get.md)|[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md);|Чтение свойств и связей объекта [девицеманажементскриптрунсуммари](../resources/intune-devices-devicemanagementscriptrunsummary.md) .|
|[Обновление Девицеманажементскриптрунсуммари](../api/intune-devices-devicemanagementscriptrunsummary-update.md)|[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md);|Обновление свойств объекта [девицеманажементскриптрунсуммари](../resources/intune-devices-devicemanagementscriptrunsummary.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Key объекта сводки запуска сценария управления устройствами. Это свойство доступно только для чтения.|
|сукцессдевицекаунт|Int32|Число устройств для успешной попытки.|
|errorDeviceCount|Int32|Количество устройств с ошибками.|
|сукцессусеркаунт|Int32|Число пользователей Success.|
|errorUserCount|Int32|Количество пользователей с ошибками.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementScriptRunSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementScriptRunSummary",
  "id": "String (identifier)",
  "successDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "successUserCount": 1024,
  "errorUserCount": 1024
}
```



