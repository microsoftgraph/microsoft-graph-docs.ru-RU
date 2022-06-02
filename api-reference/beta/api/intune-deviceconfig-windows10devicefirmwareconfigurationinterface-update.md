---
title: Обновление windows10DeviceFirmwareConfigurationInterface
description: Обновление свойств объекта windows10DeviceFirmwareConfigurationInterface.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3ddad8672e784fdc5328e0b7f7d60e51a2d5e811
ms.sourcegitcommit: 435d70e7adb27e6cedaf485ebfdab7c3ef9ffacf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/02/2022
ms.locfileid: "65857437"
---
# <a name="update-windows10devicefirmwareconfigurationinterface"></a>Обновление windows10DeviceFirmwareConfigurationInterface

Пространство имен: microsoft.graph

> **Важно:** API Graph Майкрософт в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md) .

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированное (рабочая или учебная учетная запись)|DeviceManagementConfiguration.ReadWrite.All|
|Делегированное (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса добавьте представление объекта [windows10DeviceFirmwareConfigurationInterface в формате](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md) JSON.

В следующей таблице показаны свойства, необходимые при создании [объекта windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|Идентификаторы roleScopeTagId|Коллекция String|Список тегов области для этого экземпляра сущности. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|supportsScopeTags|Boolean|Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области. Назначение свойству ScopeTags не допускается, если это значение имеет значение false и сущности не будут видны пользователям с заданной областью. Это происходит для устаревших политик, созданных в Silverlight, и их можно устранить, удалив и повторно создав политику на портале Azure. Это свойство доступно только для чтения. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|Применимость выпуска ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|Правило применимости версии ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|Правило применимости режима устройства для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|description|Строка|Указанное администратором описание конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|displayName|String|Указанное администратором имя конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|version|Int32|Версия конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|changeUefiSettingsPermission|[changeUefiSettingsPermission](../resources/intune-deviceconfig-changeuefisettingspermission.md)|Определяет уровень разрешений, предоставленный пользователям для изменения параметров UEFI. Возможные значения: `notConfiguredOnly`, `none`.|
|virtualizationOfCpuAndIO|[Включения](../resources/intune-shared-enablement.md)|Определяет, включена ли виртуализация ЦП и ввода-вывода. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|Камеры|[Включения](../resources/intune-shared-enablement.md)|Определяет, включены ли встроенные камеры. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|microphonesAndSpeakers|[Включения](../resources/intune-shared-enablement.md)|Определяет, включены ли встроенные микрофоны или динамики. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|Радио|[Включения](../resources/intune-shared-enablement.md)|Определяет, включены ли встроенные радио, например WIFI, NFC, Bluetooth. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|bootFromExternalMedia|[Включения](../resources/intune-shared-enablement.md)|Определяет, разрешена ли пользователю загрузка с внешнего носителя. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|bootFromBuiltInNetworkAdapters|[Включения](../resources/intune-shared-enablement.md)|Определяет, разрешена ли пользователю загрузка из встроенных сетевых адаптеров. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|windowsPlatformBinaryTable|[Включения](../resources/intune-shared-enablement.md)|Определяет, разрешено ли пользователю включить двоичную таблицу Windows платформы. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|simultaneousMultiThreading|[Включения](../resources/intune-shared-enablement.md)|Определяет, разрешено ли пользователю включить одновременную многопоточность. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|frontCamera|[Включения](../resources/intune-shared-enablement.md)|Определяет, разрешено ли пользователю включить front Камера. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|rearCamera|[Включения](../resources/intune-shared-enablement.md)|Определяет, разрешено ли пользователю включить задняя камера. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|инфракрасная камеры|[Включения](../resources/intune-shared-enablement.md)|Определяет, разрешено ли пользователю включить инфракрасную камеру. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|Микрофон|[Включения](../resources/intune-shared-enablement.md)|Определяет, разрешено ли пользователю включить микрофон. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|Bluetooth|[Включения](../resources/intune-shared-enablement.md)|Определяет, разрешено ли пользователю включить Bluetooth. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|wirelessWideAreaNetwork|[Включения](../resources/intune-shared-enablement.md)|Определяет, разрешено ли пользователю включить беспроводную сеть с широкими областями. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|nearFieldCommunication|[Включения](../resources/intune-shared-enablement.md)|Определяет, разрешено ли пользователю включить связь с полями, близкого к полю. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|Wifi|[Включения](../resources/intune-shared-enablement.md)|Определяет, разрешено ли пользователю включить Wi-Fi. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|usbTypeAPort|[Включения](../resources/intune-shared-enablement.md)|Определяет, разрешено ли пользователю включить порт USB типа A. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|Sdcard|[Включения](../resources/intune-shared-enablement.md)|Определяет, разрешено ли пользователю включить порт SD Card. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|wakeOnLAN|[Включения](../resources/intune-shared-enablement.md)|Определяет, разрешено ли пользователю включить пробуждение по локальной сети. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|wakeOnPower|[Включения](../resources/intune-shared-enablement.md)|Определяет, разрешено ли пользователю включить wake On Power. Возможные значения: `notConfigured`, `enabled`, `disabled`.|



## <a name="response"></a>Отклик
В случае успешного `200 OK` выполнения этот метод возвращает код отклика и обновленный объект [windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md) в теле отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1754

{
  "@odata.type": "#microsoft.graph.windows10DeviceFirmwareConfigurationInterface",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "changeUefiSettingsPermission": "none",
  "virtualizationOfCpuAndIO": "enabled",
  "cameras": "enabled",
  "microphonesAndSpeakers": "enabled",
  "radios": "enabled",
  "bootFromExternalMedia": "enabled",
  "bootFromBuiltInNetworkAdapters": "enabled",
  "windowsPlatformBinaryTable": "enabled",
  "simultaneousMultiThreading": "enabled",
  "frontCamera": "enabled",
  "rearCamera": "enabled",
  "infraredCamera": "enabled",
  "microphone": "enabled",
  "bluetooth": "enabled",
  "wirelessWideAreaNetwork": "enabled",
  "nearFieldCommunication": "enabled",
  "wiFi": "enabled",
  "usbTypeAPort": "enabled",
  "sdCard": "enabled",
  "wakeOnLAN": "enabled",
  "wakeOnPower": "enabled"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1926

{
  "@odata.type": "#microsoft.graph.windows10DeviceFirmwareConfigurationInterface",
  "id": "96474363-4363-9647-6343-479663434796",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "changeUefiSettingsPermission": "none",
  "virtualizationOfCpuAndIO": "enabled",
  "cameras": "enabled",
  "microphonesAndSpeakers": "enabled",
  "radios": "enabled",
  "bootFromExternalMedia": "enabled",
  "bootFromBuiltInNetworkAdapters": "enabled",
  "windowsPlatformBinaryTable": "enabled",
  "simultaneousMultiThreading": "enabled",
  "frontCamera": "enabled",
  "rearCamera": "enabled",
  "infraredCamera": "enabled",
  "microphone": "enabled",
  "bluetooth": "enabled",
  "wirelessWideAreaNetwork": "enabled",
  "nearFieldCommunication": "enabled",
  "wiFi": "enabled",
  "usbTypeAPort": "enabled",
  "sdCard": "enabled",
  "wakeOnLAN": "enabled",
  "wakeOnPower": "enabled"
}
```




