---
title: Создание userExperienceAnalyticsDevicePerformance
description: Создание нового объекта userExperienceAnalyticsDevicePerformance.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b3632c3e9982a1f9ca37b6af931491ecac4e0974
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58789076"
---
# <a name="create-userexperienceanalyticsdeviceperformance"></a>Создание userExperienceAnalyticsDevicePerformance

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создание нового [объекта userExperienceAnalyticsDevicePerformance.](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementManagedDevices.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Application|DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsDevicePerformance
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для объекта userExperienceAnalyticsDevicePerformance.

В следующей таблице показаны свойства, необходимые при создании пользователяExperienceAnalyticsDevicePerformance.

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор устройства загрузки загрузочного устройства для аналитики пользовательского интерфейса.|
|deviceName|String|Имя устройства аналитики пользовательского интерфейса.|
|model|String|Модель устройства аналитики пользовательских интерфейсов.|
|manufacturer|String|Производитель устройств аналитики пользовательских интерфейсов.|
|diskType|[diskType](../resources/intune-devices-disktype.md)|Тип диска для аналитики пользовательского интерфейса устройства. Возможные значения: `unkown`, `hdd`, `ssd`.|
|operatingSystemVersion|String|Версия операционной системы для аналитики пользовательского интерфейса устройства.|
|bootScore|Int32|Оценка загрузки устройства для аналитики пользовательского интерфейса.|
|coreBootTimeInMs|Int32|Основное время загрузки устройства для аналитики пользовательского интерфейса в миллисекунд.|
|groupPolicyBootTimeInMs|Int32|Время загрузки групповой политики устройств для пользовательского интерфейса в миллисекунд.|
|healthStatus|[userExperienceAnalyticsHealthState](../resources/intune-devices-userexperienceanalyticshealthstate.md)|Состояние здоровья устройства аналитики пользовательского интерфейса. Возможные значения: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.|
|loginScore|Int32|Оценка входа устройства аналитики пользовательского интерфейса.|
|coreLoginTimeInMs|Int32|Время входа основного устройства для аналитики пользовательского интерфейса в миллисекунд.|
|groupPolicyLoginTimeInMs|Int32|Время входа в группу политик пользовательского интерфейса для аналитики устройств в миллисекунд.|
|deviceCount|Int64|Аналитика пользовательских интерфейсов суммирует количество устройств.|
|responsiveDesktopTimeInMs|Int32|Аналитика пользовательского интерфейса реагирует на время рабочего стола в миллисекунд.|
|blueScreenCount|Int32|Количество синих экранов за последние 14 дней. Допустимые значения от 0 до 9999999|
|restartCount|Int32|Количество перезапусков за последние 14 дней. Допустимые значения от 0 до 9999999|
|averageBlueScreens|Двойное с плавающей точкой|Среднее (среднее) число синих экранов на устройство за последние 14 дней. Допустимые значения от 0 до 9999999|
|averageRestarts|Двойное с плавающей точкой|Среднее (среднее) число перезапусков на устройство за последние 14 дней. Допустимые значения от 0 до 9999999|
|startupPerformanceScore|Двойное с плавающей точкой|Оценка производительности запуска устройства для аналитики пользовательского интерфейса. Допустимые значения -1.79769313486232E+308 до 1.797693133486232E+308|
|modelStartupPerformanceScore|Двойное с плавающей точкой|Оценка производительности запуска модели аналитики пользовательской модели. Допустимые значения -1.79769313486232E+308 до 1.797693133486232E+308|



## <a name="response"></a>Отклик
В случае успеха этот метод возвращает код отклика и `201 Created` [объект userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDevicePerformance
Content-type: application/json
Content-length: 739

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDevicePerformance",
  "deviceName": "Device Name value",
  "model": "Model value",
  "manufacturer": "Manufacturer value",
  "diskType": "hdd",
  "operatingSystemVersion": "Operating System Version value",
  "bootScore": 9,
  "coreBootTimeInMs": 0,
  "groupPolicyBootTimeInMs": 7,
  "healthStatus": "insufficientData",
  "loginScore": 10,
  "coreLoginTimeInMs": 1,
  "groupPolicyLoginTimeInMs": 8,
  "deviceCount": 11,
  "responsiveDesktopTimeInMs": 9,
  "blueScreenCount": 15,
  "restartCount": 12,
  "averageBlueScreens": 6.0,
  "averageRestarts": 5.0,
  "startupPerformanceScore": 7.666666666666667,
  "modelStartupPerformanceScore": 9.3333333333333339
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 788

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDevicePerformance",
  "id": "852ae826-e826-852a-26e8-2a8526e82a85",
  "deviceName": "Device Name value",
  "model": "Model value",
  "manufacturer": "Manufacturer value",
  "diskType": "hdd",
  "operatingSystemVersion": "Operating System Version value",
  "bootScore": 9,
  "coreBootTimeInMs": 0,
  "groupPolicyBootTimeInMs": 7,
  "healthStatus": "insufficientData",
  "loginScore": 10,
  "coreLoginTimeInMs": 1,
  "groupPolicyLoginTimeInMs": 8,
  "deviceCount": 11,
  "responsiveDesktopTimeInMs": 9,
  "blueScreenCount": 15,
  "restartCount": 12,
  "averageBlueScreens": 6.0,
  "averageRestarts": 5.0,
  "startupPerformanceScore": 7.666666666666667,
  "modelStartupPerformanceScore": 9.3333333333333339
}
```



