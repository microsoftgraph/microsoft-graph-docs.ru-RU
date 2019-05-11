---
title: Обновление Девицеманажементдериведкредентиалсеттингс
description: Обновление свойств объекта Девицеманажементдериведкредентиалсеттингс.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7b8068d18f3531dedd727b70f894201645622a78
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33957095"
---
# <a name="update-devicemanagementderivedcredentialsettings"></a>Обновление Девицеманажементдериведкредентиалсеттингс

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [девицеманажементдериведкредентиалсеттингс](../resources/intune-deviceconfig-devicemanagementderivedcredentialsettings.md) .

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementConfiguration.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosVpnConfiguration/derivedCredentialSettings
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosEnterpriseWiFiConfiguration/derivedCredentialSettings
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosEasEmailProfileConfiguration/derivedCredentialSettings
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosDerivedCredentialAuthenticationConfiguration/derivedCredentialSettings
```

## <a name="request-headers"></a>Заголовки запросов
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Тело запроса
В тексте запроса добавьте представление объекта [Девицеманажементдериведкредентиалсеттингс](../resources/intune-deviceconfig-devicemanagementderivedcredentialsettings.md) в формате JSON.

В следующей таблице приведены свойства, необходимые при создании [девицеманажементдериведкредентиалсеттингс](../resources/intune-deviceconfig-devicemanagementderivedcredentialsettings.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для производных учетных данных|
|helpUrl|Строка|URL-адрес, который будет доступен конечным пользователям для получения производных учетных данных с помощью корпоративного портала.|
|displayName|Строка|Отображаемое имя профиля.|
|имени|[Девицеманажементдериведкредентиалиссуер](../resources/intune-deviceconfig-devicemanagementderivedcredentialissuer.md)|Производный поставщик учетных данных, который будет использоваться. Возможные значения: `intercede`, `entrustDatacard`, `purebred`.|
|notificationType|[Девицеманажементдериведкредентиалнотификатионтипе](../resources/intune-deviceconfig-devicemanagementderivedcredentialnotificationtype.md)|Методы, используемые для информирования конечного пользователя об открытии корпоративного портала для доставки в сеть Wi-Fi, VPN или профилей электронной почты, использующих сертификаты для устройства. Возможные значения: `none`, `companyPortal`, `email`.|



## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементдериведкредентиалсеттингс](../resources/intune-deviceconfig-devicemanagementderivedcredentialsettings.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosVpnConfiguration/derivedCredentialSettings
Content-type: application/json
Content-length: 241

{
  "@odata.type": "#microsoft.graph.deviceManagementDerivedCredentialSettings",
  "helpUrl": "https://example.com/helpUrl/",
  "displayName": "Display Name value",
  "issuer": "entrustDatacard",
  "notificationType": "companyPortal"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 290

{
  "@odata.type": "#microsoft.graph.deviceManagementDerivedCredentialSettings",
  "id": "bc650741-0741-bc65-4107-65bc410765bc",
  "helpUrl": "https://example.com/helpUrl/",
  "displayName": "Display Name value",
  "issuer": "entrustDatacard",
  "notificationType": "companyPortal"
}
```




