---
title: Тип ресурса Девицеманажементинтентдевицестатесуммари
description: Сущность, представляющая сводную информацию о состоянии устройства для намерения
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 35d203cfe5431e6e9acff049e041fba9c8f3f193
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43441058"
---
# <a name="devicemanagementintentdevicestatesummary-resource-type"></a>Тип ресурса Девицеманажементинтентдевицестатесуммари

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сущность, представляющая сводную информацию о состоянии устройства для намерения

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение Девицеманажементинтентдевицестатесуммари](../api/intune-deviceintent-devicemanagementintentdevicestatesummary-get.md)|[deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md)|Чтение свойств и связей объекта [девицеманажементинтентдевицестатесуммари](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) .|
|[Обновление Девицеманажементинтентдевицестатесуммари](../api/intune-deviceintent-devicemanagementintentdevicestatesummary-update.md)|[deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md)|Обновление свойств объекта [девицеманажементинтентдевицестатесуммари](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор|
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



