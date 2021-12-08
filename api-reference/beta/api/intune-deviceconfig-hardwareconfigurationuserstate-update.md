---
title: Обновление hardwareConfigurationUserState
description: Обновление свойств объекта hardwareConfigurationUserState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 502e007407fc8df86f2db41d7f99b6685b6c4f27
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2021
ms.locfileid: "61345601"
---
# <a name="update-hardwareconfigurationuserstate"></a>Обновление hardwareConfigurationUserState

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [hardwareConfigurationUserState.](../resources/intune-deviceconfig-hardwareconfigurationuserstate.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementConfiguration.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/hardwareConfigurations/{hardwareConfigurationId}/userRunStates/{hardwareConfigurationUserStateId}
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В корпусе запроса устрой представление JSON для [объекта hardwareConfigurationUserState.](../resources/intune-deviceconfig-hardwareconfigurationuserstate.md)

В следующей таблице показаны свойства, необходимые при создании [аппаратного устройстваConfigurationUserState.](../resources/intune-deviceconfig-hardwareconfigurationuserstate.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта состояния состояния скрипта конфигурации оборудования. Это свойство доступно только для чтения.|
|upn|Строка|Имя участника-пользователя (UPN)|
|userEmail|String|Адрес электронной почты пользователя|
|userName|String|Имя пользователя|
|lastStateUpdateDateTime|DateTimeOffset|Последний период времени при выполнении конфигурации оборудования|
|successfulDeviceCount|Int32|Количество устройств успеха для конкретного пользователя|
|failedDeviceCount|Int32|Неудалось количество устройств для конкретного пользователя|
|pendingDeviceCount|Int32|Ожидание подсчета устройств для определенного пользователя.|
|errorDeviceCount|Int32|Количество устройств ошибки для определенного пользователя.|
|notApplicableDeviceCount|Int32|Не применимое количество устройств для конкретного пользователя.|
|unknownDeviceCount|Int32|Неизвестное количество устройств для определенного пользователя.|



## <a name="response"></a>Отклик
В случае успешной работы этот метод возвращает код отклика и обновленный объект `200 OK` [hardwareConfigurationUserState](../resources/intune-deviceconfig-hardwareconfigurationuserstate.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/hardwareConfigurations/{hardwareConfigurationId}/userRunStates/{hardwareConfigurationUserStateId}
Content-type: application/json
Content-length: 406

{
  "@odata.type": "#microsoft.graph.hardwareConfigurationUserState",
  "upn": "Upn value",
  "userEmail": "User Email value",
  "userName": "User Name value",
  "lastStateUpdateDateTime": "2017-01-01T00:02:58.4418045-08:00",
  "successfulDeviceCount": 5,
  "failedDeviceCount": 1,
  "pendingDeviceCount": 2,
  "errorDeviceCount": 0,
  "notApplicableDeviceCount": 8,
  "unknownDeviceCount": 2
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 455

{
  "@odata.type": "#microsoft.graph.hardwareConfigurationUserState",
  "id": "303ad215-d215-303a-15d2-3a3015d23a30",
  "upn": "Upn value",
  "userEmail": "User Email value",
  "userName": "User Name value",
  "lastStateUpdateDateTime": "2017-01-01T00:02:58.4418045-08:00",
  "successfulDeviceCount": 5,
  "failedDeviceCount": 1,
  "pendingDeviceCount": 2,
  "errorDeviceCount": 0,
  "notApplicableDeviceCount": 8,
  "unknownDeviceCount": 2
}
```




