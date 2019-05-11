---
title: Тип ресурса Девицеманажементинтентдевицестатесуммари
description: Сущность, представляющая сводную информацию о состоянии устройства для намерения
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2d9e0d8af7992248114364d7bdf4c2c34d2c715b
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943385"
---
# <a name="devicemanagementintentdevicestatesummary-resource-type"></a>Тип ресурса Девицеманажементинтентдевицестатесуммари

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сущность, представляющая сводную информацию о состоянии устройства для намерения

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение Девицеманажементинтентдевицестатесуммари](../api/intune-deviceintent-devicemanagementintentdevicestatesummary-get.md)|[deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md)|Чтение свойств и связей объекта [девицеманажементинтентдевицестатесуммари](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) .|
|[Обновление Девицеманажементинтентдевицестатесуммари](../api/intune-deviceintent-devicemanagementintentdevicestatesummary-update.md)|[deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md)|Обновление свойств объекта [девицеманажементинтентдевицестатесуммари](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Идентификатор|
|conflictCount|Int32|Количество конфликтующих устройств|
|errorCount|Int32|Количество устройств с ошибками.|
|failedCount|Int32|Число устройств со сбоями.|
|notApplicableCount|Int32|Количество неприменимых устройств.|
|Свойства notapplicableplatformcount|Int32|Количество неприменимых устройств из-за несовпадения платформы и политики|
|successCount|Int32|Количество успешных устройств.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementIntentDeviceStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementIntentDeviceStateSummary",
  "id": "String (identifier)",
  "conflictCount": 1024,
  "errorCount": 1024,
  "failedCount": 1024,
  "notApplicableCount": 1024,
  "notApplicablePlatformCount": 1024,
  "successCount": 1024
}
```




