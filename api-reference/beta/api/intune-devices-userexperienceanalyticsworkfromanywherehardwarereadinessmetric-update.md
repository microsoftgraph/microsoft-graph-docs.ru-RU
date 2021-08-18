---
title: Обновление userExperienceAnalyticsWorkFromAnywhereHardwareReadinessMetric
description: Обновление свойств объекта userExperienceAnalyticsWorkFromAnywhereHardwareReadinessMetric.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 473c01d8c59912bc88880aaff42fe105b35ba234
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58265672"
---
# <a name="update-userexperienceanalyticsworkfromanywherehardwarereadinessmetric"></a>Обновление userExperienceAnalyticsWorkFromAnywhereHardwareReadinessMetric

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [userExperienceAnalyticsWorkFromAnywhereHardwareReadinessMetric.](../resources/intune-devices-userexperienceanalyticsworkfromanywherehardwarereadinessmetric.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsWorkFromAnywhereHardwareReadinessMetric
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для [объекта userExperienceAnalyticsWorkFromAnywhereHardwareReadinessMetric.](../resources/intune-devices-userexperienceanalyticsworkfromanywherehardwarereadinessmetric.md)

В следующей таблице показаны свойства, необходимые при создании [userExperienceAnalyticsWorkFromAnywhereHardwareReadinessMetric.](../resources/intune-devices-userexperienceanalyticsworkfromanywherehardwarereadinessmetric.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор объекта метрики готовности оборудования для аналитики пользовательского интерфейса.|
|totalDeviceCount|Int32|Общее количество устройств в организации. Допустимые значения 2147483648 2147483647|
|upgradeEligibleDeviceCount|Int32|Количество устройств в организации, имеющих право на обновление Windows. Допустимые значения 2147483648 2147483647|
|ramCheckFailedPercentage|Двойное с плавающей точкой|Процент устройств, для которых проверка оборудования оперативной памяти не удалась. Допустимые значения -1.79769313486232E+308 до 1.797693133486232E+308|
|storageCheckFailedPercentage|Двойное с плавающей точкой|Процент устройств, для которых проверка оборудования хранения не удалась. Допустимые значения -1.79769313486232E+308 до 1.797693133486232E+308|
|processorCoreCountCheckFailedPercentage|Двойное с плавающей точкой|Процент устройств, для которых проверка подсчета ядра процессорного оборудования не удалось. Допустимые значения -1.79769313486232E+308 до 1.797693133486232E+308|
|processorSpeedCheckFailedPercentage|Двойное с плавающей точкой|Процент устройств, для которых проверка скорости работы процессорного оборудования не удалось. Допустимые значения -1.79769313486232E+308 до 1.797693133486232E+308|
|tpmCheckFailedPercentage|Двойное с плавающей точкой|Процент устройств, для которых проверка аппаратного модуля доверенных платформ (TPM) не удалось. Допустимые значения -1.79769313486232E+308 до 1.797693133486232E+308|
|secureBootCheckFailedPercentage|Двойное с плавающей точкой|Процент устройств, для которых не удалось проверить безопасное оборудование загрузки. Допустимые значения -1.79769313486232E+308 до 1.797693133486232E+308|
|processorFamilyCheckFailedPercentage|Двойное с плавающей точкой|Процент устройств, для которых семейная проверка оборудования обработчика не удалось. Допустимые значения -1.79769313486232E+308 до 1.797693133486232E+308|
|processor64BitCheckFailedPercentage|Двойное с плавающей точкой|Процент устройств, для которых проверка архитектуры процессорного оборудования 64-битной архитектуры не удалось. Допустимые значения -1.79769313486232E+308 до 1.797693133486232E+308|
|osCheckFailedPercentage|Двойное с плавающей точкой|Процент устройств, для которых проверка ОС не удалась. Допустимые значения -1.79769313486232E+308 до 1.797693133486232E+308|



## <a name="response"></a>Отклик
В случае успеха этот метод возвращает код ответа и обновленный объект `200 OK` [userExperienceAnalyticsWorkFromAnywhereHardwareReadinessMetric](../resources/intune-devices-userexperienceanalyticsworkfromanywherehardwarereadinessmetric.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsWorkFromAnywhereHardwareReadinessMetric
Content-type: application/json
Content-length: 626

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsWorkFromAnywhereHardwareReadinessMetric",
  "totalDeviceCount": 0,
  "upgradeEligibleDeviceCount": 10,
  "ramCheckFailedPercentage": 8.0,
  "storageCheckFailedPercentage": 9.3333333333333339,
  "processorCoreCountCheckFailedPercentage": 13.0,
  "processorSpeedCheckFailedPercentage": 11.666666666666666,
  "tpmCheckFailedPercentage": 8.0,
  "secureBootCheckFailedPercentage": 10.333333333333334,
  "processorFamilyCheckFailedPercentage": 12.0,
  "processor64BitCheckFailedPercentage": 11.666666666666666,
  "osCheckFailedPercentage": 7.666666666666667
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 675

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsWorkFromAnywhereHardwareReadinessMetric",
  "id": "6df21a06-1a06-6df2-061a-f26d061af26d",
  "totalDeviceCount": 0,
  "upgradeEligibleDeviceCount": 10,
  "ramCheckFailedPercentage": 8.0,
  "storageCheckFailedPercentage": 9.3333333333333339,
  "processorCoreCountCheckFailedPercentage": 13.0,
  "processorSpeedCheckFailedPercentage": 11.666666666666666,
  "tpmCheckFailedPercentage": 8.0,
  "secureBootCheckFailedPercentage": 10.333333333333334,
  "processorFamilyCheckFailedPercentage": 12.0,
  "processor64BitCheckFailedPercentage": 11.666666666666666,
  "osCheckFailedPercentage": 7.666666666666667
}
```




