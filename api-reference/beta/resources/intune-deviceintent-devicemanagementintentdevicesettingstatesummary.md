---
title: тип ресурса deviceManagementIntentDeviceSettingStateSummary
description: Объект, представляю который представляет сводку состояния устройства для намерения
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 37b16fe8e6095b1ab957e30b00b870560f33ae26
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58803520"
---
# <a name="devicemanagementintentdevicesettingstatesummary-resource-type"></a>тип ресурса deviceManagementIntentDeviceSettingStateSummary

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект, представляю который представляет сводку состояния устройства для намерения

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список deviceManagementIntentDeviceSettingStateSummaries](../api/intune-deviceintent-devicemanagementintentdevicesettingstatesummary-list.md)|[коллекция deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md)|Список свойств и связей [объектов deviceManagementIntentDeviceSettingStateSummary.](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md)|
|[Get deviceManagementIntentDeviceSettingStateSummary](../api/intune-deviceintent-devicemanagementintentdevicesettingstatesummary-get.md)|[deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md)|Чтение свойств и связей [объекта deviceManagementIntentDeviceSettingStateSummary.](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md)|
|[Создание deviceManagementIntentDeviceSettingStateSummary](../api/intune-deviceintent-devicemanagementintentdevicesettingstatesummary-create.md)|[deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md)|Создайте новый [объект deviceManagementIntentDeviceSettingStateSummary.](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md)|
|[Удаление deviceManagementIntentDeviceSettingStateSummary](../api/intune-deviceintent-devicemanagementintentdevicesettingstatesummary-delete.md)|Нет|Удаляет [устройствоManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md).|
|[Обновление deviceManagementIntentDeviceSettingStateSummary](../api/intune-deviceintent-devicemanagementintentdevicesettingstatesummary-update.md)|[deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md)|Обновление свойств объекта [deviceManagementIntentDeviceSettingStateSummary.](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|The ID|
|settingName|String|Имя параметра|
|compliantCount|Int32|Количество устройств, соответствующих требованиям.|
|conflictCount|Int32|Количество устройств в конфликте|
|errorCount|Int32|Количество устройств с ошибками.|
|nonCompliantCount|Int32|Число устройств, не совместимых с соответствием требованиям|
|notApplicableCount|Int32|Количество неприменимых устройств.|
|исправленоКоунт|Int32|Количество исправленных устройств.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementIntentDeviceSettingStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementIntentDeviceSettingStateSummary",
  "id": "String (identifier)",
  "settingName": "String",
  "compliantCount": 1024,
  "conflictCount": 1024,
  "errorCount": 1024,
  "nonCompliantCount": 1024,
  "notApplicableCount": 1024,
  "remediatedCount": 1024
}
```



