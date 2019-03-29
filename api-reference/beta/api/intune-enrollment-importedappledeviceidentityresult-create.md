---
title: Создание Импортедаппледевицеидентитиресулт
description: Создание нового объекта Импортедаппледевицеидентитиресулт.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a03a0c982eda187c8dee2932139ca50e40535f28
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30968233"
---
# <a name="create-importedappledeviceidentityresult"></a>Создание Импортедаппледевицеидентитиресулт

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создание нового объекта [импортедаппледевицеидентитиресулт](../resources/intune-enrollment-importedappledeviceidentityresult.md) .

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementServiceConfig.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities
```

## <a name="request-headers"></a>Заголовки запросов
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление объекта Импортедаппледевицеидентитиресулт в формате JSON.

В следующей таблице приведены свойства, необходимые при создании Импортедаппледевицеидентитиресулт.

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта. НаСледуется от [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md)|
|serialNumber|String|Серийный номер устройства, наСледуемый от [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md)|
|Рекуестеденроллментпрофилеид|String|Идентификатор профиля регистрации администратор планирует применить к устройству во время следующей регистрации, унаследованной от [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md)|
|Рекуестеденроллментпрофилеассигнментдатетиме|DateTimeOffset|Профиль регистрации времени назначен устройству, унаследованному от [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md)|
|isSupervised|Boolean|Указывает, защищено ли устройство Apple. Дополнительные сведения: https://support.apple.com/en-us/HT202837 наследуются от [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md)|
|discoverySource;|[discoverySource](../resources/intune-enrollment-discoverysource.md);|Источник обнаружения устройств Apple. НаСледуется от [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md). Возможные значения: `unknown`, `adminImport`, `deviceEnrollmentProgram`.|
|createdDateTime|DateTimeOffset|Дата и время создания устройства, унаследованного от [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md)|
|Ластконтактеддатетиме|DateTimeOffset|Дата и время последнего обращения к устройству, унаследованному от [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md)|
|description|String|Описание устройства, наСледуемого из [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md)|
|Енроллментстате|[Енроллментстате](../resources/intune-enrollment-enrollmentstate.md)|Состояние устройства в Intune, наСледуемого из [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md). Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.|
|platform|[управляем](../resources/intune-enrollment-platform.md)|Платформа устройства. НаСледуется от [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md). Возможные значения: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.|
|status|Boolean|Состояние импортированного удостоверения устройства|



## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [импортедаппледевицеидентитиресулт](../resources/intune-enrollment-importedappledeviceidentityresult.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities
Content-type: application/json
Content-length: 522

{
  "@odata.type": "#microsoft.graph.importedAppleDeviceIdentityResult",
  "serialNumber": "Serial Number value",
  "requestedEnrollmentProfileId": "Requested Enrollment Profile Id value",
  "requestedEnrollmentProfileAssignmentDateTime": "2017-01-01T00:02:32.8167841-08:00",
  "isSupervised": true,
  "discoverySource": "adminImport",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "description": "Description value",
  "enrollmentState": "enrolled",
  "platform": "ios",
  "status": true
}
```

### <a name="response"></a>Отклик
Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 630

{
  "@odata.type": "#microsoft.graph.importedAppleDeviceIdentityResult",
  "id": "557cfb4a-fb4a-557c-4afb-7c554afb7c55",
  "serialNumber": "Serial Number value",
  "requestedEnrollmentProfileId": "Requested Enrollment Profile Id value",
  "requestedEnrollmentProfileAssignmentDateTime": "2017-01-01T00:02:32.8167841-08:00",
  "isSupervised": true,
  "discoverySource": "adminImport",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "description": "Description value",
  "enrollmentState": "enrolled",
  "platform": "ios",
  "status": true
}
```




