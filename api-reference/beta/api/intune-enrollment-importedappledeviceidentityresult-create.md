---
title: Создание importedAppleDeviceIdentityResult
description: Создание нового объекта importedAppleDeviceIdentityResult.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cd49bbd6af0897532540a08839bb7bcf36aa1ee1
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51135665"
---
# <a name="create-importedappledeviceidentityresult"></a>Создание importedAppleDeviceIdentityResult

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создание нового [объекта importedAppleDeviceIdentityResult.](../resources/intune-enrollment-importedappledeviceidentityresult.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированное (рабочая или учебная учетная запись)|DeviceManagementServiceConfig.ReadWrite.All|
|Делегированное (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|DeviceManagementServiceConfig.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для объекта importedAppleDeviceIdentityResult.

В следующей таблице показаны свойства, необходимые при создании импортируемогоAppleDeviceIdentityResult.

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта. Унаследованный от [импортируемогоAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|
|serialNumber|String|Серийный номер устройства, унаследованный от [импортируемого ОбъектаAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|
|requestedEnrollmentProfileId|Строка|Администратор ID профиля регистрации намерен применить к устройству во время следующей регистрации, унаследованной от [импортируемогоAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|
|requestedEnrollmentProfileAssignmentDateTime|DateTimeOffset|Профиль времени регистрации назначен устройству, унаследованной от [импортируемогоAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|
|isSupervised|Boolean|Указывает, контролируется ли устройство Apple. Дополнительные сведения: https://support.apple.com/HT202837 Унаследованные от [импортируемогоAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|
|discoverySource|[discoverySource](../resources/intune-enrollment-discoverysource.md);|Источник обнаружения устройств Apple. Наследуется [от импортируемогоAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md). Возможные значения: `unknown`, `adminImport`, `deviceEnrollmentProgram`.|
|isDeleted|Boolean|Указывает, удалено ли устройство из подразделения Apple Business Manager, унаследованной от [импортируемогоAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|
|createdDateTime|DateTimeOffset|Создано время даты устройства, унаследованной от [импортируемогоAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|
|lastContactedDateTime|DateTimeOffset|Время последней контактируемой даты устройства, унаследованной от [импортируемого ОбъектаAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|
|description|Строка|Описание устройства, унаследованной от [импортируемого ОбъектаAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|
|enrollmentState|[enrollmentState](../resources/intune-shared-enrollmentstate.md)|Состояние устройства в Intune Наследуется от [импортируемогоAppleDeviceIdentity.](../resources/intune-enrollment-importedappledeviceidentity.md) Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.|
|платформа|[платформа](../resources/intune-enrollment-platform.md)|Платформа устройства. Наследуется [от импортируемогоAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md). Возможные значения: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.|
|status|Boolean|Состояние удостоверения импортируемого устройства|



## <a name="response"></a>Отклик
В случае успешной работы этот метод возвращает код ответа и импортируемый `201 Created` [объектAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities
Content-type: application/json
Content-length: 544

{
  "@odata.type": "#microsoft.graph.importedAppleDeviceIdentityResult",
  "serialNumber": "Serial Number value",
  "requestedEnrollmentProfileId": "Requested Enrollment Profile Id value",
  "requestedEnrollmentProfileAssignmentDateTime": "2017-01-01T00:02:32.8167841-08:00",
  "isSupervised": true,
  "discoverySource": "adminImport",
  "isDeleted": true,
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "description": "Description value",
  "enrollmentState": "enrolled",
  "platform": "ios",
  "status": true
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 652

{
  "@odata.type": "#microsoft.graph.importedAppleDeviceIdentityResult",
  "id": "557cfb4a-fb4a-557c-4afb-7c554afb7c55",
  "serialNumber": "Serial Number value",
  "requestedEnrollmentProfileId": "Requested Enrollment Profile Id value",
  "requestedEnrollmentProfileAssignmentDateTime": "2017-01-01T00:02:32.8167841-08:00",
  "isSupervised": true,
  "discoverySource": "adminImport",
  "isDeleted": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "description": "Description value",
  "enrollmentState": "enrolled",
  "platform": "ios",
  "status": true
}
```




