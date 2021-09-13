---
title: Обновление appleUserInitiatedEnrollmentProfile
description: Обновление свойств объекта appleUserInitiatedEnrollmentProfile.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e63e8f3647b508c3bf6919c1b5189ec1b7a8a1a9
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59124912"
---
# <a name="update-appleuserinitiatedenrollmentprofile"></a>Обновление appleUserInitiatedEnrollmentProfile

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [appleUserInitiatedEnrollmentProfile.](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementServiceConfig.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|DeviceManagementServiceConfig.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/appleUserInitiatedEnrollmentProfiles/{appleUserInitiatedEnrollmentProfileId}
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для [объекта appleUserInitiatedEnrollmentProfile.](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)

В следующей таблице показаны свойства, необходимые при создании [appleUserInitiatedEnrollmentProfile.](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|defaultEnrollmentType|[appleUserInitiatedEnrollmentType](../resources/intune-enrollment-appleuserinitiatedenrollmenttype.md)|Тип регистрации профиля по умолчанию. Возможные значения: `unknown`, `device`, `user`.|
|availableEnrollmentTypeOptions|[коллекция appleOwnerTypeEnrollmentType](../resources/intune-enrollment-appleownertypeenrollmenttype.md)|Список доступных параметров типа регистрации|
|id|String|GUID объекта|
|displayName|String|Имя профиля|
|description|String|Описание профиля|
|priority|Int32|Приоритет, 0 — самый высокий|
|платформа|[devicePlatformType](../resources/intune-enrollment-deviceplatformtype.md)|Платформа устройства. Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.|
|createdDateTime|DateTimeOffset|Время создания профиля|
|lastModifiedDateTime|DateTimeOffset|Последнее изменение профиля|



## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код ответа и обновленный `200 OK` [объект appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/appleUserInitiatedEnrollmentProfiles/{appleUserInitiatedEnrollmentProfileId}
Content-type: application/json
Content-length: 439

{
  "@odata.type": "#microsoft.graph.appleUserInitiatedEnrollmentProfile",
  "defaultEnrollmentType": "device",
  "availableEnrollmentTypeOptions": [
    {
      "@odata.type": "microsoft.graph.appleOwnerTypeEnrollmentType",
      "ownerType": "company",
      "enrollmentType": "device"
    }
  ],
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "platform": "androidForWork"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 611

{
  "@odata.type": "#microsoft.graph.appleUserInitiatedEnrollmentProfile",
  "defaultEnrollmentType": "device",
  "availableEnrollmentTypeOptions": [
    {
      "@odata.type": "microsoft.graph.appleOwnerTypeEnrollmentType",
      "ownerType": "company",
      "enrollmentType": "device"
    }
  ],
  "id": "5a11d98e-d98e-5a11-8ed9-115a8ed9115a",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "platform": "androidForWork",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```



