---
title: Обновление userExperienceAnalyticsResourcePerformance
description: Обновление свойств объекта userExperienceAnalyticsResourcePerformance.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b5ca79e7870893e9748ea93222e96ade36649e6e
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51135917"
---
# <a name="update-userexperienceanalyticsresourceperformance"></a>Обновление userExperienceAnalyticsResourcePerformance

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [userExperienceAnalyticsResourcePerformance.](../resources/intune-devices-userexperienceanalyticsresourceperformance.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированное (рабочая или учебная учетная запись)|DeviceManagementManagedDevices.ReadWrite.All|
|Делегированное (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsResourcePerformance/{userExperienceAnalyticsResourcePerformanceId}
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для [объекта userExperienceAnalyticsResourcePerformance.](../resources/intune-devices-userexperienceanalyticsresourceperformance.md)

В следующей таблице показаны свойства, необходимые при создании [userExperienceAnalyticsResourcePerformance.](../resources/intune-devices-userexperienceanalyticsresourceperformance.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор сущности производительности ресурсов аналитики пользовательских интерфейсов.|
|deviceId|String|ID устройства.|
|deviceName|String|Имя устройства.|
|model|String|Модель устройства аналитики пользовательских интерфейсов.|
|deviceCount|Int64|Аналитика пользовательских интерфейсов суммирует количество устройств.|
|manufacturer|String|Производитель устройств аналитики пользовательских интерфейсов.|
|cpuSpikeTimePercentage|Двойное с плавающей точкой|Время пика ЦП в процентах. Допустимые значения: от 0 до 100|
|ramSpikeTimePercentage|Двойное с плавающей точкой|Время пика оперативной памяти в процентах. Допустимые значения: от 0 до 100|
|cpuSpikeTimeScore|Int32|Оценка времени пика пика ЦП для пользовательского интерфейса. Допустимые значения: от 0 до 100|
|cpuSpikeTimePercentageThreshold|Двойное с плавающей точкой|Порог cpuSpikeTimeScore. Допустимые значения: от 0 до 100|
|ramSpikeTimeScore|Int32|Оценка времени пика пика оперативной памяти устройства аналитики пользовательского интерфейса. Допустимые значения: от 0 до 100|
|ramSpikeTimePercentageThreshold|Двойное с плавающей точкой|Порог ramSpikeTimeScore. Допустимые значения: от 0 до 100|
|deviceResourcePerformanceScore|Int32|Оценка производительности ресурсов определенного устройства. Допустимые значения: от 0 до 100|



## <a name="response"></a>Отклик
В случае успеха этот метод возвращает код ответа и обновленный объект `200 OK` [userExperienceAnalyticsResourcePerformance](../resources/intune-devices-userexperienceanalyticsresourceperformance.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsResourcePerformance/{userExperienceAnalyticsResourcePerformanceId}
Content-type: application/json
Content-length: 553

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsResourcePerformance",
  "deviceId": "Device Id value",
  "deviceName": "Device Name value",
  "model": "Model value",
  "deviceCount": 11,
  "manufacturer": "Manufacturer value",
  "cpuSpikeTimePercentage": 7.333333333333333,
  "ramSpikeTimePercentage": 7.333333333333333,
  "cpuSpikeTimeScore": 1,
  "cpuSpikeTimePercentageThreshold": 10.333333333333334,
  "ramSpikeTimeScore": 1,
  "ramSpikeTimePercentageThreshold": 10.333333333333334,
  "deviceResourcePerformanceScore": 14
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 602

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsResourcePerformance",
  "id": "d34d78e8-78e8-d34d-e878-4dd3e8784dd3",
  "deviceId": "Device Id value",
  "deviceName": "Device Name value",
  "model": "Model value",
  "deviceCount": 11,
  "manufacturer": "Manufacturer value",
  "cpuSpikeTimePercentage": 7.333333333333333,
  "ramSpikeTimePercentage": 7.333333333333333,
  "cpuSpikeTimeScore": 1,
  "cpuSpikeTimePercentageThreshold": 10.333333333333334,
  "ramSpikeTimeScore": 1,
  "ramSpikeTimePercentageThreshold": 10.333333333333334,
  "deviceResourcePerformanceScore": 14
}
```




