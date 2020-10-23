---
title: Обновление Девицеманажементдериведкредентиалсеттингс
description: Обновление свойств объекта Девицеманажементдериведкредентиалсеттингс.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b611c63d069e0abbf74490406c52af76bf5efa1a
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48706291"
---
# <a name="update-devicemanagementderivedcredentialsettings"></a>Обновление Девицеманажементдериведкредентиалсеттингс

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [девицеманажементдериведкредентиалсеттингс](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) .

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)||
| &nbsp; &nbsp; **Конфигурация устройства** | DeviceManagementConfiguration.ReadWrite.All|
| &nbsp;&nbsp; **Политика доступа к ресурсам** | DeviceManagementConfiguration.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений||
| &nbsp; &nbsp; **Конфигурация устройства** | DeviceManagementConfiguration.ReadWrite.All|
| &nbsp;&nbsp; **Политика доступа к ресурсам** | DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/derivedCredentials/{deviceManagementDerivedCredentialSettingsId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/derivedCredentialSettings
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosVpnConfiguration/derivedCredentialSettings
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosEnterpriseWiFiConfiguration/derivedCredentialSettings
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosEasEmailProfileConfiguration/derivedCredentialSettings
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosDerivedCredentialAuthenticationConfiguration/derivedCredentialSettings
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Тело запроса
В тексте запроса добавьте представление объекта [девицеманажементдериведкредентиалсеттингс](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) в формате JSON.

В следующей таблице приведены свойства, необходимые при создании [девицеманажементдериведкредентиалсеттингс](../resources/intune-shared-devicemanagementderivedcredentialsettings.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор для производных учетных данных|
|**Политика RA**|
|helpUrl|Строка|URL-адрес, который будет доступен конечным пользователям для получения производных учетных данных с помощью корпоративного портала.|
|displayName|Строка|Отображаемое имя профиля.|
|имени|deviceManagementDerivedCredentialIssuer|Производный поставщик учетных данных, который будет использоваться. Возможные значения: `intercede`, `entrustDatacard`, `purebred`.|
|notificationType|deviceManagementDerivedCredentialNotificationType|Методы, используемые для информирования конечного пользователя об открытии корпоративного портала для доставки в сеть Wi-Fi, VPN или профилей электронной почты, использующих сертификаты для устройства. Возможные значения: `none`, `companyPortal`, `email`.|


## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементдериведкредентиалсеттингс](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/derivedCredentialSettings
Content-type: application/json
Content-length: 83

{
  "@odata.type": "#microsoft.graph.deviceManagementDerivedCredentialSettings"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 132

{
  "@odata.type": "#microsoft.graph.deviceManagementDerivedCredentialSettings",
  "id": "bc650741-0741-bc65-4107-65bc410765bc"
}
```









