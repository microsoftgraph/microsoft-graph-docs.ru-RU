---
title: Обновление userExperienceAnalyticsBatteryHealthDeviceRuntimeHistory
description: Обновление свойств объекта userExperienceAnalyticsBatteryHealthDeviceRuntimeHistory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 74862de35ed29c0a1eb5c9e1ee0de8c3e6ae7f3f
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60697435"
---
# <a name="update-userexperienceanalyticsbatteryhealthdeviceruntimehistory"></a>Обновление userExperienceAnalyticsBatteryHealthDeviceRuntimeHistory

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [userExperienceAnalyticsBatteryHealthDeviceRuntimeHistory.](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceruntimehistory.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementManagedDevices.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Application|DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsBatteryHealthDeviceRuntimeHistory/{userExperienceAnalyticsBatteryHealthDeviceRuntimeHistoryId}
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для [объекта userExperienceAnalyticsBatteryHealthDeviceRuntimeHistory.](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceruntimehistory.md)

В следующей таблице показаны свойства, необходимые при создании [пользователяExperienceAnalyticsBatteryHealthDeviceRuntimeHistory.](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceruntimehistory.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор объекта для аналитики пользовательского интерфейса для запуска заряда батареи.|
|deviceId|String|Уникальный идентификатор устройства, идентификатор устройства Intune DeviceID или SCCM.|
|runtimeDateTime|String|Время даты для экземпляра истории запуска.|
|estimatedRuntimeInMinutes|Int32|Предполагаемое время работы устройства при полной зарядке батареи. Единица в минутах. Допустимые значения 2147483648 2147483647|



## <a name="response"></a>Отклик
В случае успешной работы этот метод возвращает код ответа и обновленный объект `200 OK` [userExperienceAnalyticsBatteryHealthDeviceRuntimeHistory](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceruntimehistory.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsBatteryHealthDeviceRuntimeHistory/{userExperienceAnalyticsBatteryHealthDeviceRuntimeHistoryId}
Content-type: application/json
Content-length: 216

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBatteryHealthDeviceRuntimeHistory",
  "deviceId": "Device Id value",
  "runtimeDateTime": "Runtime Date Time value",
  "estimatedRuntimeInMinutes": 9
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 265

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBatteryHealthDeviceRuntimeHistory",
  "id": "0fbcbdaf-bdaf-0fbc-afbd-bc0fafbdbc0f",
  "deviceId": "Device Id value",
  "runtimeDateTime": "Runtime Date Time value",
  "estimatedRuntimeInMinutes": 9
}
```



