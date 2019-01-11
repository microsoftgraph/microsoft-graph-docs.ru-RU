---
title: Тип ресурса deviceCompliancePolicySettingStateSummary
description: Сводка по состоянию параметров политики соответствия для устройств в учетной записи.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: afe2b1518aa2ac9c803cc41fce2efffabf4c44d3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844844"
---
# <a name="devicecompliancepolicysettingstatesummary-resource-type"></a>Тип ресурса deviceCompliancePolicySettingStateSummary

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Сводка по состоянию параметров политики соответствия для устройств в учетной записи.
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов deviceCompliancePolicySettingStateSummary](../api/intune-deviceconfig-devicecompliancepolicysettingstatesummary-list.md)|Коллекция [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md)|Список свойств и связей объектов [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).|
|[Получение объекта deviceCompliancePolicySettingStateSummary](../api/intune-deviceconfig-devicecompliancepolicysettingstatesummary-get.md)|[deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md)|Чтение свойств и связей объекта [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).|
|[Создание объекта deviceCompliancePolicySettingStateSummary](../api/intune-deviceconfig-devicecompliancepolicysettingstatesummary-create.md)|[deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md)|Создание объекта [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).|
|[Удаление объекта deviceCompliancePolicySettingStateSummary](../api/intune-deviceconfig-devicecompliancepolicysettingstatesummary-delete.md)|Нет|Удаляет объект [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).|
|[Обновление объекта deviceCompliancePolicySettingStateSummary](../api/intune-deviceconfig-devicecompliancepolicysettingstatesummary-update.md)|[deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md)|Обновление свойств объекта [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта.|
|setting|String|Имя класса параметров и свойства.|
|settingName|String|Имя параметра.|
|platformType|[policyPlatformType](../resources/intune-deviceconfig-policyplatformtype.md)|Параметр платформы. Возможные значения: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.|
|unknownDeviceCount|Int32|Количество неизвестных устройств.|
|notApplicableDeviceCount|Int32|Количество неприменимых устройств.|
|compliantDeviceCount|Int32|Количество устройств, соответствующих требованиям.|
|remediatedDeviceCount|Int32|Количество исправленных устройств.|
|nonCompliantDeviceCount|Int32|Количество устройств, не соответствующих требованиям.|
|errorDeviceCount|Int32|Количество устройств с ошибками.|
|conflictDeviceCount|Int32|Количество конфликтующих устройств|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|deviceComplianceSettingStates|Коллекция [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md)|Н/Д|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCompliancePolicySettingStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingStateSummary",
  "id": "String (identifier)",
  "setting": "String",
  "settingName": "String",
  "platformType": "String",
  "unknownDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "compliantDeviceCount": 1024,
  "remediatedDeviceCount": 1024,
  "nonCompliantDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "conflictDeviceCount": 1024
}
```



