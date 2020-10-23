---
title: Обновление Усерекспериенцеаналитиксапфеалсаппликатионперформанце
description: Обновление свойств объекта Усерекспериенцеаналитиксапфеалсаппликатионперформанце.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e433f05f64b5290c5697e80bcf0cfbbb87d92075
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48694566"
---
# <a name="update-userexperienceanalyticsapphealthapplicationperformance"></a>Обновление Усерекспериенцеаналитиксапфеалсаппликатионперформанце

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [усерекспериенцеаналитиксапфеалсаппликатионперформанце](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) .

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
PATCH /deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformance/{userExperienceAnalyticsAppHealthApplicationPerformanceId}
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Тело запроса
В тексте запроса добавьте представление объекта [усерекспериенцеаналитиксапфеалсаппликатионперформанце](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) в формате JSON.

В следующей таблице приведены свойства, необходимые при создании [усерекспериенцеаналитиксапфеалсаппликатионперформанце](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор объекта производительности приложения аналитики взаимодействия с пользователем.|
|апфангкаунт|Int32|Число зависаний для приложения. Допустимые значения: от 2147483648 до 2147483647|
|апфеалсскоре|Двойное с плавающей точкой|Оценка работоспособности приложения. Допустимые значения — 1 79769313486232e308 E + 308 — 1 79769313486232e308 E + 308|
|апфеалсстатус|Строка|Общее состояние работоспособности приложения.|
|аллоргшеалсскоре|Двойное с плавающей точкой|Медианный показатель работоспособности приложения во всех организациях. Допустимые значения — 1 79769313486232e308 E + 308 — 1 79769313486232e308 E + 308|
|активедевицекаунт|Int32|Количество устройств, в которых приложение было активно. Допустимые значения: от 2147483648 до 2147483647|
|appName|String|Имя приложения.|
|appDisplayName|String|Понятное имя приложения.|
|апппублишер|Строка|Издатель приложения.|
|аппусажедуратион|Int32|Общее время использования приложения в минутах. Допустимые значения: от 2147483648 до 2147483647|
|аппкрашкаунт|Int32|Число сбоев для приложения. Допустимые значения: от 2147483648 до 2147483647|
|меантиметофаилуреинминутес|Int32|Среднее время до сбоя приложения в минутах. Допустимые значения: от 2147483648 до 2147483647|



## <a name="response"></a>Ответ
В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [усерекспериенцеаналитиксапфеалсаппликатионперформанце](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformance/{userExperienceAnalyticsAppHealthApplicationPerformanceId}
Content-type: application/json
Content-length: 473

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthApplicationPerformance",
  "appHangCount": 12,
  "appHealthScore": 4.666666666666667,
  "appHealthStatus": "App Health Status value",
  "allOrgsHealthScore": 6.0,
  "activeDeviceCount": 1,
  "appName": "App Name value",
  "appDisplayName": "App Display Name value",
  "appPublisher": "App Publisher value",
  "appUsageDuration": 0,
  "appCrashCount": 13,
  "meanTimeToFailureInMinutes": 10
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 522

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthApplicationPerformance",
  "id": "c7962a87-2a87-c796-872a-96c7872a96c7",
  "appHangCount": 12,
  "appHealthScore": 4.666666666666667,
  "appHealthStatus": "App Health Status value",
  "allOrgsHealthScore": 6.0,
  "activeDeviceCount": 1,
  "appName": "App Name value",
  "appDisplayName": "App Display Name value",
  "appPublisher": "App Publisher value",
  "appUsageDuration": 0,
  "appCrashCount": 13,
  "meanTimeToFailureInMinutes": 10
}
```





