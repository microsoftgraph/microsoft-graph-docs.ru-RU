---
title: Обновление userExperienceAnalyticsOverview
description: Обновление свойств объекта userExperienceAnalyticsOverview.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c1df141edc551b62aea8c32534aa852490d9772f
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51866708"
---
# <a name="update-userexperienceanalyticsoverview"></a>Обновление userExperienceAnalyticsOverview

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [userExperienceAnalyticsOverview.](../resources/intune-devices-userexperienceanalyticsoverview.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
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
PATCH /deviceManagement/userExperienceAnalyticsOverview
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для [объекта userExperienceAnalyticsOverview.](../resources/intune-devices-userexperienceanalyticsoverview.md)

В следующей таблице показаны свойства, необходимые при создании [userExperienceAnalyticsOverview.](../resources/intune-devices-userexperienceanalyticsoverview.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор обзора аналитики пользовательских интерфейсов.|
|overallScore|Int32|Общая оценка аналитики пользовательского опыта.|
|deviceBootPerformanceOverallScore|Int32|Общая оценка производительности загрузки устройства для аналитики пользовательского интерфейса.|
|bestPracticesOverallScore|Int32|Анализ пользовательских интерфейсов позволяет опытом работы с общим показателем.|
|workFromAnywhereOverallScore|Int32|Аналитика пользовательского интерфейса Работает с любого общего балла.|
|appHealthOverallScore|Int32|Общее состояние здоровья приложения для аналитики пользовательского интерфейса.|
|resourcePerformanceOverallScore|Int32|Общая оценка производительности ресурсов аналитики пользовательских ресурсов.|
|insights|[коллекция userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md)|Аналитические сведения о пользовательском опыте.|
|state|[userExperienceAnalyticsHealthState](../resources/intune-devices-userexperienceanalyticshealthstate.md)|Текущее состояние состояния состояния аналитики пользовательских интерфейсов. Возможные значения: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.|
|deviceBootPerformanceHealthState|[userExperienceAnalyticsHealthState](../resources/intune-devices-userexperienceanalyticshealthstate.md)|Текущее состояние состояния состояния аналитики пользовательского интерфейса категории BootPerformance. Возможные значения: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.|
|bestPracticesHealthState|[userExperienceAnalyticsHealthState](../resources/intune-devices-userexperienceanalyticshealthstate.md)|Текущее состояние здоровья категории аналитики пользовательских интерфейсов "BestPractices". Возможные значения: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.|
|workFromAnywhereHealthState|[userExperienceAnalyticsHealthState](../resources/intune-devices-userexperienceanalyticshealthstate.md)|Текущее состояние состояния здоровья аналитики пользовательских интерфейсов категории WorkFromAnywhere. Возможные значения: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.|
|appHealthState|[userExperienceAnalyticsHealthState](../resources/intune-devices-userexperienceanalyticshealthstate.md)|Текущее состояние здоровья категории аналитики пользовательских интерфейсов "BestPractices". Возможные значения: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.|
|resourcePerformanceHealthState|[userExperienceAnalyticsHealthState](../resources/intune-devices-userexperienceanalyticshealthstate.md)|Текущее состояние состояния здоровья в категории аналитики пользовательского интерфейса "ResourcePerformance". Возможные значения: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.|



## <a name="response"></a>Отклик
В случае успеха этот метод возвращает код отклика и обновленный `200 OK` [объект userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsOverview
Content-type: application/json
Content-length: 1005

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsOverview",
  "overallScore": 12,
  "deviceBootPerformanceOverallScore": 1,
  "bestPracticesOverallScore": 9,
  "workFromAnywhereOverallScore": 12,
  "appHealthOverallScore": 5,
  "resourcePerformanceOverallScore": 15,
  "insights": [
    {
      "@odata.type": "microsoft.graph.userExperienceAnalyticsInsight",
      "userExperienceAnalyticsMetricId": "User Experience Analytics Metric Id value",
      "insightId": "Insight Id value",
      "values": [
        {
          "@odata.type": "microsoft.graph.insightValueDouble",
          "value": 1.6666666666666667
        }
      ],
      "severity": "informational"
    }
  ],
  "state": "insufficientData",
  "deviceBootPerformanceHealthState": "insufficientData",
  "bestPracticesHealthState": "insufficientData",
  "workFromAnywhereHealthState": "insufficientData",
  "appHealthState": "insufficientData",
  "resourcePerformanceHealthState": "insufficientData"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1054

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsOverview",
  "id": "8228da2b-da2b-8228-2bda-28822bda2882",
  "overallScore": 12,
  "deviceBootPerformanceOverallScore": 1,
  "bestPracticesOverallScore": 9,
  "workFromAnywhereOverallScore": 12,
  "appHealthOverallScore": 5,
  "resourcePerformanceOverallScore": 15,
  "insights": [
    {
      "@odata.type": "microsoft.graph.userExperienceAnalyticsInsight",
      "userExperienceAnalyticsMetricId": "User Experience Analytics Metric Id value",
      "insightId": "Insight Id value",
      "values": [
        {
          "@odata.type": "microsoft.graph.insightValueDouble",
          "value": 1.6666666666666667
        }
      ],
      "severity": "informational"
    }
  ],
  "state": "insufficientData",
  "deviceBootPerformanceHealthState": "insufficientData",
  "bestPracticesHealthState": "insufficientData",
  "workFromAnywhereHealthState": "insufficientData",
  "appHealthState": "insufficientData",
  "resourcePerformanceHealthState": "insufficientData"
}
```




