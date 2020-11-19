---
title: Получение Усерекспериенцеаналитиксовервиев
description: Чтение свойств и связей объекта Усерекспериенцеаналитиксовервиев.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c6d414ad8a4fb968dea084268ba78a170f2ca8dc
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49233966"
---
# <a name="get-userexperienceanalyticsoverview"></a>Получение Усерекспериенцеаналитиксовервиев

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Чтение свойств и связей объекта [усерекспериенцеаналитиксовервиев](../resources/intune-devices-userexperienceanalyticsoverview.md) .

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsOverview
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.

## <a name="request-headers"></a>Заголовки запросов
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [усерекспериенцеаналитиксовервиев](../resources/intune-devices-userexperienceanalyticsoverview.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsOverview
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 853

{
  "value": {
    "@odata.type": "#microsoft.graph.userExperienceAnalyticsOverview",
    "id": "8228da2b-da2b-8228-2bda-28822bda2882",
    "overallScore": 12,
    "deviceBootPerformanceOverallScore": 1,
    "bestPracticesOverallScore": 9,
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
    "bestPracticesHealthState": "insufficientData"
  }
}
```




