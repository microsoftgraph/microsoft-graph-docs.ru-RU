---
title: Создание Усерекспериенцеаналитиксдевицестартуфистори
description: Создание нового объекта Усерекспериенцеаналитиксдевицестартуфистори.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 33ed2485f87be0687ade81e51a64f495bfc5f9ed
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49234298"
---
# <a name="create-userexperienceanalyticsdevicestartuphistory"></a>Создание Усерекспериенцеаналитиксдевицестартуфистори

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создание нового объекта [усерекспериенцеаналитиксдевицестартуфистори](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) .

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementManagedDevices.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsDeviceStartupHistory
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление объекта Усерекспериенцеаналитиксдевицестартуфистори в формате JSON.

В следующей таблице приведены свойства, необходимые при создании Усерекспериенцеаналитиксдевицестартуфистори.

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор журнала запуска устройства Analytics User Experience.|
|deviceId|String|Идентификатор устройства службы аналитики взаимодействия с пользователем.|
|startTime|DateTimeOffset|Время начала загрузки устройства Analytics User Experience.|
|коребуттимеинмс|Int32|Время загрузки ядра устройства аналитики для пользователя (в миллисекундах).|
|граупполицибуттимеинмс|Int32|Время загрузки групповой политики устройства Analytics для пользователя (в миллисекундах).|
|феатуреупдатебуттимеинмс|Int32|Время обновления компонента службы аналитики взаимодействия с пользователем (в миллисекундах).|
|тоталбуттимеинмс|Int32|Общее время загрузки устройства Analytics User Experience (в миллисекундах).|
|граупполицилогинтимеинмс|Int32|Время входа в групповую политику устройства Analytics User Experience (в миллисекундах).|
|корелогинтимеинмс|Int32|Время входа в ядро устройства аналитики взаимодействия с пользователем (в миллисекундах).|
|респонсиведесктоптимеинмс|Int32|Время, в течение которого выполняется анализ пользовательского интерфейса на рабочем столе в миллисекундах.|
|тоталлогинтимеинмс|Int32|Общее время входа в систему для устройства аналитики взаимодействия с пользователем (в миллисекундах).|
|исфирстлогин|Boolean|Первое имя входа устройства Analytics User Experience.|
|исфеатуреупдате|Boolean|Загрузочная запись устройства аналитики взаимодействия с пользователем — это обновление компонентов.|
|operatingSystemVersion|String|Версия операционной системы для записи загрузки устройства службы аналитики взаимодействия с пользователем.|
|рестарткатегори|[userExperienceAnalyticsOperatingSystemRestartCategory](../resources/intune-devices-userexperienceanalyticsoperatingsystemrestartcategory.md)|Категория перезагрузки ОС. Возможные значения: `unknown`, `restartWithUpdate`, `restartWithoutUpdate`, `blueScreen`, `shutdownWithUpdate`, `shutdownWithoutUpdate`, `longPowerButtonPress`, `bootError`.|
|рестартстопкоде|String|Код остановки перезапуска ОС. Здесь показан код проверки ошибки, который можно использовать для поиска причины синего экрана.|
|рестартфаултбуккет|String|Сегмент сбоя при перезапуске ОС. Блок сбоя используется для поиска дополнительных сведений о сбое системы.|



## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [усерекспериенцеаналитиксдевицестартуфистори](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDeviceStartupHistory
Content-type: application/json
Content-length: 680

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceStartupHistory",
  "deviceId": "Device Id value",
  "startTime": "2017-01-01T00:03:29.2730865-08:00",
  "coreBootTimeInMs": 0,
  "groupPolicyBootTimeInMs": 7,
  "featureUpdateBootTimeInMs": 9,
  "totalBootTimeInMs": 1,
  "groupPolicyLoginTimeInMs": 8,
  "coreLoginTimeInMs": 1,
  "responsiveDesktopTimeInMs": 9,
  "totalLoginTimeInMs": 2,
  "isFirstLogin": true,
  "isFeatureUpdate": true,
  "operatingSystemVersion": "Operating System Version value",
  "restartCategory": "restartWithUpdate",
  "restartStopCode": "Restart Stop Code value",
  "restartFaultBucket": "Restart Fault Bucket value"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 729

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceStartupHistory",
  "id": "13357123-7123-1335-2371-351323713513",
  "deviceId": "Device Id value",
  "startTime": "2017-01-01T00:03:29.2730865-08:00",
  "coreBootTimeInMs": 0,
  "groupPolicyBootTimeInMs": 7,
  "featureUpdateBootTimeInMs": 9,
  "totalBootTimeInMs": 1,
  "groupPolicyLoginTimeInMs": 8,
  "coreLoginTimeInMs": 1,
  "responsiveDesktopTimeInMs": 9,
  "totalLoginTimeInMs": 2,
  "isFirstLogin": true,
  "isFeatureUpdate": true,
  "operatingSystemVersion": "Operating System Version value",
  "restartCategory": "restartWithUpdate",
  "restartStopCode": "Restart Stop Code value",
  "restartFaultBucket": "Restart Fault Bucket value"
}
```




