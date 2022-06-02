---
title: Создание объекта userExperienceAnalyticsBatteryHealthModelPerformance
description: Создайте объект userExperienceAnalyticsBatteryHealthModelPerformance.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cbe1f1ff409c602ccf578003ee0bf75a8a5b73a8
ms.sourcegitcommit: 435d70e7adb27e6cedaf485ebfdab7c3ef9ffacf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/02/2022
ms.locfileid: "65857822"
---
# <a name="create-userexperienceanalyticsbatteryhealthmodelperformance"></a>Создание объекта userExperienceAnalyticsBatteryHealthModelPerformance

Пространство имен: microsoft.graph

> **Важно:** API Graph Майкрософт в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создайте объект [userExperienceAnalyticsBatteryHealthModelPerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance.md) .

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированное (рабочая или учебная учетная запись)|DeviceManagementConfiguration.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All|
|Делегированное (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|DeviceManagementConfiguration.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsBatteryHealthModelPerformance
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление объекта userExperienceAnalyticsBatteryHealthModelPerformance в формате JSON.

В следующей таблице показаны свойства, необходимые при создании объекта userExperienceAnalyticsBatteryHealthModelPerformance.

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор объекта производительности модели работоспособности батареи аналитики пользовательского интерфейса.|
|activeDevices|Int32|Количество активных устройств для этой модели. Допустимые значения — 2147483648 2147483647|
|model|String|Имя модели устройства.|
|manufacturer|String|Имя производителя устройства.|
|averageMaxCapacityPercentage|Int32|Среднее значение максимальной емкости для всех устройств данной модели. Максимальная емкость измеряет полную стоимость и емкость конструктора для аккумуляторов устройства. Допустимые значения — 2147483648 2147483647|
|averageEstimatedRuntimeInMinutes|Int32|Среднее значение предполагаемых сред выполнения при полной оплате для всех устройств данной модели. Единица в минутах. Допустимые значения — 2147483648 2147483647|
|averageBatteryAgeInDays|Int32|Среднее время заряда батареи для всех устройств данной модели в клиенте. Единица в днях. Допустимые значения — 2147483648 2147483647|
|modelBatteryHealthScore|Int32|Взвешенного среднего значения максимальной оценки емкости модели и оценки времени выполнения. Значения в диапазоне от 0 до 100. Допустимые значения — 2147483648 2147483647|



## <a name="response"></a>Отклик
В случае успешного выполнения `201 Created` этот метод возвращает код отклика и объект [userExperienceAnalyticsBatteryHealthModelPerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsBatteryHealthModelPerformance
Content-type: application/json
Content-length: 333

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBatteryHealthModelPerformance",
  "activeDevices": 13,
  "model": "Model value",
  "manufacturer": "Manufacturer value",
  "averageMaxCapacityPercentage": 12,
  "averageEstimatedRuntimeInMinutes": 0,
  "averageBatteryAgeInDays": 7,
  "modelBatteryHealthScore": 7
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 382

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBatteryHealthModelPerformance",
  "id": "0850afa4-afa4-0850-a4af-5008a4af5008",
  "activeDevices": 13,
  "model": "Model value",
  "manufacturer": "Manufacturer value",
  "averageMaxCapacityPercentage": 12,
  "averageEstimatedRuntimeInMinutes": 0,
  "averageBatteryAgeInDays": 7,
  "modelBatteryHealthScore": 7
}
```




