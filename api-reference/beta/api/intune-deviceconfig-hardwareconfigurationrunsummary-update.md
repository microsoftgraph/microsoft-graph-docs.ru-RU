---
title: Обновление hardwareConfigurationRunSummary
description: Обновление свойств объекта hardwareConfigurationRunSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5657005360e6f66d361f9490481d2b89653ea244
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2021
ms.locfileid: "61348515"
---
# <a name="update-hardwareconfigurationrunsummary"></a>Обновление hardwareConfigurationRunSummary

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [hardwareConfigurationRunSummary.](../resources/intune-deviceconfig-hardwareconfigurationrunsummary.md)

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
PATCH /deviceManagement/hardwareConfigurations/{hardwareConfigurationId}/runSummary
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для [объекта hardwareConfigurationRunSummary.](../resources/intune-deviceconfig-hardwareconfigurationrunsummary.md)

В следующей таблице показаны свойства, необходимые при создании [оборудованияConfigurationRunSummary.](../resources/intune-deviceconfig-hardwareconfigurationrunsummary.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Клавиша конфигурации оборудования выполнить сводную сущность. Это свойство доступно только для чтения.|
|successfulDeviceCount|Int32|Количество устройств, для которых оборудование настроено без проблем|
|failedDeviceCount|Int32|Количество устройств, для которых конфигурация оборудования обнаружила проблему|
|pendingDeviceCount|Int32|Количество устройств, для которых конфигурация оборудования находится в ожидаемом состоянии|
|errorDeviceCount|Int32|Количество устройств, для которых состояние конфигурации оборудования является ошибкой|
|notApplicableDeviceCount|Int32|Количество устройств, для которых не применимо состояние конфигурации оборудования|
|unknownDeviceCount|Int32|Количество устройств, для которых неизвестно состояние конфигурации оборудования|
|successfulUserCount|Int32|Число пользователей, для которых оборудование настроено без каких-либо проблем|
|failedUserCount|Int32|Число пользователей, для которых конфигурация оборудования обнаружила проблему|
|pendingUserCount|Int32|Число пользователей, для которых конфигурация оборудования находится в ожидаемом состоянии|
|errorUserCount|Int32|Число пользователей, для которых состояние конфигурации оборудования является ошибкой|
|notApplicableUserCount|Int32|Число пользователей, для которых не применимо состояние конфигурации оборудования|
|unknownUserCount|Int32|Число пользователей, для которых неизвестно состояние конфигурации оборудования|
|lastRunDateTime|DateTimeOffset|Время последнего запуска конфигурации на всех устройствах|



## <a name="response"></a>Отклик
В случае успешной работы этот метод возвращает код отклика и обновленный объект `200 OK` [hardwareConfigurationRunSummary](../resources/intune-deviceconfig-hardwareconfigurationrunsummary.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/hardwareConfigurations/{hardwareConfigurationId}/runSummary
Content-type: application/json
Content-length: 469

{
  "@odata.type": "#microsoft.graph.hardwareConfigurationRunSummary",
  "successfulDeviceCount": 5,
  "failedDeviceCount": 1,
  "pendingDeviceCount": 2,
  "errorDeviceCount": 0,
  "notApplicableDeviceCount": 8,
  "unknownDeviceCount": 2,
  "successfulUserCount": 3,
  "failedUserCount": 15,
  "pendingUserCount": 0,
  "errorUserCount": 14,
  "notApplicableUserCount": 6,
  "unknownUserCount": 0,
  "lastRunDateTime": "2016-12-31T23:57:28.499537-08:00"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 518

{
  "@odata.type": "#microsoft.graph.hardwareConfigurationRunSummary",
  "id": "76b964f2-64f2-76b9-f264-b976f264b976",
  "successfulDeviceCount": 5,
  "failedDeviceCount": 1,
  "pendingDeviceCount": 2,
  "errorDeviceCount": 0,
  "notApplicableDeviceCount": 8,
  "unknownDeviceCount": 2,
  "successfulUserCount": 3,
  "failedUserCount": 15,
  "pendingUserCount": 0,
  "errorUserCount": 14,
  "notApplicableUserCount": 6,
  "unknownUserCount": 0,
  "lastRunDateTime": "2016-12-31T23:57:28.499537-08:00"
}
```




