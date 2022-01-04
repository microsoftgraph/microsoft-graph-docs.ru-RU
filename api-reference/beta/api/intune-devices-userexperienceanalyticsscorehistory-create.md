---
title: Создание userExperienceAnalyticsScoreHistory
description: Создание нового объекта userExperienceAnalyticsScoreHistory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bd24c7cdca18aa304ab3de785b215f1dcd3fae0c
ms.sourcegitcommit: 00ac72f7b1cdde4f71ff332c2e7953908ef9de52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/04/2022
ms.locfileid: "61712091"
---
# <a name="create-userexperienceanalyticsscorehistory"></a>Создание userExperienceAnalyticsScoreHistory

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создание нового [объекта userExperienceAnalyticsScoreHistory.](../resources/intune-devices-userexperienceanalyticsscorehistory.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementConfiguration.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|DeviceManagementConfiguration.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsScoreHistory
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для объекта userExperienceAnalyticsScoreHistory.

В следующей таблице показаны свойства, необходимые при создании пользовательского интерфейсаExperienceAnalyticsScoreHistory.

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор процесса запуска устройства аналитики пользовательского интерфейса.|
|startupDateTime|DateTimeOffset|Время запуска устройства аналитики пользовательского интерфейса.|
|overallScore|Int32|Общая оценка аналитики пользовательского опыта. Оценка будет в диапазоне 0-100, 100 является идеальным показателем. Допустимые значения: от 0 до 100|
|startupScore|Int32|Оценка запуска устройства аналитики пользовательских интерфейсов. Оценка будет в диапазоне 0-100, 100 является идеальным показателем.|
|coreBootScore|Int32|Оценка загрузки основного загрузочного устройства для аналитики пользовательского интерфейса. Оценка будет в диапазоне 0-100, 100 является идеальным показателем.|
|coreSigninScore|Int32|Оценка основного входного знака устройства для аналитики пользовательского интерфейса. Оценка будет в диапазоне 0-100, 100 является идеальным показателем.|
|recommendedSoftwareScore|Int32|Оценка основного входного знака устройства для аналитики пользовательского интерфейса. Оценка будет в диапазоне 0-100, 100 является идеальным показателем.|
|appHealthOverallScore|Int32|Общее состояние здоровья приложения для аналитики пользовательского интерфейса.|
|workFromAnywhereScore|Int32|Аналитика пользовательских интерфейсов работает из любой точки.|
|batteryHealthScore|Int32|Оценка состояния заряда батареи для аналитики пользовательского интерфейса.|
|startupTotalDevices|Int32|Общее число устройств для производительности запуска для аналитики пользовательских интерфейсов.|
|recommendedSoftwareTotalDevices|Int32|Общее число устройств категории аналитики пользовательских интерфейсов рекомендуемого программного обеспечения.|
|appHealthTotalDevices|Int32|Общее число устройств для здоровья приложения для аналитики пользовательского интерфейса.|
|workFromAnywhereTotalDevices|Int32|Общее число устройств категории аналитики пользовательских интерфейсов работает из любой точки мира.|
|batteryHealthTotalDevices|Int32|Общее число устройств для здоровья батареи категории аналитики пользовательских интерфейсов.|
|restartScore|Int32|Оценка перезапуска. Оценка будет в диапазоне 0-100, 100 является идеальным показателем, 0 указывает на чрезмерные перезапуски. Допустимые значения от 0 до 9999999|



## <a name="response"></a>Отклик
В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsScoreHistory
Content-type: application/json
Content-length: 555

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsScoreHistory",
  "startupDateTime": "2017-01-01T00:03:13.1084278-08:00",
  "overallScore": 12,
  "startupScore": 12,
  "coreBootScore": 13,
  "coreSigninScore": 15,
  "recommendedSoftwareScore": 8,
  "appHealthOverallScore": 5,
  "workFromAnywhereScore": 5,
  "batteryHealthScore": 2,
  "startupTotalDevices": 3,
  "recommendedSoftwareTotalDevices": 15,
  "appHealthTotalDevices": 5,
  "workFromAnywhereTotalDevices": 12,
  "batteryHealthTotalDevices": 9,
  "restartScore": 12
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 604

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
  "workFromAnywhereScore": 5,
  "batteryHealthScore": 2,
  "startupTotalDevices": 3,
  "recommendedSoftwareTotalDevices": 15,
  "appHealthTotalDevices": 5,
  "workFromAnywhereTotalDevices": 12,
  "batteryHealthTotalDevices": 9,
  "restartScore": 12
}
```




