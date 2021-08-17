---
title: Обновление userExperienceAnalyticsScoreHistory
description: Обновление свойств объекта userExperienceAnalyticsScoreHistory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d2beea28e8e6c5ef9165cb42058cf72733ed49ca
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58264264"
---
# <a name="update-userexperienceanalyticsscorehistory"></a>Обновление userExperienceAnalyticsScoreHistory

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [userExperienceAnalyticsScoreHistory.](../resources/intune-devices-userexperienceanalyticsscorehistory.md)

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
PATCH /deviceManagement/userExperienceAnalyticsScoreHistory/{userExperienceAnalyticsScoreHistoryId}
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для [объекта userExperienceAnalyticsScoreHistory.](../resources/intune-devices-userexperienceanalyticsscorehistory.md)

В следующей таблице показаны свойства, необходимые при создании [userExperienceAnalyticsScoreHistory.](../resources/intune-devices-userexperienceanalyticsscorehistory.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор процесса запуска устройства аналитики пользовательского интерфейса.|
|startupDateTime|DateTimeOffset|Время запуска устройства аналитики пользовательского интерфейса.|
|overallScore|Int32|Общая оценка аналитики пользовательского опыта. Оценка будет в диапазоне 0-100, 100 является идеальным показателем. Допустимые значения: от 0 до 100|
|startupScore|Int32|Оценка запуска устройства аналитики пользовательских интерфейсов. Оценка будет в диапазоне 0-100, 100 является идеальным показателем.|
|coreBootScore|Int32|Оценка загрузки основного загрузочного устройства для аналитики пользовательского интерфейса. Оценка будет в диапазоне 0-100, 100 является идеальным показателем.|
|coreSigninScore|Int32|Оценка основного входного знака устройства для аналитики пользовательского интерфейса. Оценка будет в диапазоне 0-100, 100 является идеальным показателем.|
|recommendedSoftwareScore|Int32|Оценка основного входного знака устройства для аналитики пользовательского интерфейса. Оценка будет в диапазоне 0-100, 100 является идеальным показателем.|
|appHealthOverallScore|Int32|Общее состояние здоровья приложения для аналитики пользовательского интерфейса.|
|startupTotalDevices|Int32|Общее число устройств для производительности запуска для аналитики пользовательских интерфейсов.|
|recommendedSoftwareTotalDevices|Int32|Общее число устройств категории аналитики пользовательских интерфейсов рекомендуемого программного обеспечения.|
|appHealthTotalDevices|Int32|Общее число устройств для здоровья приложения для аналитики пользовательского интерфейса.|
|restartScore|Int32|Оценка перезапуска. Оценка будет в диапазоне 0-100, 100 является идеальным показателем, 0 указывает на чрезмерные перезапуски. Допустимые значения от 0 до 9999999|



## <a name="response"></a>Отклик
В случае успеха этот метод возвращает код ответа и обновленный объект `200 OK` [userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsScoreHistory/{userExperienceAnalyticsScoreHistoryId}
Content-type: application/json
Content-length: 422

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsScoreHistory",
  "startupDateTime": "2017-01-01T00:03:13.1084278-08:00",
  "overallScore": 12,
  "startupScore": 12,
  "coreBootScore": 13,
  "coreSigninScore": 15,
  "recommendedSoftwareScore": 8,
  "appHealthOverallScore": 5,
  "startupTotalDevices": 3,
  "recommendedSoftwareTotalDevices": 15,
  "appHealthTotalDevices": 5,
  "restartScore": 12
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 471

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsScoreHistory",
  "id": "d15e3ba8-3ba8-d15e-a83b-5ed1a83b5ed1",
  "startupDateTime": "2017-01-01T00:03:13.1084278-08:00",
  "overallScore": 12,
  "startupScore": 12,
  "coreBootScore": 13,
  "coreSigninScore": 15,
  "recommendedSoftwareScore": 8,
  "appHealthOverallScore": 5,
  "startupTotalDevices": 3,
  "recommendedSoftwareTotalDevices": 15,
  "appHealthTotalDevices": 5,
  "restartScore": 12
}
```




