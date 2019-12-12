---
title: Обновление объекта enrollmentprofile
description: Обновление свойств объекта объекта enrollmentprofile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d6ef78ef7ade1a57456c28bfd295ef895f5eadd0
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39955352"
---
# <a name="update-enrollmentprofile"></a>Обновление объекта enrollmentprofile

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md) .

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
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
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Тело запроса
В тексте запроса добавьте представление объекта [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md) в формате JSON.

В следующей таблице приведены свойства, необходимые при создании [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|GUID объекта|
|displayName|Строка|Имя профиля|
|description|String|Описание профиля|
|рекуиресусераусентикатион|Boolean|Указывает, требуется ли для профиля проверка подлинности пользователя|
|конфигуратионендпоинтурл|Строка|URL-адрес конечной точки конфигурации, используемый для регистрации|
|enableAuthenticationViaCompanyPortal|Boolean|Указывает на проверку подлинности с помощью помощника по настройке Apple, а не корпоративного портала.|
|рекуирекомпанипорталонсетупассистантенролледдевицес|Boolean|Указывает, что корпоративный портал необходим на зарегистрированных устройствах помощника по настройке|



## <a name="response"></a>Ответ
В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
Content-type: application/json
Content-length: 370

{
  "@odata.type": "#microsoft.graph.enrollmentProfile",
  "displayName": "Display Name value",
  "description": "Description value",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
  "enableAuthenticationViaCompanyPortal": true,
  "requireCompanyPortalOnSetupAssistantEnrolledDevices": true
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 419

{
  "@odata.type": "#microsoft.graph.enrollmentProfile",
  "id": "012d8d5e-8d5e-012d-5e8d-2d015e8d2d01",
  "displayName": "Display Name value",
  "description": "Description value",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
  "enableAuthenticationViaCompanyPortal": true,
  "requireCompanyPortalOnSetupAssistantEnrolledDevices": true
}
```





