---
title: Создание userExperienceAnalyticsResourcePerformance
description: Создание объекта userExperienceAnalyticsResourcePerformance.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b35601c4ad92313d910d4813ac8ace84c4fce9da
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50162516"
---
# <a name="create-userexperienceanalyticsresourceperformance"></a>Создание userExperienceAnalyticsResourcePerformance

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создание объекта [userExperienceAnalyticsResourcePerformance.](../resources/intune-devices-userexperienceanalyticsresourceperformance.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
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
POST /deviceManagement/userExperienceAnalyticsResourcePerformance
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса укажу представление объекта userExperienceAnalyticsResourcePerformance в JSON.

В следующей таблице показаны свойства, необходимые при создании объекта userExperienceAnalyticsResourcePerformance.

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор сущности производительности ресурсов аналитики пользовательского интерфейса.|
|deviceId|String|ИД устройства.|
|deviceName|String|Имя устройства.|
|model|String|Модель устройства аналитики пользовательского интерфейса.|
|deviceCount|Int64|Аналитика пользовательского интерфейса суммирует количество устройств.|
|manufacturer|String|Изготовитель устройства аналитики пользовательского интерфейса.|
|cpuSpikeTimePercentage|Двойное с плавающей точкой|Время пика ЦП в процентах. Допустимые значения: от 0 до 100|
|ramSpikeTimePercentage|Двойное с плавающей точкой|Время пика ОЗУ в процентах. Допустимые значения: от 0 до 100|
|cpuSpikeTimeScore|Int32|Оценка времени пика пика ЦП устройства аналитики пользовательского интерфейса. Допустимые значения: от 0 до 100|
|cpuSpikeTimePercentageThreshold|Двойное с плавающей точкой|Пороговое значение cpuSpikeTimeScore. Допустимые значения: от 0 до 100|
|ramSpikeTimeScore|Int32|Показатель времени пика пика ОЗУ устройства аналитики пользовательского интерфейса. Допустимые значения: от 0 до 100|
|ramSpikeTimePercentageThreshold|Двойное с плавающей точкой|Пороговое значение ramSpikeTimeScore. Допустимые значения: от 0 до 100|
|deviceResourcePerformanceScore|Int32|Оценка производительности ресурсов для конкретного устройства. Допустимые значения: от 0 до 100|



## <a name="response"></a>Отклик
В случае успеха этот метод возвращает код отклика и объект `201 Created` [userExperienceAnalyticsResourcePerformance](../resources/intune-devices-userexperienceanalyticsresourceperformance.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsResourcePerformance
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
HTTP/1.1 201 Created
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




