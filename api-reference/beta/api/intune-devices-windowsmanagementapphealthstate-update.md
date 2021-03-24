---
title: Обновление windowsManagementAppHealthState
description: Обновление свойств объекта windowsManagementAppHealthState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 88bfa7732662a1a3d2d0f7b60835a3a83bde90ad
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51126327"
---
# <a name="update-windowsmanagementapphealthstate"></a>Обновление windowsManagementAppHealthState

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [windowsManagementAppHealthState.](../resources/intune-devices-windowsmanagementapphealthstate.md)

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
PATCH /deviceAppManagement/windowsManagementApp/healthStates/{windowsManagementAppHealthStateId}
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса укажи представление JSON для [объекта WindowsManagementAppHealthState.](../resources/intune-devices-windowsmanagementapphealthstate.md)

В следующей таблице показаны свойства, необходимые при создании [windowsManagementAppHealthState.](../resources/intune-devices-windowsmanagementapphealthstate.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор для состояния здоровья приложения управления Windows. Это свойство доступно только для чтения.|
|healthState|[healthState](../resources/intune-devices-healthstate.md)|Состояние здоровья приложения управления Windows. Возможные значения: `unknown`, `healthy`, `unhealthy`.|
|installedVersion|Строка|Установленная версия приложения для управления Windows.|
|lastCheckInDateTime|DateTimeOffset|Приложение для управления Windows во время последней проверки.|
|deviceName|String|Имя устройства, на котором установлено приложение для управления Windows.|
|deviceOSVersion|Строка|Windows 10 ОС версии устройства, на котором установлено приложение для управления Windows.|



## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код отклика и обновленный `200 OK` [объект WindowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/windowsManagementApp/healthStates/{windowsManagementAppHealthStateId}
Content-type: application/json
Content-length: 300

{
  "@odata.type": "#microsoft.graph.windowsManagementAppHealthState",
  "healthState": "healthy",
  "installedVersion": "Installed Version value",
  "lastCheckInDateTime": "2016-12-31T23:59:56.413532-08:00",
  "deviceName": "Device Name value",
  "deviceOSVersion": "Device OSVersion value"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 349

{
  "@odata.type": "#microsoft.graph.windowsManagementAppHealthState",
  "id": "5c7e50fb-50fb-5c7e-fb50-7e5cfb507e5c",
  "healthState": "healthy",
  "installedVersion": "Installed Version value",
  "lastCheckInDateTime": "2016-12-31T23:59:56.413532-08:00",
  "deviceName": "Device Name value",
  "deviceOSVersion": "Device OSVersion value"
}
```




