---
title: Обновление Усерекспериенцеаналитиксметрик
description: Обновление свойств объекта Усерекспериенцеаналитиксметрик.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e30b55ec0cb1bb015a01f8864b4095c67a20f5e6
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43379194"
---
# <a name="update-userexperienceanalyticsmetric"></a>Обновление Усерекспериенцеаналитиксметрик

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [усерекспериенцеаналитиксметрик](../resources/intune-devices-userexperienceanalyticsmetric.md) .

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementManagedDevices.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложения|DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsRegressionSummary/modelRegression/{userExperienceAnalyticsMetricId}
PATCH /deviceManagement/userExperienceAnalyticsRegressionSummary/manufacturerRegression/{userExperienceAnalyticsMetricId}
PATCH /deviceManagement/userExperienceAnalyticsRegressionSummary/operatingSystemRegression/{userExperienceAnalyticsMetricId}
PATCH /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/deviceBootPerformanceMetrics/metricValues/{userExperienceAnalyticsMetricId}
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление объекта [усерекспериенцеаналитиксметрик](../resources/intune-devices-userexperienceanalyticsmetric.md) в формате JSON.

В следующей таблице приведены свойства, необходимые при создании [усерекспериенцеаналитиксметрик](../resources/intune-devices-userexperienceanalyticsmetric.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор метрики аналитики взаимодействия с пользователем.|
|значение|Двойное с плавающей точкой|Значение метрики аналитики взаимодействия с пользователем.|
|устройств|String|Единица измерения показателя взаимодействия с пользователем.|



## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [усерекспериенцеаналитиксметрик](../resources/intune-devices-userexperienceanalyticsmetric.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsRegressionSummary/modelRegression/{userExperienceAnalyticsMetricId}
Content-type: application/json
Content-length: 147

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsMetric",
  "value": "<Unknown Primitive Type Edm.Double>",
  "unit": "Unit value"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 196

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsMetric",
  "id": "1371822e-822e-1371-2e82-71132e827113",
  "value": "<Unknown Primitive Type Edm.Double>",
  "unit": "Unit value"
}
```



