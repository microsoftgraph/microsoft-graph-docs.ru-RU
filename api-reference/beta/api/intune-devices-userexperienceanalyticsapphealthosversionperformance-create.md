---
title: Создание userExperienceAnalyticsAppHealthOSVersionPerformance
description: Создание нового объекта userExperienceAnalyticsAppHealthOSVersionPerformance.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 80ae02ef79f06808a83997c494862d769e82bce2
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51136001"
---
# <a name="create-userexperienceanalyticsapphealthosversionperformance"></a>Создание userExperienceAnalyticsAppHealthOSVersionPerformance

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создание нового [объекта userExperienceAnalyticsAppHealthOSVersionPerformance.](../resources/intune-devices-userexperienceanalyticsapphealthosversionperformance.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированное (рабочая или учебная учетная запись)|DeviceManagementManagedDevices.ReadWrite.All|
|Делегированное (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsAppHealthOSVersionPerformance
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для объекта userExperienceAnalyticsAppHealthOSVersionPerformance.

В следующей таблице показаны свойства, необходимые при создании userExperienceAnalyticsAppHealthOSVersionPerformance.

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор объекта производительности версии оси для пользовательского интерфейса аналитики оси.|
|osVersion|String|Версия ОС, установленная на устройстве.|
|osBuildNumber|Строка|Номер сборки ОС, установленный на устройстве.|
|activeDeviceCount|Int32|Количество активных устройств для версии ОС. Допустимые значения -2147483648 до 2147483647|
|meanTimeToFailureInMinutes|Int32|Время сбоя для версии ОС в минутах. Допустимые значения -2147483648 до 2147483647|
|osVersionAppHealthScore|Двойное с плавающей точкой|Оценка состояния здоровья приложения в версии ОС. Допустимые значения -1.79769313486232E+308 до 1.797693133486232E+308|
|osVersionAppHealthStatus|Строка|Общее состояние состояния здоровья приложения в версии ОС.|



## <a name="response"></a>Отклик
В случае успеха этот метод возвращает код отклика и объект `201 Created` [userExperienceAnalyticsAppHealthOSVersionPerformance](../resources/intune-devices-userexperienceanalyticsapphealthosversionperformance.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthOSVersionPerformance
Content-type: application/json
Content-length: 357

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthOSVersionPerformance",
  "osVersion": "Os Version value",
  "osBuildNumber": "Os Build Number value",
  "activeDeviceCount": 1,
  "meanTimeToFailureInMinutes": 10,
  "osVersionAppHealthScore": 7.666666666666667,
  "osVersionAppHealthStatus": "Os Version App Health Status value"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 406

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthOSVersionPerformance",
  "id": "7c28e16b-e16b-7c28-6be1-287c6be1287c",
  "osVersion": "Os Version value",
  "osBuildNumber": "Os Build Number value",
  "activeDeviceCount": 1,
  "meanTimeToFailureInMinutes": 10,
  "osVersionAppHealthScore": 7.666666666666667,
  "osVersionAppHealthStatus": "Os Version App Health Status value"
}
```




