---
title: Создание hardwareConfigurationDeviceState
description: Создание нового объекта hardwareConfigurationDeviceState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3d8e2a81c7d706d45e56dae807cb54fe26661459
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2021
ms.locfileid: "61348502"
---
# <a name="create-hardwareconfigurationdevicestate"></a>Создание hardwareConfigurationDeviceState

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создание нового [объекта hardwareConfigurationDeviceState.](../resources/intune-deviceconfig-hardwareconfigurationdevicestate.md)

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
POST /deviceManagement/hardwareConfigurations/{hardwareConfigurationId}/deviceRunStates
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для объекта hardwareConfigurationDeviceState.

В следующей таблице показаны свойства, необходимые при создании оборудованияConfigurationDeviceState.

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Клавиша состояния состояния устройства конфигурации оборудования. Это свойство доступно только для чтения.|
|deviceName|String|Имя устройства|
|osVersion|String|Версия операционной системы устройства.|
|upn|String|Имя участника-пользователя (UPN).|
|internalVersion|Int32|Внутренняя версия Policy|
|lastStateUpdateDateTime|DateTimeOffset|Последний период выполнения конфигурации оборудования|
|configurationState|[runState](../resources/intune-shared-runstate.md)|Состояние конфигурации из последнего выполнения конфигурации оборудования. Возможные значения: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.|
|configurationOutput|Строка|Выход выполнения конфигурации оборудования|
|configurationError|Строка|Ошибка при выполнении конфигурации оборудования|



## <a name="response"></a>Отклик
В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект hardwareConfigurationDeviceState](../resources/intune-deviceconfig-hardwareconfigurationdevicestate.md) в теле ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/hardwareConfigurations/{hardwareConfigurationId}/deviceRunStates
Content-type: application/json
Content-length: 410

{
  "@odata.type": "#microsoft.graph.hardwareConfigurationDeviceState",
  "deviceName": "Device Name value",
  "osVersion": "Os Version value",
  "upn": "Upn value",
  "internalVersion": 15,
  "lastStateUpdateDateTime": "2017-01-01T00:02:58.4418045-08:00",
  "configurationState": "success",
  "configurationOutput": "Configuration Output value",
  "configurationError": "Configuration Error value"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 459

{
  "@odata.type": "#microsoft.graph.hardwareConfigurationDeviceState",
  "id": "74b9fcd8-fcd8-74b9-d8fc-b974d8fcb974",
  "deviceName": "Device Name value",
  "osVersion": "Os Version value",
  "upn": "Upn value",
  "internalVersion": 15,
  "lastStateUpdateDateTime": "2017-01-01T00:02:58.4418045-08:00",
  "configurationState": "success",
  "configurationOutput": "Configuration Output value",
  "configurationError": "Configuration Error value"
}
```




