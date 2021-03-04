---
title: Создание userExperienceAnalyticsRemoteConnection
description: Создание нового объекта userExperienceAnalyticsRemoteConnection.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5937a7bc044ff56776242e3446a71ca5dd45cbac
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446738"
---
# <a name="create-userexperienceanalyticsremoteconnection"></a>Создание userExperienceAnalyticsRemoteConnection

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создание нового [объекта userExperienceAnalyticsRemoteConnection.](../resources/intune-devices-userexperienceanalyticsremoteconnection.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
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
POST /deviceManagement/userExperienceAnalyticsRemoteConnection
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Тело запроса
В теле запроса поставляем представление JSON для объекта userExperienceAnalyticsRemoteConnection.

В следующей таблице показаны свойства, необходимые при создании userExperienceAnalyticsRemoteConnection.

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор объекта удаленного подключения для аналитики пользовательского интерфейса.|
|deviceId|String|ID устройства.|
|deviceName|String|Имя устройства.|
|model|String|Модель устройства аналитики пользовательских интерфейсов.|
|virtualNetwork|String|Виртуальная сеть аналитики пользовательских интерфейсов.|
|deviceCount|Int32|Количество удаленных подключений. Допустимые значения от 0 до 2147483647|
|cloudPcRoundTripTime|Двойное с плавающей точкой|Время круговой оконечности устройства облачного ПК. Допустимые значения от 0 до 1.79769313486232E+308|
|cloudPcSignInTime|Двойное с плавающей точкой|Вход во время устройства облачного ПК. Допустимые значения от 0 до 1.79769313486232E+308|
|remoteSignInTime|Двойное с плавающей точкой|Удаленный вход во время устройства облачного ПК. Допустимые значения от 0 до 1.79769313486232E+308|
|coreBootTime|Двойное с плавающей точкой|Основное время загрузки устройства облачного ПК. Допустимые значения от 0 до 1.79769313486232E+308|
|coreSignInTime|Двойное с плавающей точкой|Основной знак во время устройства облачного ПК. Допустимые значения от 0 до 1.79769313486232E+308|
|cloudPcFailurePercentage|Двойное с плавающей точкой|Вход в процент отказа облачного устройства PC. Допустимые значения: от 0 до 100|



## <a name="response"></a>Отклик
В случае успеха этот метод возвращает код отклика и `201 Created` [объект userExperienceAnalyticsRemoteConnection](../resources/intune-devices-userexperienceanalyticsremoteconnection.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsRemoteConnection
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
HTTP/1.1 201 Created
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




