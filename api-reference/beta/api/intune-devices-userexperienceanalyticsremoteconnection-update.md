---
title: Обновление userExperienceAnalyticsRemoteConnection
description: Обновление свойств объекта userExperienceAnalyticsRemoteConnection.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a26b5bfaabe9a10eb77f7f3337138d47db0dea88
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51159139"
---
# <a name="update-userexperienceanalyticsremoteconnection"></a>Обновление userExperienceAnalyticsRemoteConnection

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [userExperienceAnalyticsRemoteConnection.](../resources/intune-devices-userexperienceanalyticsremoteconnection.md)

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
PATCH /deviceManagement/userExperienceAnalyticsRemoteConnection/{userExperienceAnalyticsRemoteConnectionId}
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для [объекта userExperienceAnalyticsRemoteConnection.](../resources/intune-devices-userexperienceanalyticsremoteconnection.md)

В следующей таблице показаны свойства, необходимые при создании [userExperienceAnalyticsRemoteConnection.](../resources/intune-devices-userexperienceanalyticsremoteconnection.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор объекта удаленного подключения для аналитики пользовательского интерфейса.|
|deviceId|String|ID устройства.|
|deviceName|String|Имя устройства.|
|model|String|Модель устройства аналитики пользовательских интерфейсов.|
|virtualNetwork|Строка|Виртуальная сеть аналитики пользовательских интерфейсов.|
|deviceCount|Int32|Количество удаленных подключений. Допустимые значения от 0 до 2147483647|
|cloudPcRoundTripTime|Двойное с плавающей точкой|Время круговой оконечности устройства облачного ПК. Допустимые значения от 0 до 1.79769313486232E+308|
|cloudPcSignInTime|Двойное с плавающей точкой|Вход во время устройства облачного ПК. Допустимые значения от 0 до 1.79769313486232E+308|
|remoteSignInTime|Двойное с плавающей точкой|Удаленный вход во время устройства облачного ПК. Допустимые значения от 0 до 1.79769313486232E+308|
|coreBootTime|Двойное с плавающей точкой|Основное время загрузки устройства облачного ПК. Допустимые значения от 0 до 1.79769313486232E+308|
|coreSignInTime|Двойное с плавающей точкой|Основной знак во время устройства облачного ПК. Допустимые значения от 0 до 1.79769313486232E+308|
|cloudPcFailurePercentage|Двойное с плавающей точкой|Вход в процент отказа облачного устройства PC. Допустимые значения: от 0 до 100|



## <a name="response"></a>Отклик
В случае успеха этот метод возвращает код отклика и обновленный объект `200 OK` [userExperienceAnalyticsRemoteConnection](../resources/intune-devices-userexperienceanalyticsremoteconnection.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsRemoteConnection/{userExperienceAnalyticsRemoteConnectionId}
Content-type: application/json
Content-length: 479

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsRemoteConnection",
  "deviceId": "Device Id value",
  "deviceName": "Device Name value",
  "model": "Model value",
  "virtualNetwork": "Virtual Network value",
  "deviceCount": 11,
  "cloudPcRoundTripTime": 6.666666666666667,
  "cloudPcSignInTime": 5.666666666666667,
  "remoteSignInTime": 5.333333333333333,
  "coreBootTime": 4.0,
  "coreSignInTime": 4.666666666666667,
  "cloudPcFailurePercentage": 8.0
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 528

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsRemoteConnection",
  "id": "9ecbcf80-cf80-9ecb-80cf-cb9e80cfcb9e",
  "deviceId": "Device Id value",
  "deviceName": "Device Name value",
  "model": "Model value",
  "virtualNetwork": "Virtual Network value",
  "deviceCount": 11,
  "cloudPcRoundTripTime": 6.666666666666667,
  "cloudPcSignInTime": 5.666666666666667,
  "remoteSignInTime": 5.333333333333333,
  "coreBootTime": 4.0,
  "coreSignInTime": 4.666666666666667,
  "cloudPcFailurePercentage": 8.0
}
```




