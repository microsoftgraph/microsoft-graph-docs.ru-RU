---
title: тип ресурса deviceManagementIntentDeviceStateSummary
description: Сущность, представляюая сводку состояния устройства для намерения
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: db0b72aa612e1866e11fe5887759ca417149bcd9
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59137919"
---
# <a name="devicemanagementintentdevicestatesummary-resource-type"></a>тип ресурса deviceManagementIntentDeviceStateSummary

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сущность, представляюая сводку состояния устройства для намерения

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Get deviceManagementIntentDeviceStateSummary](../api/intune-deviceintent-devicemanagementintentdevicestatesummary-get.md)|[deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md)|Чтение свойств и связей [объекта deviceManagementIntentDeviceStateSummary.](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md)|
|[Обновление deviceManagementIntentDeviceStateSummary](../api/intune-deviceintent-devicemanagementintentdevicestatesummary-update.md)|[deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md)|Обновление свойств объекта [deviceManagementIntentDeviceStateSummary.](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|The ID|
|conflictCount|Int32|Количество устройств в конфликте|
|errorCount|Int32|Количество устройств с ошибками.|
|failedCount|Int32|Число устройств со сбоями.|
|notApplicableCount|Int32|Количество неприменимых устройств.|
|notApplicablePlatformCount|Int32|Количество не применимых устройств из-за несоответствия платформы и политики|
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



