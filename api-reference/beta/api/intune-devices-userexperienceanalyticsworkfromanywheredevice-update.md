---
title: Обновление userExperienceAnalyticsWorkFromAnywhereDevice
description: Обновление свойств объекта userExperienceAnalyticsWorkFromAnywhereDevice.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f2dfdfd64aa892ce5668ddd267a4f20ece31e4a9
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59058994"
---
# <a name="update-userexperienceanalyticsworkfromanywheredevice"></a>Обновление userExperienceAnalyticsWorkFromAnywhereDevice

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [userExperienceAnalyticsWorkFromAnywhereDevice.](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementManagedDevices.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsWorkFromAnywhereMetrics/{userExperienceAnalyticsWorkFromAnywhereMetricId}/metricDevices/{userExperienceAnalyticsWorkFromAnywhereDeviceId}
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для [объекта userExperienceAnalyticsWorkFromAnywhereDevice.](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md)

В следующей таблице показаны свойства, необходимые при создании [userExperienceAnalyticsWorkFromAnywhereDevice.](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор аналитики пользовательских интерфейсов работает с любого устройства.|
|deviceName|String|Работа из любого имени устройства.|
|serialNumber|String|Пользовательский интерфейс работает с любого серийного номера устройства.|
|manufacturer|String|Пользовательский интерфейс работает с любого производителя устройства.|
|model|String|Пользовательский интерфейс работает из любой модели устройства.|
|владение|String|Пользовательский интерфейс работает с любого владельца устройства.|
|managedBy|Строка|Пользовательский интерфейс работает из любого агента управления устройства.|
|autoPilotRegistered|Логический|Пользовательский интерфейс работает с автопилотом устройства intune.|
|autoPilotProfileAssigned|Логический|Аналитика пользовательских интерфейсов работает из любого автопилота устройства intuneProfileAssigned.|
|azureAdRegistered|Логический|Пользовательский интерфейс работает с azureAdRegistered любого устройства.|
|azureAdDeviceId|Строка|Пользовательский интерфейс работает из любого id-устройства Azure Ad.|
|azureAdJoinType|Строка|Пользовательский опыт работы из любого устройства azure Ad joinType.|
|osDescription|String|Пользовательский интерфейс работает из любого описания ОС устройства.|
|osVersion|String|Пользовательский интерфейс работает из любой версии ОС устройства.|
|tenantAttached|Логический|Пользовательский интерфейс работает с любого клиента устройстваAttached.|
|compliancePolicySetToIntune|Логический|Пользовательский интерфейс работает из любой точки устройства compliancePolicySetToIntune.|
|otherWorkloadsSetToIntune|Boolean|Пользовательский интерфейс работает из любого другого устройстваWorkloadsSetToIntune.|
|upgradeEligibility|[operatingSystemUpgradeEligibility](../resources/intune-devices-operatingsystemupgradeeligibility.md)|Пользовательский опыт работы из любой точки windows обновить состояние приемлемости устройства. Возможные значения: `upgraded`, `unknown`, `notCapable`, `capable`.|
|ramCheckFailed|Boolean|Является ли работа аналитики пользовательского интерфейса из любой точки проверки оборудования оперативной памяти устройства неудачной для устройства для обновления до последней версии windows|
|storageCheckFailed|Boolean|Пользовательский опыт работы с любого устройства, Является ли проверка оборудования хранения не удалось для устройства для обновления до последней версии windows.|
|processorCoreCountCheckFailed|Логический|Работа пользовательского интерфейса с любого устройства— проверка подсчета ядра процессора не удалось для устройства, чтобы обновиться до последней версии windows.|
|processorSpeedCheckFailed|Логический|Пользовательский опыт работы с любого устройства, Является ли проверка скорости оборудования процессора не удалось для устройства для обновления до последней версии windows.|
|tpmCheckFailed|Логический|Работа пользовательского интерфейса с любого устройства — это проверка аппаратного модуля доверенных платформ (TPM) для устройства до последней версии обновления до windows.|
|secureBootCheckFailed|Логический|Пользовательский опыт работы с любого устройства, является безопасной проверки оборудования загрузки не удалось для устройства для обновления до последней версии windows.|
|processorFamilyCheckFailed|Логический|Пользовательский опыт работы с любого устройства, является проверка семейства оборудования процессора не удалось для устройства для обновления до последней версии windows.|
|processor64BitCheckFailed|Boolean|Пользовательский опыт работы с любого устройства, является ли проверка архитектуры процессорного оборудования 64-битной не удалось для устройства, чтобы обновить до последней версии windows.|
|osCheckFailed|Логический|Пользовательский опыт работы с любого устройства, является ли проверка ОС не удалось для устройства для обновления до последней версии windows.|
|WindowsScore|Двойное с плавающей точкой|Пользовательский интерфейс работает из любой точки на счет windows устройства. Допустимые значения -1.79769313486232E+308 до 1.797693133486232E+308|
|cloudManagementScore|Двойное с плавающей точкой|Пользовательский интерфейс работает из любой точки за оценку облачного управления устройствами. Допустимые значения -1.79769313486232E+308 до 1.797693133486232E+308|
|cloudIdentityScore|Двойное с плавающей точкой|Пользовательский опыт работы из любой точки за счет облачного удостоверения устройства. Допустимые значения -1.79769313486232E+308 до 1.797693133486232E+308|
|cloudProvisioningScore|Двойное с плавающей точкой|Пользовательский интерфейс работает из любой точки на счет облачного обеспечения устройства. Допустимые значения -1.79769313486232E+308 до 1.797693133486232E+308|
|healthStatus|[userExperienceAnalyticsHealthState](../resources/intune-devices-userexperienceanalyticshealthstate.md)|Пользовательский интерфейс работает из любой точки на состояние здоровья устройства. Возможные значения: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.|



## <a name="response"></a>Отклик
В случае успеха этот метод возвращает код ответа и обновленный объект `200 OK` [userExperienceAnalyticsWorkFromAnywhereDevice](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsWorkFromAnywhereMetrics/{userExperienceAnalyticsWorkFromAnywhereMetricId}/metricDevices/{userExperienceAnalyticsWorkFromAnywhereDeviceId}
Content-type: application/json
Content-length: 1215

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsWorkFromAnywhereDevice",
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
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1264

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsWorkFromAnywhereDevice",
  "id": "83d5adfc-adfc-83d5-fcad-d583fcadd583",
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
  "windowsScore": 4.0,
  "cloudManagementScore": 6.666666666666667,
  "cloudIdentityScore": 6.0,
  "cloudProvisioningScore": 7.333333333333333,
  "healthStatus": "insufficientData"
}
```



