---
title: Тип ресурса Девицеманажементскриптрунсуммари
description: Содержит свойства сводки по запуску сценария управления устройствами.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3fe26fc121d0d1d9339de999101975d2c4c225a5
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30174272"
---
# <a name="devicemanagementscriptrunsummary-resource-type"></a>Тип ресурса Девицеманажементскриптрунсуммари

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства сводки по запуску сценария управления устройствами.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение Девицеманажементскриптрунсуммари](../api/intune-devices-devicemanagementscriptrunsummary-get.md)|[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md);|Чтение свойств и связей объекта [девицеманажементскриптрунсуммари](../resources/intune-devices-devicemanagementscriptrunsummary.md) .|
|[Обновление Девицеманажементскриптрунсуммари](../api/intune-devices-devicemanagementscriptrunsummary-update.md)|[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md);|Обновление свойств объекта [девицеманажементскриптрунсуммари](../resources/intune-devices-devicemanagementscriptrunsummary.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Key объекта сводки запуска сценария управления устройствами.|
|Сукцессдевицекаунт|Int32|Число устройств для успешной попытки.|
|errorDeviceCount|Int32|Количество устройств с ошибками.|
|Сукцессусеркаунт|Int32|Число пользователей Success.|
|errorUserCount|Int32|Количество пользователей с ошибками.|

## <a name="relationships"></a>Отношения
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




