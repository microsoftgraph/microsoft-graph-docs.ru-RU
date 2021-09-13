---
title: Обновление userExperienceAnalyticsModelScores
description: Обновление свойств объекта userExperienceAnalyticsModelScores.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 86f53d1bfae0f23dc8cae64983334a9fa28875e6
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59065381"
---
# <a name="update-userexperienceanalyticsmodelscores"></a>Обновление userExperienceAnalyticsModelScores

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [userExperienceAnalyticsModelScores.](../resources/intune-devices-userexperienceanalyticsmodelscores.md)

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
PATCH /deviceManagement/userExperienceAnalyticsModelScores/{userExperienceAnalyticsModelScoresId}
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для [объекта userExperienceAnalyticsModelScores.](../resources/intune-devices-userexperienceanalyticsmodelscores.md)

В следующей таблице показаны свойства, необходимые при создании [пользователяExperienceAnalyticsModelScores.](../resources/intune-devices-userexperienceanalyticsmodelscores.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор модели аналитики пользовательского интерфейса засмеяет объект.|
|model|String|Уникальный идентификатор оценки моделей аналитики пользовательских интерфейсов: модель устройства.|
|manufacturer|String|Уникальный идентификатор оценки моделей аналитики пользовательских интерфейсов: производитель устройств.|
|modelDeviceCount|Int64|Количество устройств модели аналитики пользовательских интерфейсов. Допустимые значения -9.2237203685478E+18 до 9.22337203685478E+18|
|endpointAnalyticsScore|Двойное с плавающей точкой|Оценка модели аналитики пользовательского опыта. Допустимые значения -1.79769313486232E+308 до 1.797693133486232E+308|
|startupPerformanceScore|Двойное с плавающей точкой|Оценка производительности запуска модели аналитики пользовательских интерфейсов. Допустимые значения -1.79769313486232E+308 до 1.797693133486232E+308|
|appReliabilityScore|Двойное с плавающей точкой|Оценка надежности приложения для аналитики пользовательского интерфейса. Допустимые значения -1.79769313486232E+308 до 1.797693133486232E+308|
|healthStatus|[userExperienceAnalyticsHealthState](../resources/intune-devices-userexperienceanalyticshealthstate.md)|Состояние состояния модели аналитики пользовательских интерфейсов. Возможные значения: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.|



## <a name="response"></a>Отклик
В случае успеха этот метод возвращает код отклика и обновленный `200 OK` [объект userExperienceAnalyticsModelScores](../resources/intune-devices-userexperienceanalyticsmodelscores.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsModelScores/{userExperienceAnalyticsModelScoresId}
Content-type: application/json
Content-length: 351

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsModelScores",
  "model": "Model value",
  "manufacturer": "Manufacturer value",
  "modelDeviceCount": 0,
  "endpointAnalyticsScore": 7.333333333333333,
  "startupPerformanceScore": 7.666666666666667,
  "appReliabilityScore": 6.333333333333333,
  "healthStatus": "insufficientData"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 400

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsModelScores",
  "id": "f2c0f69c-f69c-f2c0-9cf6-c0f29cf6c0f2",
  "model": "Model value",
  "manufacturer": "Manufacturer value",
  "modelDeviceCount": 0,
  "endpointAnalyticsScore": 7.333333333333333,
  "startupPerformanceScore": 7.666666666666667,
  "appReliabilityScore": 6.333333333333333,
  "healthStatus": "insufficientData"
}
```



