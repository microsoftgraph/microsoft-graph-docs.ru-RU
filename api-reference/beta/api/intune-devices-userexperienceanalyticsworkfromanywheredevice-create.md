---
title: Создание userExperienceAnalyticsWorkFromAnywhereDevice
description: Создание нового объекта userExperienceAnalyticsWorkFromAnywhereDevice.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ecbe4677c288856fa896d0d7d84296a5a941ba82
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2021
ms.locfileid: "61334419"
---
# <a name="create-userexperienceanalyticsworkfromanywheredevice"></a>Создание userExperienceAnalyticsWorkFromAnywhereDevice

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создание нового [объекта userExperienceAnalyticsWorkFromAnywhereDevice.](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementConfiguration.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|DeviceManagementConfiguration.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsWorkFromAnywhereMetrics/{userExperienceAnalyticsWorkFromAnywhereMetricId}/metricDevices
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для объекта userExperienceAnalyticsWorkFromAnywhereDevice.

В следующей таблице показаны свойства, необходимые при создании userExperienceAnalyticsWorkFromAnywhereDevice.

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор аналитики пользовательских интерфейсов работает с любого устройства.|
|deviceId|String|Пользовательский интерфейс работает из любого id устройства.|
|deviceName|String|Работа из любого имени устройства.|
|serialNumber|String|Пользовательский интерфейс работает с любого серийного номера устройства.|
|manufacturer|String|Пользовательский интерфейс работает с любого производителя устройства.|
|model|String|Пользовательский интерфейс работает из любой модели устройства.|
|владение|String|Пользовательский интерфейс работает с любого владельца устройства.|
|managedBy|Строка|Пользовательский интерфейс работает из любого агента управления устройства.|
|autoPilotRegistered|Boolean|Пользовательский интерфейс работает с автопилотом устройства intune.|
|autoPilotProfileAssigned|Boolean|Аналитика пользовательских интерфейсов работает из любого автопилота устройства intuneProfileAssigned.|
|azureAdRegistered|Boolean|Пользовательский интерфейс работает с azureAdRegistered любого устройства.|
|azureAdDeviceId|String|Пользовательский интерфейс работает из любого id-устройства Azure Ad.|
|azureAdJoinType|Строка|Пользовательский опыт работы из любого устройства azure Ad joinType.|
|osDescription|String|Пользовательский интерфейс работает из любого описания ОС устройства.|
|osVersion|String|Пользовательский интерфейс работает из любой версии ОС устройства.|
|tenantAttached|Boolean|Пользовательский интерфейс работает с любого клиента устройстваAttached.|
|compliancePolicySetToIntune|Boolean|Пользовательский интерфейс работает из любой точки устройства compliancePolicySetToIntune.|
|otherWorkloadsSetToIntune|Boolean|Пользовательский интерфейс работает из любого другого устройстваWorkloadsSetToIntune.|
|isCloudManagedGatewayEnabled|Boolean|Работа с пользователем из любого шлюза облачного управления устройства для диспетчера конфигурации включена.|
|upgradeEligibility|[operatingSystemUpgradeEligibility](../resources/intune-devices-operatingsystemupgradeeligibility.md)|Пользовательский опыт работы из любой точки windows обновить состояние приемлемости устройства. Возможные значения: `upgraded`, `unknown`, `notCapable`, `capable`.|
|ramCheckFailed|Boolean|Является ли работа аналитики пользовательского интерфейса из любой точки проверки оборудования оперативной памяти устройства неудачной для устройства для обновления до последней версии windows|
|storageCheckFailed|Boolean|Пользовательский опыт работы с любого устройства, Является ли проверка оборудования хранения не удалось для устройства для обновления до последней версии windows.|
|processorCoreCountCheckFailed|Boolean|Работа пользовательского интерфейса с любого устройства— проверка подсчета ядра процессора не удалось для устройства, чтобы обновиться до последней версии windows.|
|processorSpeedCheckFailed|Boolean|Пользовательский опыт работы с любого устройства, Является ли проверка скорости оборудования процессора не удалось для устройства для обновления до последней версии windows.|
|tpmCheckFailed|Boolean|Работа пользовательского интерфейса с любого устройства — это проверка аппаратного модуля доверенных платформ (TPM) для устройства до последней версии обновления до windows.|
|secureBootCheckFailed|Boolean|Пользовательский опыт работы с любого устройства, является безопасной проверки оборудования загрузки не удалось для устройства для обновления до последней версии windows.|
|processorFamilyCheckFailed|Boolean|Пользовательский опыт работы с любого устройства, является проверка семейства оборудования процессора не удалось для устройства для обновления до последней версии windows.|
|processor64BitCheckFailed|Boolean|Пользовательский опыт работы с любого устройства, является ли проверка архитектуры процессорного оборудования 64-битной не удалось для устройства, чтобы обновить до последней версии windows.|
|osCheckFailed|Boolean|Пользовательский опыт работы с любого устройства, является ли проверка ОС не удалось для устройства для обновления до последней версии windows.|
|workFromAnywhereScore|Double|Пользовательский интерфейс работает из любой точки на устройство общего балла. Допустимые значения -1.79769313486232E+308 до 1.797693133486232E+308|
|WindowsScore|Double|Пользовательский интерфейс работает из любой точки на счет windows устройства. Допустимые значения -1.79769313486232E+308 до 1.797693133486232E+308|
|cloudManagementScore|Double|Пользовательский интерфейс работает из любой точки за оценку облачного управления устройствами. Допустимые значения -1.79769313486232E+308 до 1.797693133486232E+308|
|cloudIdentityScore|Double|Пользовательский опыт работы из любой точки за счет облачного удостоверения устройства. Допустимые значения -1.79769313486232E+308 до 1.797693133486232E+308|
|cloudProvisioningScore|Double|Пользовательский интерфейс работает из любой точки на счет облачного обеспечения устройства. Допустимые значения -1.79769313486232E+308 до 1.797693133486232E+308|
|healthStatus|[userExperienceAnalyticsHealthState](../resources/intune-devices-userexperienceanalyticshealthstate.md)|Пользовательский интерфейс работает из любой точки на состояние здоровья устройства. Возможные значения: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.|



## <a name="response"></a>Отклик
В случае успеха этот метод возвращает код отклика и `201 Created` [объект userExperienceAnalyticsWorkFromAnywhereDevice](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsWorkFromAnywhereMetrics/{userExperienceAnalyticsWorkFromAnywhereMetricId}/metricDevices
Content-type: application/json
Content-length: 1323

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsWorkFromAnywhereDevice",
  "deviceId": "Device Id value",
  "deviceName": "Device Name value",
  "serialNumber": "Serial Number value",
  "manufacturer": "Manufacturer value",
  "model": "Model value",
  "ownership": "Ownership value",
  "managedBy": "Managed By value",
  "autoPilotRegistered": true,
  "autoPilotProfileAssigned": true,
  "azureAdRegistered": true,
  "azureAdDeviceId": "Azure Ad Device Id value",
  "azureAdJoinType": "Azure Ad Join Type value",
  "osDescription": "Os Description value",
  "osVersion": "Os Version value",
  "tenantAttached": true,
  "compliancePolicySetToIntune": true,
  "otherWorkloadsSetToIntune": true,
  "isCloudManagedGatewayEnabled": true,
  "upgradeEligibility": "unknown",
  "ramCheckFailed": true,
  "storageCheckFailed": true,
  "processorCoreCountCheckFailed": true,
  "processorSpeedCheckFailed": true,
  "tpmCheckFailed": true,
  "secureBootCheckFailed": true,
  "processorFamilyCheckFailed": true,
  "processor64BitCheckFailed": true,
  "osCheckFailed": true,
  "workFromAnywhereScore": 7.0,
  "windowsScore": 4.0,
  "cloudManagementScore": 6.666666666666667,
  "cloudIdentityScore": 6.0,
  "cloudProvisioningScore": 7.333333333333333,
  "healthStatus": "insufficientData"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1372

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsWorkFromAnywhereDevice",
  "id": "83d5adfc-adfc-83d5-fcad-d583fcadd583",
  "deviceId": "Device Id value",
  "deviceName": "Device Name value",
  "serialNumber": "Serial Number value",
  "manufacturer": "Manufacturer value",
  "model": "Model value",
  "ownership": "Ownership value",
  "managedBy": "Managed By value",
  "autoPilotRegistered": true,
  "autoPilotProfileAssigned": true,
  "azureAdRegistered": true,
  "azureAdDeviceId": "Azure Ad Device Id value",
  "azureAdJoinType": "Azure Ad Join Type value",
  "osDescription": "Os Description value",
  "osVersion": "Os Version value",
  "tenantAttached": true,
  "compliancePolicySetToIntune": true,
  "otherWorkloadsSetToIntune": true,
  "isCloudManagedGatewayEnabled": true,
  "upgradeEligibility": "unknown",
  "ramCheckFailed": true,
  "storageCheckFailed": true,
  "processorCoreCountCheckFailed": true,
  "processorSpeedCheckFailed": true,
  "tpmCheckFailed": true,
  "secureBootCheckFailed": true,
  "processorFamilyCheckFailed": true,
  "processor64BitCheckFailed": true,
  "osCheckFailed": true,
  "workFromAnywhereScore": 7.0,
  "windowsScore": 4.0,
  "cloudManagementScore": 6.666666666666667,
  "cloudIdentityScore": 6.0,
  "cloudProvisioningScore": 7.333333333333333,
  "healthStatus": "insufficientData"
}
```




