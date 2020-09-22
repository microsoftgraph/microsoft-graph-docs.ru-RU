---
title: Создание Усерекспериенцеаналитиксскорехистори
description: Создание нового объекта Усерекспериенцеаналитиксскорехистори.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: dd6345848b3637ece09b439b3b84fd2f1ec7a60b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48047451"
---
# <a name="create-userexperienceanalyticsscorehistory"></a>Создание Усерекспериенцеаналитиксскорехистори

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создание нового объекта [усерекспериенцеаналитиксскорехистори](../resources/intune-devices-userexperienceanalyticsscorehistory.md) .

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
POST /deviceManagement/userExperienceAnalyticsScoreHistory
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Тело запроса
В тексте запроса добавьте представление объекта Усерекспериенцеаналитиксскорехистори в формате JSON.

В следующей таблице приведены свойства, необходимые при создании Усерекспериенцеаналитиксскорехистори.

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор процесса запуска устройства аналитики взаимодействия с пользователем.|
|стартупдатетиме|DateTimeOffset|Дата и время запуска устройства Analytics Device Experience.|
|стартупскоре|Int32|Оценка запуска устройства Analytics для пользователя. Показатель будет находиться в диапазоне 0-100, 100 — идеальный показатель.|
|коребутскоре|Int32|Оценка загрузки ядра устройств для службы аналитики взаимодействия с пользователем. Показатель будет находиться в диапазоне 0-100, 100 — идеальный показатель.|
|коресигнинскоре|Int32|Показатель для входа в систему для устройства аналитики с пользовательским интерфейсом. Показатель будет находиться в диапазоне 0-100, 100 — идеальный показатель.|
|рекоммендедсофтварескоре|Int32|Показатель для входа в систему для устройства аналитики с пользовательским интерфейсом. Показатель будет находиться в диапазоне 0-100, 100 — идеальный показатель.|
|рестартскоре|Int32|Оценка перезапуска. Показатель будет находиться в диапазоне 0-100, 100 — идеальный показатель, 0 указывает на чрезмерные перегрузки. Допустимые значения — от 0 до 9999999|



## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [усерекспериенцеаналитиксскорехистори](../resources/intune-devices-userexperienceanalyticsscorehistory.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsScoreHistory
Content-type: application/json
Content-length: 266

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsScoreHistory",
  "startupDateTime": "2017-01-01T00:03:13.1084278-08:00",
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
Content-Length: 315

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsScoreHistory",
  "id": "d15e3ba8-3ba8-d15e-a83b-5ed1a83b5ed1",
  "startupDateTime": "2017-01-01T00:03:13.1084278-08:00",
  "startupScore": 12,
  "coreBootScore": 13,
  "coreSigninScore": 15,
  "recommendedSoftwareScore": 8,
  "restartScore": 12
}
```






