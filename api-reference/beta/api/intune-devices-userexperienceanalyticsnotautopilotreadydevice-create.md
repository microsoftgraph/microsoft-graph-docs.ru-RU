---
title: Создание userExperienceAnalyticsNotAutopilotReadyDevice
description: Создание нового объекта userExperienceAnalyticsNotAutopilotReadyDevice.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3842a478ab89e03366a111a52aed901613959dce
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51159472"
---
# <a name="create-userexperienceanalyticsnotautopilotreadydevice"></a>Создание userExperienceAnalyticsNotAutopilotReadyDevice

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создание нового [объекта userExperienceAnalyticsNotAutopilotReadyDevice.](../resources/intune-devices-userexperienceanalyticsnotautopilotreadydevice.md)

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
POST /deviceManagement/userExperienceAnalyticsNotAutopilotReadyDevice
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для объекта userExperienceAnalyticsNotAutopilotReadyDevice.

В следующей таблице показаны свойства, необходимые при создании пользователяExperienceAnalyticsNotAutopilotReadyDevice.

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор устройства intune аналитики пользовательского интерфейса.|
|deviceName|String|Имя устройства intune.|
|serialNumber|String|Серийный номер устройства intune.|
|manufacturer|String|Производитель устройства intune.|
|model|String|Модель устройства intune.|
|managedBy|Строка|Устройство intune управляется.|
|autoPilotRegistered|Boolean|Автопилотрегистер устройства intune.|
|autoPilotProfileAssigned|Boolean|Автопилот Устройства intuneProfileAssigned.|
|azureAdRegistered|[azureAdRegisteredState](../resources/intune-devices-azureadregisteredstate.md)|Устройство intune azureAdRegistered. Возможные значения: `no`, `yes`, `unknown`.|
|azureAdJoinType|Строка|Azure Ad ad для устройства intune присоединяется кType.|



## <a name="response"></a>Отклик
В случае успеха этот метод возвращает код ответа и `201 Created` [объект userExperienceAnalyticsNotAutopilotReadyDevice](../resources/intune-devices-userexperienceanalyticsnotautopilotreadydevice.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsNotAutopilotReadyDevice
Content-type: application/json
Content-length: 422

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsNotAutopilotReadyDevice",
  "deviceName": "Device Name value",
  "serialNumber": "Serial Number value",
  "manufacturer": "Manufacturer value",
  "model": "Model value",
  "managedBy": "Managed By value",
  "autoPilotRegistered": true,
  "autoPilotProfileAssigned": true,
  "azureAdRegistered": "yes",
  "azureAdJoinType": "Azure Ad Join Type value"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 471

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsNotAutopilotReadyDevice",
  "id": "11c3ffd7-ffd7-11c3-d7ff-c311d7ffc311",
  "deviceName": "Device Name value",
  "serialNumber": "Serial Number value",
  "manufacturer": "Manufacturer value",
  "model": "Model value",
  "managedBy": "Managed By value",
  "autoPilotRegistered": true,
  "autoPilotProfileAssigned": true,
  "azureAdRegistered": "yes",
  "azureAdJoinType": "Azure Ad Join Type value"
}
```




