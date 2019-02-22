---
title: Тип ресурса Виндовсманажементапфеалссуммари
description: Содержит свойства для сводки о работоспособности приложения управления Windows.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f62f5967702143149176cecd2513478256ead6d3
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172060"
---
# <a name="windowsmanagementapphealthsummary-resource-type"></a>Тип ресурса Виндовсманажементапфеалссуммари

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства для сводки о работоспособности приложения управления Windows.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение Виндовсманажементапфеалссуммари](../api/intune-devices-windowsmanagementapphealthsummary-get.md)|[windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md).|Чтение свойств и связей объекта [виндовсманажементапфеалссуммари](../resources/intune-devices-windowsmanagementapphealthsummary.md) .|
|[Обновление Виндовсманажементапфеалссуммари](../api/intune-devices-windowsmanagementapphealthsummary-update.md)|[windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md).|Обновление свойств объекта [виндовсманажементапфеалссуммари](../resources/intune-devices-windowsmanagementapphealthsummary.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта сводки работоспособности приложения управления Windows.|
|Хеалсидевицекаунт|Int32|Работоспособное число устройств.|
|Унхеалсидевицекаунт|Int32|Неработоспособное число устройств.|
|unknownDeviceCount|Int32|Количество неИзвестных устройств.|

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




