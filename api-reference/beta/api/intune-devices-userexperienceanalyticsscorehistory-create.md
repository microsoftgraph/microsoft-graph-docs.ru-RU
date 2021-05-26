---
title: Создание userExperienceAnalyticsScoreHistory
description: Создание нового объекта userExperienceAnalyticsScoreHistory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2cee5d19742711a4ea6f0858d3054337fabf3309
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52663812"
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
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementManagedDevices.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|DeviceManagementManagedDevices.ReadWrite.All|

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
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для объекта userExperienceAnalyticsScoreHistory.

В следующей таблице показаны свойства, необходимые при создании пользовательского интерфейсаExperienceAnalyticsScoreHistory.

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор процесса запуска устройства аналитики пользовательского интерфейса.|
|startupDateTime|DateTimeOffset|Время запуска устройства аналитики пользовательского интерфейса.|
|overallScore|Int32|Общая оценка аналитики пользовательского опыта. Оценка будет в диапазоне 0-100, 100 является идеальным показателем. Допустимые значения: от 0 до 100|
|startupScore|Int32|Оценка запуска устройства аналитики пользовательских интерфейсов. Оценка будет в диапазоне 0-100, 100 является идеальным показателем.|
|coreBootScore|Int32|Оценка загрузки основного загрузочного устройства для аналитики пользовательского интерфейса. Оценка будет в диапазоне 0-100, 100 является идеальным показателем.|
|coreSigninScore|Int32|Оценка основного входного знака устройства для аналитики пользовательского интерфейса. Оценка будет в диапазоне 0-100, 100 является идеальным показателем.|
|recommendedSoftwareScore|Int32|Оценка основного входного знака устройства для аналитики пользовательского интерфейса. Оценка будет в диапазоне 0-100, 100 является идеальным показателем.|
|restartScore|Int32|Оценка перезапуска. Оценка будет в диапазоне 0-100, 100 является идеальным показателем, 0 указывает на чрезмерные перезапуски. Допустимые значения от 0 до 9999999|



## <a name="response"></a>Отклик
В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsScoreHistory
Content-type: application/json
Content-length: 289

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsScoreHistory",
  "startupDateTime": "2017-01-01T00:03:13.1084278-08:00",
  "overallScore": 12,
  "startupScore": 12,
  "coreBootScore": 13,
  "coreSigninScore": 15,
  "recommendedSoftwareScore": 8,
  "restartScore": 12
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 338

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsScoreHistory",
  "id": "d15e3ba8-3ba8-d15e-a83b-5ed1a83b5ed1",
  "startupDateTime": "2017-01-01T00:03:13.1084278-08:00",
  "overallScore": 12,
  "startupScore": 12,
  "coreBootScore": 13,
  "coreSigninScore": 15,
  "recommendedSoftwareScore": 8,
  "restartScore": 12
}
```




