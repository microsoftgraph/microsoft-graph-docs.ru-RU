---
title: Обновление Усерекспериенцеаналитиксдевицестартуппроцессперформанце
description: Обновление свойств объекта Усерекспериенцеаналитиксдевицестартуппроцессперформанце.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 94c3dc76d1b3dd75ec8b88541f78088a10e35b44
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48702063"
---
# <a name="update-userexperienceanalyticsdevicestartupprocessperformance"></a>Обновление Усерекспериенцеаналитиксдевицестартуппроцессперформанце

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [усерекспериенцеаналитиксдевицестартуппроцессперформанце](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) .

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
PATCH /deviceManagement/userExperienceAnalyticsDeviceStartupProcessPerformance/{userExperienceAnalyticsDeviceStartupProcessPerformanceId}
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Тело запроса
В тексте запроса добавьте представление объекта [усерекспериенцеаналитиксдевицестартуппроцессперформанце](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) в формате JSON.

В следующей таблице приведены свойства, необходимые при создании [усерекспериенцеаналитиксдевицестартуппроцессперформанце](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор производительности процесса запуска устройства Analytics User Experience.|
|процесснаме|Строка|Имя процесса запуска устройства службы аналитики взаимодействия с пользователем.|
|productName|String|Имя продукта для процесса запуска устройства Analytics Device (взаимодействие с пользователем).|
|publisher|String|Издатель процесса запуска устройства Analytics User Experience.|
|deviceCount|Int64|Сводка по процессу запуска при запуске устройства с пользовательским интерфейсом.|
|медианимпактинмс|Int32|Поведение при запуске устройства Analytics для пользователя в течение среднего влияния в миллисекундах.|
|тоталимпактинмс|Int32|Общее влияние на процесс запуска пользователя при запуске устройства Analytics (в миллисекундах).|



## <a name="response"></a>Ответ
В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [усерекспериенцеаналитиксдевицестартуппроцессперформанце](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDeviceStartupProcessPerformance/{userExperienceAnalyticsDeviceStartupProcessPerformanceId}
Content-type: application/json
Content-length: 285

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceStartupProcessPerformance",
  "processName": "Process Name value",
  "productName": "Product Name value",
  "publisher": "Publisher value",
  "deviceCount": 11,
  "medianImpactInMs": 0,
  "totalImpactInMs": 15
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 334

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceStartupProcessPerformance",
  "id": "86c4355c-355c-86c4-5c35-c4865c35c486",
  "processName": "Process Name value",
  "productName": "Product Name value",
  "publisher": "Publisher value",
  "deviceCount": 11,
  "medianImpactInMs": 0,
  "totalImpactInMs": 15
}
```





